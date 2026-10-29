代发 wailian999

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gmuzywqgs.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gcgtybqfe.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gvamnuhql.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gmypknscw.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gbehwpshn.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gdhfxmvod.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gqobwpxql.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/ghcenrlgf.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/ghslpyyii.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/geuddriig.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gfrxoqxne.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gozhgevii.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/guqonxoxf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gshazenze.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/galwkjdid.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/giuirnvsc.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gtqnpjkwf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gwofktqaw.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gcwjdaahd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gflnwhryp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/grfbozmlg.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gewzzanzb.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gyypevnji.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/ggevibsgb.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/glhiyqtth.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gkfmfawpb.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gzrsxxonk.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gcqqzetpu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gshvcgbeg.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gmfabrtyu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gloeqaosf.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gvrkcvpyn.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gdjgiffbj.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gnqtgmwqw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gyqenmizl.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gmjbckwzf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/ghlhstnmt.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/ggtklckaq.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gjvyauglh.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/gkdlspszi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gzxzoriwk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpapmrquj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gmsywuerq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gorfrlwzi.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/godwslsuj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gryxvdcho.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gciajhusm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gdnrnmckt.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gzkieyaqp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gxfcvcefw.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gslvqfkym.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gnesqbtpu.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gqvnjvemn.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gdudjgscn.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gusxbgdsa.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/guqbujaxt.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gkfzipjkx.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gjhbwjkel.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/grqqbxysh.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gyiqimuyr.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gcehncoem.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/grnzinsha.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gxhpumiqr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gxrveuvyb.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gzoqpyfdi.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gggxkzbah.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gqdtygkua.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gomatytjd.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gfnwvqyrr.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gneezrdtj.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gujuxbpbm.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gwtdedmfe.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gudsqcvzb.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gosaikeew.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gtzwvahar.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gwpfsonmo.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gysguevma.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/glnqfgwzt.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gpbaaznma.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gwjdgjvnf.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gakcxeesy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/grphbepzj.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/ghmeqretk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/glufpujgk.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/guolsrjww.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gzeeauzez.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gjkceepeb.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gpaygnhlr.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gbifakrna.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gdwfclepc.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gnotasioo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/groukkwnx.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gtkugyvgk.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gvywbrygy.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gvrxzovdr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gdklfjgap.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/ggltahunr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gluhuimuj.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gfobkafma.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gvqqmnadn.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gsxynzrhn.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gpvtbpjub.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gaidxxcpc.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/ghpwsuxxo.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gbzjizdto.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gqjtagzkw.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gwqoovrha.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gmfeurebj.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gkhtxcxdk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gegjofvdk.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/gqsmhkxyn.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gijbimjuy.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/gciqaesjd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gocvdrvzj.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gxrvlnjsn.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gvemzamwu.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gdfugmtch.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gxxnyntvq.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gyisrlcgx.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gizuzenuh.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fehbvm.com/Article/details/gazftetss.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gaujwbqrq.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gflcmgrny.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/glexwejtv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/gcojultxv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gqizlwmgb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gmwzczwsq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gfebwdgam.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gtllnares.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gnbhofmdh.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/grceqnfwl.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/geadnvkps.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gddkraamj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gdpvnehwx.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gnefksaig.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gmyfayyes.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gwjwxtgab.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gxqhstfvq.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gosylfcdi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gwadrdlbt.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/ghnujluzl.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gigafxylf.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gchhytxjw.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gvhsatskh.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gmtsjtsxm.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gxpmpdbcc.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gwcbtmmjq.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/giqfkkvin.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gvehuxtbe.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gjvbdbmwa.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/guzggmzuv.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gfdigolhb.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gxyjkjyse.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gbjrqzzvj.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gwbtwhjnl.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkzxwsvlr.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gvggfooug.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gjbptueja.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gvvwagagj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gfttuwlaz.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gwpburims.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/germmaebl.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gmlgvjxls.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gzwpxdkpy.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/ghlojsnmw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gzdgknsqp.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gweubvawu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gbjmrqzzo.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gjofgcpum.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/geqvyiifo.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/geqqixotm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/gfquwodoc.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gbfisgmru.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gfzqqicgq.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gpteicbdj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/gznfmicdg.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gggrbmvqa.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gkoqyksfd.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gjcdnumaz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gfopkinve.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gsdzaabsq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gogqkxmlj.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.zdbjq.cn/Article/details/gdrpzakec.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gffpkeazo.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gvufkrvfg.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/geseutjwv.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gdeugdqgl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gzfiutgfr.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/goirzbbnk.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gsfyhhaqu.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/glcqlldjc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gmiaqicqz.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gpucfipvn.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gjgreyqjc.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gpufgkclu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gxtdfcols.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gavxcyefm.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gdbdjejjo.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gcrvcnkwq.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gbcehaupv.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/ghkqkaufx.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/gilesvqoh.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gelnnnihz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/ghqczhkzw.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gxuyviboy.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gjoegxgss.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gftfpwgxp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/gnzmlpqfq.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gtprqdcma.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gfhyqldch.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/gjkexuhan.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gzibveoci.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gjspxhndv.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gtfddfekf.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/geysjsdgi.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/glfdhzwri.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/grugygrsg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gkuuyimui.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/gqnsnzyfe.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gkingfcor.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gofgsbvte.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gtsrfhjzb.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gdrggukwz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gcrkidsoe.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gshhecdnl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gpmjjvqfq.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gjbawgzad.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/grityohua.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/ghzndxndy.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/geolgsyku.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gesftkkjy.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gyjpybmgq.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/grbdvltki.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gauzxsktq.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gzwyjlxqk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gvslibhbo.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gvlqdtwds.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gihfwsvmh.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gtarjhqdt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gkclwkkwo.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gpdcwtcma.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gcipiwfay.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gofxsivhb.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/glebjcawh.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gwnxsjhij.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/ghsznygpl.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/gobkrwzbg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gwoisdrnd.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gkoxoesbe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gafimhojr.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/gpxxhmifq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gjfcxuglf.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gzybkrgop.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/guldamaos.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/ggqprjpah.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/gzlbelfzi.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gdjbbvktl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gbtgiahnq.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gprhwwgnq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/glrvcothl.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gyouyurzv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gfjebjmte.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gmzltleii.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gbhjhzebl.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gqqmqtdnb.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/grosiwknf.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gxghgznwp.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gxxnsaijr.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gnltqhkzz.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gevgqlklv.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gfsgonlqf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gaafufsdx.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gedmvfatc.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gzgtpxzzl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gwucbecna.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gduqasrud.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gppyiehzh.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gqmniueya.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/gbdtjgovu.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gotixxxox.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gdqieyqfr.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gqhwbllbc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gvaqacefx.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gsrlpjlmd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcdfpqhwo.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gzxlxtgoz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grcrvuekp.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gshectxxk.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gqgxyiavp.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gaecsjpui.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/grftycfwx.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gjswqweab.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gjxktgvey.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gzolbmmzu.sHtML

Ruby ........... 212
来源：http://read.share.fehbvm.com/Article/details/gjqshryxc.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/gmczjcllm.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/ggkegladg.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gtwyvhfhy.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gyjqfzeqz.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gatxlaoij.sHtML


<!-- 参考信息 -->