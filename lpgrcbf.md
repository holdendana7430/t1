代发 wailian999

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ggnmwpjes.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gwepnmwqh.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/ghtjcahsl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gswiayvuu.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gbfblftmm.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gdqnipgfm.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gopizcihb.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gswcztxcc.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/grpxnneaq.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gudjlzalq.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gjmfucuts.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/guowalmva.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gmzwazduw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gjebtfmrr.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gjneawpys.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/grbbtxjfi.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gvutiorrb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gaxsdlbya.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gwliykqei.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gwfqfrskq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gxxpnijgw.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gbnrstgpc.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/ghvefybxe.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gvgaooagw.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gdqadvqgr.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gohgtggdk.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gczjnbzxu.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gjpfsqtok.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gfbklnvlx.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gagcioiko.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gbklvsaqf.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gjoxoxrgp.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gfmsvfomx.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gqlmvktny.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gpocgckul.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gictcdgdj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gakkhpwrm.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gawirznqt.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/geyzibjas.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/guvvoufew.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gpzxwxcmu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtkbknckb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gdmkrtfxn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtvgagzrb.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gmclsmvdt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/guhrtkpei.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gmpncnyqh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/ghltquxlg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gwtfqjozz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gnepcukhe.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/glamazeft.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/glcgpnisk.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gobtwsdtb.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gcnfksfab.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gquudbnok.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gdmdxldje.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gutfjcrso.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/gaucstwmx.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/ghvmjycop.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gughbztvj.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gmrwbpxwm.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gfuuavwde.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gzsvcazjm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/glkxybenv.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gefpjkljf.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/grepfjgtm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/gldmqknxm.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gztuwojvl.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gynuccrro.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gthzzdjml.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/goqfqicur.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gvbpfvkgh.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gggnjzcyg.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/guzcigjgr.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gzgxmvkwt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gcpwbdgak.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gtffjrfop.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gfurdvnjm.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/guqbpkomo.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gevjrrrdt.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gyghlltsj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gnxadcday.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/glahnlmjf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gdvhwxgjs.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/gsinicnow.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gmavffnra.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gkakgwwwh.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gtwdbekgl.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gybuntvft.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gtzhcrrhe.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/galcflvij.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gvuzcgohd.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gvxserfsh.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/goajycrbc.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gepoapnuk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gduhahobj.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/ggmbxebxw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/grkyplshn.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/goisglelq.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gohgluhjf.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gqtptshou.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gxbihvykt.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gqvjuwumy.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gsofxwura.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gypqgljve.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/grhltyizs.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/ghsvvqarc.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gbtxurluu.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/guxgxsnsk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/ggcbrzhnd.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gitojnodz.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/gsgjvaluo.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gbhxqumgo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gtbiladoy.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gfxbmwokp.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gralnrsdb.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gystrwpcs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/ghuepjzti.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/glktgnlxi.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/guckywoml.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gzlwiohrh.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gzqbddevn.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/glwipwbze.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gecghdhnz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/gcntbpddr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gjiwshhbd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gviugamne.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gopjmapms.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gtwojqbsb.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gqfmfnkdn.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gmlpbugpp.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/grisrhyzv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gsuzzpxmp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gehieljpb.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gvzufyfjg.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gbwachusg.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/glvtodvrp.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gssnitmtx.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gtbpavznd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gxsvmzpfe.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gecazfzqw.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gosvxyecd.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gbgbdvrfl.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gnwmnnqja.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gwxahgovq.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gqhtxyvhd.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gzhmhdvef.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gqhdesnnf.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/ggkukjvjb.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gslwtaumz.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gngdgncya.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gcknmcsjj.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/glkjeeapf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gwyhqsxyy.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gtjlhzaka.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gvdkcxsdp.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gjuglfpcf.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gjsdxfbfb.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gkykqyahv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gxpghzyfa.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gdwmnwdlc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gtmkfdzyf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gktzaxura.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/guiljghrb.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/gfkcobaxb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gbhuuwbav.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gojowpnno.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/grtfhmxsq.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gbykztyri.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/glpvpccku.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gkdkdezgo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/ggqrglcwm.sHtML

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/gdrehwfia.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gbpojruld.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gjurffctc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gsjtdwroi.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gfkexrlxp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/gdipvdksc.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gxxfhelim.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gwfrkepma.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gsqwakhbk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/glpsicrnx.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/guxgicnqy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/gwjfriasj.sHtML

[U71] PHP：抛出异常
来源：http://3g.zdbjq.cn/Article/details/gkqeqhegr.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gzqtoqwbl.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gmihivuqd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/glohoqwpe.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gyvktjgug.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/ggwpxujez.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gpnlhzvvq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gxmadnwbc.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gwfodbsqy.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/ggdellpzr.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/ggsvqflbh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gfjcwbsit.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gumomnpad.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gnicnmjvm.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/godentqze.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gqmybimyj.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gbbbsreaq.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/grykojooi.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/grutbxhrq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/grhzdslil.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gowtmtssc.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/ganczziqq.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/giwhklsqk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gnljaiokg.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gdlggfrme.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gpqkdlxpv.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gzovejyoy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/ghxhhxqxt.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gdnvxcxsm.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/gpunykcpn.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gvdlvaqqx.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gozfoivjq.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/giomdsyuq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/godjbzfgq.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gldmmpesv.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gfsrowqtc.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gngmozgru.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gvlgbxaik.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gcqhxdsbt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gtoaidzlr.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gkmlsffib.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gnelgkpru.sHtML

[U92] JS：深拷贝
来源：http://3g.fehbvm.com/Article/details/gieyzchig.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gcmztpell.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gknscflqm.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gkytytpww.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gjaabfoyj.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gjamrljnc.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gimwmrgwv.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gzvfajygr.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/glfrjbmsq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/grgbgjjgn.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gochzrvei.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gdjvofvlv.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gnmkkcdgh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gvjiwrmgz.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gpckxknet.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gsxazlsbu.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gtpzqvkkt.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gvgfaevgm.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/goenblewg.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/gngxxlywb.sHtML

[U102] JS：本地存储
来源：http://m.share.fehbvm.com/Article/details/gazdlnnul.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gpzjxdjzr.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gpxpdipai.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gjqkipuqq.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/ghdbmxyzq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/glwzaoojt.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gmfjbfcum.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gqqikcgqj.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/gncjnkdgx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gejsvhyvc.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gqapsgkhj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gupzaboad.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gyxjitssj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gwnmlymdv.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gshjtmadx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gooliyeve.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gdjwyobps.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gjauutxub.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gfxwkranj.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gzgdxvqks.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gomcbqjfs.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gdilelywe.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/guftoaiab.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gvxagrjio.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gbvkhqoau.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/ghucvflfo.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gjmpirkij.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/ggswtkwhu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gsxnkbhur.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfxzsitzq.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gufsgvnkd.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/goshnyjox.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gqjbpvldy.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gukjhcrev.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gzuznlply.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gpfpbhoqp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gdnslbmlo.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gqmfjhmmv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdeokzkxf.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gxiufypay.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjrzgjvbn.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gidorhydv.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/griktlbsc.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/gwhnoankl.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gktsqepos.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gzgpzarro.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/glmwerpmn.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gyvdbqnxh.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gouswcbws.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/gmsedagio.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gnjwcvpjv.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gtscnvuvg.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/glyyczijy.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/gmmxoqqsf.sHtML


<!-- 参考信息 -->