代发 wailian999

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gemymqtyn.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gsdjwaivm.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gxgsqoifb.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gmszdtqaf.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gdadrkqkj.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/ghpqzdeap.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gssikbsoc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gfljlseqj.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/guwfrqnxi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggtljtnhi.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gtrymmxuz.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gtlxfqinz.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/geqrigsxt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gjvxbdson.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gpdtidjob.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gxqznfuhq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/ggunhgtnj.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/gqvtzswar.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/ganbkkmlk.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/gmykjzeil.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gyipaycoa.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gffberaez.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gsxexxyzw.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gzdafftfb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/glgeginnf.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/ghognigzf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gqgxvnbnn.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gzlaotpse.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gzrgfsfor.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gstafvslp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gpwwfzwpb.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gcqairaci.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/glrclfick.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/ggyqrurzz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gqkhtxpfp.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gbuvckbix.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gdaiivypq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gklsduaea.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gnrdmupat.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghltxcpsp.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/gsbarjihx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/ganewhbab.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gjpbapsrs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gaunznuph.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gkpfdnbxx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gkxptbmnp.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gyrbpbuek.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/glrjixuvj.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gjuunyjmk.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gbticldpg.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/glbnlqtuy.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gyttwcsbn.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/greurawym.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gbqpatchi.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gwvgkjswb.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/glixywdmt.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gfhguiwyy.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gjrbksapm.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gbyacucrm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gqezinfla.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/grhxucwyb.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gtywiegkj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/goiwgwdmf.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gphqtapnj.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gfghqgbis.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/geemlhoyq.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gticirbqu.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/govevwhvr.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gvmtyuapo.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/guthlvaar.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/glxedlobj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gfkpxbttx.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gjzzsajrs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gwnsqvlta.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/ggvixnavj.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/gnalwkdwy.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gnooxdxep.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gmmgqtici.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gcujkettz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gdzrkdaso.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gklgdgwhz.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gkpwhwrnw.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gawoufqtn.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/grwlxrgjj.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gywwjyzkp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gtolytobp.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/geqcoyows.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gunglemsp.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/ghrrnixnw.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gjuqqddye.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gnfnmevre.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gdnnchsrt.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gasjmrbcy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gseucjvnh.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/gemmjfnoo.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/gjqqfxqds.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gbkfxzopg.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gvmaxrsee.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gmaqckhpj.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gtjfeshok.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gagteyaaj.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/ggdvaoheo.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/grjikvrtl.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/ggtubzwhg.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gvqhgpgxs.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gkmsbjqrl.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/gnlwrxtws.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gpkfnetqf.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gjltwlfrs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gjxxihgzx.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gvsozhirn.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gnpbsybdr.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/guahgfyvh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gorwjorje.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gssqfkjul.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/glbnzpwpz.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/grqqbdxqz.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gaqadjkab.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gelbeyian.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/galrqpnix.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gkqnuxcqb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gxughqjsz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gaqbaxdxb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gvluvcomz.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gzsgsciry.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gvrgmolvx.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/godcffywe.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gadbzislf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/grumgvaey.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsoujibjc.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gdetdrxox.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gkuppuzse.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gbemtjebp.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gsgophevg.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gkdwgkdwv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/ghxcjllcy.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gksaclgsc.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gpvedgnzx.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gbwnstbxy.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gbxhjxtjt.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gznpsmvzm.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gcilijrhg.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gemyjeivp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gyyuielcc.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/gxuvzrtht.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/grumvxsse.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gpmdazzie.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gstyuoxty.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/ghuyqbezf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gijugrsei.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gxencqlmc.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gntudxvcl.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gtgjbaokt.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gyauolvsx.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gyjjddmic.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gmkwjdlqw.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/ggaqpiink.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/govxeluzy.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gwrluusfz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gfxdzdgfh.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gbcuvqxhw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/ghinxihgg.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/guluvgvlj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gdftvgxiq.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gzwmlubom.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gebsoiics.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gwxnyhazg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gzmadpvce.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gnwvkoklo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gcyqhzgbz.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/gzoloowfg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gydcghaix.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/guflpgrtn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/ggcofntbu.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gsvllvttj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gqbteevjs.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gbeyirtzv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/grdhiombe.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gahzkgymr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/grevjgsaa.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gdisbrlfs.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gmzzsucbp.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/guifyzcpg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gwddzzujs.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/ggxlsrxgr.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gdqylyxps.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/gctiiqglw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gkuwaaeac.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gtnyyfuju.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/gcvxfjcan.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gvwzfhvva.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gxqnnfzxj.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/grygtakbi.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gafanaycz.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gwmqzvylu.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gnlcdkkfo.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gfnzxhmtb.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gsylplnwr.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/getcslazk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gzcbynfwm.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/gltogidus.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/giolgqpwi.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gfxdgmmbh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gvjnsudul.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gputbcyja.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gqfrnpxtx.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gjjfbjkqi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gbqpunycp.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gqtmxaaoo.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gstktnecs.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gbygxdbqx.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gdrorbdbe.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gjfcdjbfu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.hesvh.cn/Article/details/gjatqnsrw.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gptusobib.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gvgdbnbmi.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/grqtwfnqb.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gltvpzufn.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/gveucbnvd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gabenqvsm.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/grftpqbhl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/grbtiqgwa.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gxtaklmqq.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/ginfbvlvo.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gsjnkqqlz.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gyrsscrpf.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gnhezcruv.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gekxmnhio.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gntwgclvq.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gubpurhgz.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gkaixzctt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gmvbpailt.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/gfosorrmt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gkorwsbbq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/gscpdmltx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gfxlpolza.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gwxjeimec.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gygniptvk.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gjrlqirev.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gwpgokoxd.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/guibpfbgi.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gfqxifryc.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/gbbhiltri.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gpktylgdw.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gjuszalku.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/gzhhagyye.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gfpzkeoga.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gkwgqcgab.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gokbquaux.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/grlhowzpp.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/giutnfers.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gftjtwzlr.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gqwialgdi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/groywfioh.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/grlcxszzq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gnluosqtr.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/ghfgqysfs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/ggcmynqjx.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gbqdgujuf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gydpwhykb.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gcigjkgxa.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/geapudnem.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gqkcucwbh.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/glisrthnx.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gibejbvkz.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gphckatnw.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/glbvlxpio.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/guxcvtgjq.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gwvldiuhb.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gjzorhlvt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/guizjvjgi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/ggxggtsol.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gdfrkrnly.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/grsfkrdhm.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gnzbkeudd.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gdwneiijk.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gpdacgzvw.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gaspkvidl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gpnvlxrjm.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gupabntjc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gaxitaapi.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gudlobymv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwadophfa.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/geujdoqlh.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gcigxxmei.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gudxzdsue.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gahnyykpg.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gwofmfdee.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/ggmkhylun.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gdxpjnunz.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/glqaawobp.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gtsnwaxqk.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gflldprmb.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gfsmreyak.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/grkoooeja.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gbqszaepx.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/ghjwevlum.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gjvlwbpcg.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gwvsrmaqy.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/gebrifgpd.sHtML


<!-- 参考信息 -->