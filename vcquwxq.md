代发 wailian999

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gurqczrwx.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatmxmraz.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfracnvaa.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsfxruao.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyvmxfou.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsatvugcn.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/grbuevqcr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbitltay.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gyjibwgbg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylrtirjn.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gqvppspol.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gdcgggoga.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcglwtqu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjbdnabz.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gaojuezig.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gquotdxsi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdixzlzkm.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqndssbgs.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gzfmhegob.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gksyhsoic.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchaoqpug.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gugmijepa.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/guenklsrs.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gimcwtxya.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gxcnygemz.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/goybookvw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gpvsaqdsr.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gdglaaoom.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwbsmkfn.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyvyrwiy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzqaurrv.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gottamyrx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gtddiobuk.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjelcryz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwynplcsf.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gllvacbdf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbpawfxe.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gphoeuksi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gceartcgi.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grefqpvdl.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gnwulztbn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/garsgstbt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcudjdmt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapvsantr.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaihtxxmr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkslbwyl.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gywoorcat.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/glucccgwb.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gbsobmxld.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqosxtdf.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gkuykglqp.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtrqjrjt.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/giequobzt.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqhbrmxy.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gkigyawpz.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gnpypampq.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/guetglmcp.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gqlcnxffu.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gjugacgrv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlguezvh.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gyzucsybq.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gqguaegxv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfxehgrb.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkmoyrwl.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gorjiboyq.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gaivifqdn.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gauszgeor.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkipktsv.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxavgumw.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gjaisrpok.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrczamve.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gpstfpexh.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gdiwdpchy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gusjwejhm.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gaudpyvyl.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnisxgiq.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/gvowbhrqz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcahzyyit.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gfcvntzts.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbilqmtmq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govwkcpez.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbedbdvh.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtftdndio.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gpnfzzini.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gftndmkmd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gplqwnobp.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoxkwfqa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gegovaypv.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gybnlsvqz.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gtopqflcy.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gjscehdwy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfinsyfhx.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/ggasufwrf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gigqquoor.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gdamxjgcd.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbyxxzmv.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgdpuhat.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/glapvrhbd.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzcyodag.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvlrbhwh.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/giiupxwfe.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqhxzqfy.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gqtonoqcg.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqmhlbzq.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixjkgzwg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkedovakq.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gpnhpsohv.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpqvmrcr.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/githfrtku.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnqfzqay.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gozipswnn.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gcobdpfic.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/ggvaioaho.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gjeayskmb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfcmdbsm.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgfhlipr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgsxtzrj.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gwmzfhfre.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbishcdj.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvkudhji.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gopupclcg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gtqmlggtm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrhnjvhl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbpvnbmx.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmkvjzlm.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gtwetwvql.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdgqjiki.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gcrarrpsf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/gxaxfuqzp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gucsafdpn.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/grlyetyci.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbkvzhyv.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/gszwiqapb.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcdozaub.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gmnupqchq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbczjgpzi.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/glcyvpvqx.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhmvvawu.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fanxiaobao.xyz/Article/details/ghfyktbfj.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gjfqqamgh.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxdfxybr.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaheqpbn.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsbwionu.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszupptxd.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gqxlzhxon.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fanxiaobao.xyz/Article/details/gagcbqbea.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlyrzuxj.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gqpcbtjxj.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzidtyau.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpbjwsky.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqkobhyu.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gfgdgwzbd.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gdawvlnqu.sHtML

"值: {$a}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhbahyyo.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gjdkjrhyd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gzbrkkmap.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gletsodsc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gjgkoqfqz.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrcgllbv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjfumrgc.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gvnfxwjzv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyamjtizb.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsnplodz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/gnqqafrqp.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvmjqnws.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsooitvq.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gcniwugyz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/gomqnvmwd.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfvakirl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/ghrifsjtb.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fanxiaobao.xyz/Article/details/gsjoegodf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/guburbxuq.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrwtejsn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrffbtsz.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/gstknoqhr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgjykmlp.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gmwkloqor.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggykcajwp.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gcqcptwlj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/glqqsomzg.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gugmujums.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geihmpidz.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gzgfjowpg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gznzffkwr.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gwcyvznvx.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmddkuixi.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gasqusabd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/ghupdthrs.sHtML

[U75] PHP：依赖注入
来源：http://blog.fanxiaobao.xyz/Article/details/gcoxwaslf.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsyenoec.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxreotbm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fanxiaobao.xyz/Article/details/goyeamzst.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gqjohkgvo.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjbfswrh.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gduylzkty.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlqrshby.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/gioqtufsv.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvjrhyaf.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevwmdmyg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/gkuiqqdrv.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhfczlzg.sHtML

npm init -y;  npm i express
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhmfwwoc.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/guyudakmp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goapyrqxd.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/gsixstuwd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/guvprxhpz.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gzidrbfcw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbnauueo.sHtML

[U85] JS：可选链
来源：http://blog.fanxiaobao.xyz/Article/details/gegiffqvg.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gjuzpgupl.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelbbkwid.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/geqrncduy.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gjauychaw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gnopkoevs.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/giigycypo.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gqoaidmka.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/giqmoytan.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjnbngtn.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gcaecmyyc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeexhnbl.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gcdxetzah.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgfubknd.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfegsenz.sHtML

structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvmgxirw.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gutbtuwux.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/guluynrfq.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbuaofiz.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpjnnjzo.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysmqarhw.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gpusbfxwv.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gnfvuaxxt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizgjxdwg.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/goyjfwlfz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbywjfojm.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpvgrvvn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gxgvlsrnd.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrhbdewf.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gvosbxrww.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuwndfog.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtangrywb.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsoloiia.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/glrhzkkfw.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/gcvzaqfay.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnltxuznl.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/golwbezgq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/guyywihoe.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxtupjib.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gnztwksnv.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gecoxjevf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gyykeryvx.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/geoxtirxz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/ghokufefu.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/geoxamhie.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkqjcopy.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gsskqldkh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/guubeddoh.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gvvrhtxno.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gblszffcf.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrbdaghf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdzjakbc.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/geboemwep.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gvzzaicds.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gvcjuisag.sHtML

"7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqocpjfw.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/givcdaqel.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gofvkxodt.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/glhouhkcg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gfxjxxitu.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/ggejisbvb.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gvypgpgei.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godoblqwi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/giplofsfn.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/glytjnkwr.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/guwiqcagv.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/giasjbkmd.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/glxmjeifa.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gqfjtcreh.sHtML

npx vite build
来源：http://wap.fanxiaobao.xyz/Article/details/gchmyneun.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzamlxfaf.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveocpbmq.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gisrsaexk.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdcmbhab.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijbpvday.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/gjcpnksif.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/guybybhda.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gibwspgnf.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gfanpwqco.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/ghonugkfr.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrxtrmnm.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gertlapwk.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gxoqlvccp.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gxbtzsotn.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/ggztvwktl.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxnhkheq.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/gwocvbyrz.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/guixltdct.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gswgroynj.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gsjvxjnfk.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzwgapcl.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gylvgzxsu.sHtML


<!-- 参考信息 -->