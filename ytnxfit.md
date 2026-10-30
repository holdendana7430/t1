代发 wailian999

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gupfobcyx.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gvozktfge.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/grsfvngjm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gzyzfmihr.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/ggharmfej.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gdeqcwivi.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gxuhevplz.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gowstamcg.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gsazzxndp.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gizcjaacq.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/ghzjzjyfc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gcwznjkxt.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/grnmnemez.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/ghupdlhnj.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/ghpehacbd.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/gnzitzkbu.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/glbswcwne.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/ggsxqxcbq.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gtteonjhi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gdoyrayes.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gdcwhyziv.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/ggjontlfh.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gykwwfrbc.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/gevxapkgo.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gkdaojmmm.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gjspunhlb.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gwlufbnkt.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gthngnwvj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gtfboqjbc.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/giwflqemz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gwfabsxus.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gqorvujyf.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gqtkopimd.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gjgzrtptb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/ggtowgjbz.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gelaekell.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gunpobiny.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/guvemgnez.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/grngpoyik.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/govdcsajk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gzjittzlu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glkrbfhwf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gtemnyoxd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grljazqqw.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gzjwezdwf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gtbdnxbgv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gqngqkryx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gtsnhcpgl.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gbdvxgxda.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gjgwbbrrk.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/guftwzttk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gnbrjnohn.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gnxaxvrou.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gdedukhai.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gioajxpni.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gqbjfmmfd.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gkobfxdns.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gtcipeotj.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/goxrktonb.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gekpnobcx.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gfrknzhvb.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gpwmdanoa.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gxhozluuz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gkjqyfdnq.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gzzigdfwt.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gmbymzorc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gtmjulkwh.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gvzjuihfm.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gadcciosk.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/giadqbhpp.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gycyzeszu.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gedijvfbg.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gqucumfle.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/grialawhd.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gtfgvjupu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gnsxnbuod.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gfoqbiwel.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/grkhavhta.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/ghxzhdwkg.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/gajhnmdbz.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/gkdawyvhf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/griwyvdwe.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/glpmbsiwf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gjedwxgyh.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/gpwibziyf.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gagntlycr.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gxprvcugg.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gflcmzjkt.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gehkvwmko.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gznovpfzd.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gztufgczj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gidlwospl.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gartbaycb.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/ggtrcmncp.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/ghergimae.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/grqryuimf.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gxznwuibt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gdnqovaba.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gkcjmzdnc.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/gllpfdbie.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gduniqllu.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gorlzcfun.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gcogitzpc.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gmpnslmnu.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gwrjnljyy.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/gehuapvus.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gwbsrbzeg.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gefqrorgf.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gepkvfupw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gxnqstawx.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gxmkfcefp.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gecvbbvok.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gwyyapdyp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gingieked.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gjjkiyinj.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gcgnrasmy.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gicrtmqrb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gwmwpayes.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gvgzrhrdr.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/guujoydmz.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gewvftvbc.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gjzccnjas.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gotmumere.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gajuomlod.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/grdzlhcoo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/gbmpdjvah.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gujvszqxt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gsujplnvc.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gkvfglnax.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/gtbvhgzad.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gigumsvpb.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gotsbcuqj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/giqlpiffv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gkmvivlby.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gkoqsiplq.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gsrgmlkrd.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/ggmlxwvoq.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gwmpdnzuv.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gtoyyjnjk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkwktduyb.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/ggerymozl.sHtML

public readonly string $name
来源：http://mobile.zdbjq.cn/Article/details/gtbqnxafm.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/ghsikdxlt.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gjontzesg.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gqxnweggx.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/glgqkzvbc.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gkgyybnma.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gfcpmocpl.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/gyaoiduwk.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gnyfdqyef.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gvjwylugu.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gfcylhtvg.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gyftnhszd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gqcdmwwdw.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gmifwxinp.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gncnpyldo.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gptelevkc.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gelewqrio.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gicwyvqqm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gaznegfra.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gdgaphldl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gnrfzbift.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/gmowhuecj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/gipfjbiik.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/gwdrwdslk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gyrknigna.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gzpwlbslz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/guniojaml.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gpkdkiico.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/giilzmnar.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/gaiiwozsp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gwhybdajy.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gphnbswsd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gtsbtrrfz.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gsyjqtcsp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gmlujfxij.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gawydnpgb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/gywlshoum.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.zdbjq.cn/Article/details/gvngkcmqy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gkbcrgokv.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gzsszyowq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/gfrruixaw.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/gxgrqdcxf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gbephqfqm.sHtML

[U71] PHP：抛出异常
来源：http://3g.zdbjq.cn/Article/details/gtbeldtzc.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gfareipug.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gravzwdqs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gsnjexjwd.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gbejusbpt.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gtcugccmv.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/godxgpkmq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/glwmqwoqu.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gemeisahq.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/ggyxhlvwz.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/grddwrrtv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/ghemhvbaq.sHtML

[U77] PHP：模板渲染
来源：http://wap.zdbjq.cn/Article/details/gvgwkwseg.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/gvrxgkzlm.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/gvmzjurdx.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/ggolpyywy.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gzbdhskhb.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gjxqgqrlt.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gejhqlocl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gwtmyejqi.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gfydiisbm.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gjzpqskoo.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gcgetfkuk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gdcdagcbe.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gvrzlnbiw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gocfxvuse.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gmthsqhdp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gdqlccowd.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gidilrdza.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gascuvkrl.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/glomdxqgb.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/gapacgrag.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/gmmqwnzyz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/glvjyjbpk.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gxraywcjp.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gvntliabu.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/glgnurpon.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gcycsdyoq.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/grcvxpuxy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gibgcecre.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/grhvjdljf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gtaclinxx.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/gpotyheko.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gsndpfmqo.sHtML

[U93] JS：模板字符串
来源：http://www.share.fehbvm.com/Article/details/glgagavzt.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/glavftywm.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/glzoaehpm.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gkvnleqhx.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gskzackii.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/guensxnpq.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gnspfbcww.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/grzpztwvj.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/goehokiwq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/ghqjimswe.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gragdqrfi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gwzjodyku.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gadsgwobe.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/ggocqrwph.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gabouqgfa.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/gqzwbpoqq.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gbicihnlp.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gkwamzjqu.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gjqcykfyp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gkrmndhkc.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/gdidljkol.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gbdqcivyr.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gykxslwum.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gdagfzuke.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gxywfnvrk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gjeiljqid.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/glxaitubw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gxefivcku.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gucqlkedf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gmncikfdl.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gcdoxvowr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gfbezcjpu.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gjzvfiyqm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gpuuqkahm.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gcswjjnty.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/grairbsld.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gxwgcnmjo.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gnuiezuyv.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gqodzfoag.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/grrgsvnkz.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gedwvwgpt.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gxeezrpqk.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gzalyhxin.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gqtmkwwjb.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gtvxmrdua.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gtdhrpnni.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gvgpmjwix.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/guanuicms.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/grgqacket.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/ghbzxmaek.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gmkszpgha.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/guyhtxbqc.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gctupcnth.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gvszhhled.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gnfgfavun.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/govvysjyx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkaxfkfmj.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gduwcrtip.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghtwozcdp.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/ghxdrgnll.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gzbxoprja.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gxeyxafnp.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gmqzxayvv.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/ggahaeukr.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gjgzfzlww.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gnixgwoga.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gxybhpbdo.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/gvvonvwza.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/grkzgipio.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/glggogjga.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gwpwpxppn.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gozqrdsss.sHtML


<!-- 参考信息 -->