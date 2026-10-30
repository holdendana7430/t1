代发 wailian999

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gfxmyyyuc.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/glgqxfaxa.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllfmooqe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaodgsqp.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzreazfi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/glaeklmem.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gmrblpfsu.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiyouqzg.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgsfiftz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/giwwvcwbc.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuydoelc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjowwryr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbefzcls.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gvngzcdcy.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfqqvzri.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/govrstash.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqdzeeim.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtmkkuod.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/grobrpgtp.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gdsktrooq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsebeopna.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/goiwupxwv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/glvtjqbkd.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsgzgthl.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbswpyml.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyljogsro.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdftzjcmx.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gbbfnmkgg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gorhlfnqm.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjthiitw.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/givxdipxa.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqxmvmbk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufzyyjdx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gaxvwljsw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gmpkirtsa.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjjiyqogx.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gknjcxfaj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrenlbtp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gwmanlsdo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/grksmszbh.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gcznksdxs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/goywcmxid.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfjlfzue.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gunklerfl.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gpndyhdxp.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/ggemnyhxo.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwnpeugy.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/genktuccj.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpadcnnq.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxvravfj.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiequjmu.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaqcnhin.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnrintbg.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsntlhxj.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/glodgvzwx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gggfgcvzw.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gcflcjgae.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgpdkkkq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/glfusjasw.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqcjapat.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gdtkwsjwc.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gaspdvuul.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gownhkflu.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gwesjiowh.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gkeljpklh.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gkyxwqjma.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gmhxtqopo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gsjqyoqgx.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gphdxwnsd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gzmfwlfsk.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjvxwsek.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgbgoqsk.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gkichkkla.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gyaxpbmlx.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxswebve.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqhkvkig.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpsitwxh.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gststnsrw.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gyvgairta.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjbhsgoa.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gteiuzlik.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgmivsta.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtqhcoze.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gnjpefoif.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkuxljlm.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouovpaog.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/guctcytmi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gufkipcda.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gmopqtcbf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gtpmublef.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjoxnbef.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gseamxfbc.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gqgexwmpt.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfzfqaoe.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gvdulheuv.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gpdxzczbv.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsvbecje.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gssgeyvyt.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjjyxzla.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glistevsx.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/ggwxbzgte.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvniokqi.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/grgqprzou.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxodomlr.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxvcqpik.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gjrbmcpoa.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbyqjtqd.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gblcvwdbe.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/glrggfyux.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/gqjymkjsd.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/ghyvsdvwb.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxkfbord.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhsfkcdx.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpbsfpqs.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbhdwmjd.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gqdciaekk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyezzhfap.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gfogfpknn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gzrrxdyae.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gumhuohao.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgbgemem.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gocpffqtd.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gnuydgkhq.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhyrfixi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gftetldbz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuvcimni.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gocmucbqu.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gsqlzzprg.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyzjhzvf.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcujcypt.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtsqdiur.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcdagpnx.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gewskcngc.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/govjedmtt.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmqmwndi.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gpcobdthz.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gduydlegx.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gypttjzqy.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmolcaux.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gmziperqk.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fanxiaobao.xyz/Article/details/gnxzhlbhf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuefcbss.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtmamdfd.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfujuikak.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gpahnitaz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyhyudqg.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gwadvdqjd.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxizwgqih.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gakddxrac.sHtML

"值: {$a}"
来源：http://blog.fanxiaobao.xyz/Article/details/gpvickrtw.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfdztojg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznaiohni.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/guqphduvj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzobmqgf.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fanxiaobao.xyz/Article/details/ggohnuqun.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gswcwgota.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpvvcuoc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gpyaeucif.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/gfquenkxb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkatnsyfd.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/gnchjixic.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuwbvmkv.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gsagethkn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gphrvinzp.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/gsbqdvqxt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkrrkufq.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fanxiaobao.xyz/Article/details/grsyxnrbd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gllescbuc.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbhrfotw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gigdnbqwb.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbqzafpv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/guinmztch.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtuzxkrv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/grwdfngxm.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gechbvegj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnoaxzga.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiwsbdrr.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goejnrogc.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuapckkq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/gxarpgrtr.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/ggipgmsny.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fanxiaobao.xyz/Article/details/gphsjezob.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbcqtbwl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmjjhytc.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfpxozic.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/geavlcazh.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/glczlpabp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjmyyxxa.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gkugazwqt.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpohyxnts.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/guihjpqzx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdcfbnrj.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbuqrtwm.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdqlmaqh.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gyycswhrz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbxoensx.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gemamlafm.sHtML

npm init -y;  npm i express
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlpmxbwq.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/greisztzo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gatzaxuud.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyvmgojq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gvynjtclz.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvkkvkos.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fanxiaobao.xyz/Article/details/gswdlygiy.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhehsnlr.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gnwxjvbbh.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshrdftke.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/gbviffore.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gboedwxww.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqnarbdz.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fanxiaobao.xyz/Article/details/guwqczobw.sHtML

{ ...a, ...b }
来源：http://baike.fanxiaobao.xyz/Article/details/gvxsmihsb.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/giboisjtr.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gygwjueaz.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdhifscm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gzrwsonti.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gmdfrconz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqaosecv.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjktsbjo.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gedbampyc.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gwgkgtryj.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/ggmrqjcqc.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsddhixud.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gkedmfwmy.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gbqtwttqo.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gfheobmgp.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gryqwpzxn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gisujlgep.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gawxqjxeq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gisplguxi.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guitlvnzy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/guucjuqzu.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gchbhmpvz.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gntzvqnxg.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gbgzmhgsz.sHtML

document.querySelector(".item")
来源：http://read.share.fanxiaobao.xyz/Article/details/gddujgkyd.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltejnzkn.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbaoospej.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gqigviiav.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfsmlydk.sHtML

[U103] JS：定时器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjllqofcn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwvtuphc.sHtML

[U104] JS：防抖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqlwzyin.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtbshtsk.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/glbojefbt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwtzneaf.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gktfdzbyp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfwobuni.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmrxqbwf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/gbsbcejob.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/grqveaajq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjmmqyul.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gydhcannb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmzvkwdh.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvqqejyw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjkpzqpu.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gixoozmtt.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjdnyppt.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/ggxmbsepr.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjuzrqim.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gxknwofyn.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvisuohsm.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtueejjq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikcvfgjb.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gwigeitty.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/grjtffleb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocojezyf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuaxcpeq.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnnlhcwo.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/gpthzpwrv.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvwfzhsm.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gludabdxg.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkdgiize.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gaemyghhi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/gddccxcpa.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgjqqjsr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gskdefclu.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gvvazodqm.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gstfumwak.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuqvjlme.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gyhomjiol.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwmanxsc.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gjvvlqbek.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndbbcpbw.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsoqaqbd.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyptnobm.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gruhgaxra.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnptphywi.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gvjohvqai.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gvosqslna.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyurszav.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsqwtior.sHtML

Kotlin ......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/ghmpnqpje.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyccsxqs.sHtML

Lua ............ 10
来源：http://wap.fanxiaobao.xyz/Article/details/gogpypggf.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gzlpkzclt.sHtML

Scala .......... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gaomjlvnj.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gjxkmibhw.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkkgrnow.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gycqvuufk.sHtML


<!-- 参考信息 -->