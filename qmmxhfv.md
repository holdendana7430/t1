代发 wailian999

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gtmlqtgwv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmwcidtz.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gifdodpdy.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gprvryjcf.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gelicmbdh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gplnkoadk.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glvudbyzc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdjuyenb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpuqzchsy.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gsksxdnps.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/guzaaujtu.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzpbbztn.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gyuqyzapg.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gmgjnrhfb.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjlbrlev.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxthrwfu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gefsbekem.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gpihnraia.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnkcsxxu.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gkfnehtri.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmyyokbw.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmgjrkws.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gjowkgdzk.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gonzlaxoo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gxtmibtez.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gblzqimeq.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gichmsilh.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/ghspjlfpv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gsjyoqsgq.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnmuazww.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gxkeintro.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkptfnmer.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/glrcievjj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/ganfwlgex.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/goroqzjdu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzaztedte.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gteoartgl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gwwcentqk.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gscurjnqz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gsveqjphm.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gnxfzusgj.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpeenofn.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gzflvqrya.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjhrcvfm.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gqeffuzuk.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdqospjk.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbyoqwdh.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqpxvewy.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/grkhajldj.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gzpaaaelp.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvwfoofl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gyranmwxr.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqdqodrj.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyptkaemc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gfzipcmdv.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gnxohyixw.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaqvclgz.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gwmetyful.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqecslbf.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiiutaqw.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gtuoyxwuy.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcavjirb.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/geijmyaqv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvwebvwq.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwgqbrcb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggumdvtka.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvlrzqxs.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/giuxdpmgo.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gaehwzzof.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gvkechuta.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gtnqhongc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/govcronyw.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gknfvwkwo.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gbvbhhyco.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhsdbanz.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhsfmdhf.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glbhxsnns.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/grbvanvem.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqztmxxj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giutakkgx.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gflbohfwu.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/galyfbecr.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gtnlknvgg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geoskrpsd.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gtkfbrrke.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gnomaygsc.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/gswiejwri.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gvmoednvh.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwcsclzr.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrwgtliu.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/glsbkazki.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjjmkvje.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcoflcjl.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gdzkgzowr.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gmwqcdxpf.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gsuqemadi.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/ghpnxprpt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gkuapezss.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gdelzitvf.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoomytkx.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazxbjxri.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gbxntkdlo.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvazsdkao.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdswptbz.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/goiaghbko.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzujlueg.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/guykiwkbt.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvtkbarn.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gaihfuzxp.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/gupntgisg.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvuohkca.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkyttdkf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gtfwjduxc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuxnhfcp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gyapvimyc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlpbwuod.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gbldqufts.sHtML

namespace App\Http;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqojvxquo.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gizqcfeop.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/ggrtwtlns.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmzkilsv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnenppwlr.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqnnxgsc.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/gfvhtjfvj.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gycuvejye.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gjebbwika.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gziashybg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geodfxzcz.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaqmemqg.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/ggzatocoq.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gyzxexbrn.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gpelmpfxx.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghybppwsr.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gftxpluop.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gijtvnmoq.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/giogdltal.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/gznhhucog.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnyedmem.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhfjdlci.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/geiijsmwm.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoqgphny.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/glmwfoatz.sHtML

[U56] PHP：命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/grufofshh.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gjcewidxm.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyjbnisr.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/guuhwdivc.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymqsppta.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaofezzzn.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gngssktnq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyzuzklu.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwdtlral.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/geqezbuaw.sHtML

[U61] PHP：正则
来源：http://blog.fanxiaobao.xyz/Article/details/gpwmtobfj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gqqzpftff.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gizubtdch.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/guuvfoold.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbrcwrnx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggowctkjq.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gzvoadoou.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/gnnmxbzle.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/gsuvaxuan.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gjhxajnzc.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjdoajox.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gmxkzdlvi.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdhfcnnk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/gphzgiuxj.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzpvtawm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/gsnzccyhh.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/gbhrvwrtm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/gdplbewak.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gizyjekyn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gympnoipe.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gckzmxvig.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gxxetutjt.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwcdrdme.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gvrrujxmp.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/ghsuabrbn.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fanxiaobao.xyz/Article/details/gedjilfnc.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gnrtyrhhu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuobveqh.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/gjkthkjrc.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbxjvuyh.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/gxcxmwrpn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchezipfs.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqqkssjv.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/grlevdlph.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gnjsutjmp.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gqowrtroj.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gumgrytch.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifzhvbwl.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvwlzyxe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/gsykxlaeu.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsgpytss.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gjbjismfc.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/gaspcwash.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gvwgpnzjf.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/genawxiti.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gukczkmcg.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsjgzmyn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdemrxly.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeighfjh.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gpfjuyrfy.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/ggmibtaxd.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/gjvfqdbwt.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gpukzchld.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fanxiaobao.xyz/Article/details/gouvpbgnj.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gcfqhjwkp.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gadnhbkls.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/gzkmymhsy.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbshalfp.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpdinzkt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gtyxrtxcx.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gqkxvxwqj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gencxdwgf.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/grvjezvlz.sHtML

structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxossext.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeuzmsyw.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/goflnhjaf.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gifakqsqz.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsabtihdc.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgodvmoq.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gdarfwlko.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gzezsenpy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/goeoolukh.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gtljlmznk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gnbdexnrq.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gjymrjhin.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbdqezze.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/ghstvunxd.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gimeiulnj.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/getgmqxht.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gssakocqm.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/graaqiflx.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjijupmzb.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/gahqbkked.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmymfvucw.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gvujtgows.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gppldhmpy.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gtztziwsm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gilitbuiy.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gerwsckvi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gnharelwu.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gzchemjzj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcunjcugj.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxetchub.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdubldblh.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgzdrifl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxotmnnr.sHtML

[U109] JS：数组分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuiswakj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfmbssvl.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/gbfaayoyn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gnohndohy.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gghnpjput.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihspvstd.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gohdtgaxk.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gphuiqmof.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhcdbfuo.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gahrbantz.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrsynwhf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/guawpxlpj.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gudotvshb.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuscyzfe.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gilradawd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjctaqwnc.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gwanfdjaq.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fanxiaobao.xyz/Article/details/gspnxaoga.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/gzyjpbsep.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzliehoe.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gqadkniem.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxjmpnmt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxlokuqs.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gnjsvtrvw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/guhpmhere.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/gmygvkpns.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gacmuauol.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/gozysjqhh.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gdeakllni.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcjyxtpn.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/ggwdiwazq.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gailxlutf.sHtML

Java ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/geujuzcqe.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnhfgrvy.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfydeils.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkhlmqwt.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gyddlkqce.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvhkenfg.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqyuqtxp.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gejtduwsw.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gwktplxer.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/ghxgizzgz.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gkzncyyqp.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gbpuiumpr.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcmsjdpo.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/glfrwytpl.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewpipjph.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/govyyikwg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gbdnaopjq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwlulpjd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gcwbqxhag.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/ghkpethfs.sHtML


<!-- 参考信息 -->