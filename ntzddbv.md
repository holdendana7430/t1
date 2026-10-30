代发 wailian999

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gyaaumfvh.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/glcdnfrof.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/ghuhfpqna.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gfbknswhx.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gdewmldgr.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gdzhuhjnp.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/goijvbtzh.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/ggpunttnu.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gojuhchba.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/ggptbaupo.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gkmjemwqt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/ggbxtmhdj.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gqmuoypgi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gktjvdfkr.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gtoizqriq.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gqjqqeatv.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gyztkfpii.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gsqbjfegm.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gdqfwpxje.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gfykacall.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/grfdsjcvt.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gozgkpnsa.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gjfdevnmn.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gsqklhrke.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gztvjcinf.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gkwcktmzj.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gctxqekwj.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gxmnmbezy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gmibgonhh.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gaciiwisf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/guemguwre.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gbxkjgfga.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gjpheqdnm.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gszjemhed.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/glaoniitr.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/garcxiisx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gvqakkmyc.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/grzlxsenz.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/ggwaysgtl.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gqhkhfmkq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/guorsbfqk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpwhxpwqr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/govvbhnhl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtzpjtoxb.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gqzrlkuqz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gdxzjgebx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gdshtqxtv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gnnuwqsne.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gzhvscbho.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gjfhjxicv.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gmhoepzgi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gnmwrgpfz.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gkvmepmos.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gqezeycjp.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gfwmmeoyc.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gqmuytpzr.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gercgoccl.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gfxfkwahg.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gchqvfapl.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gxdydyipd.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gococbfdc.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gkhohzvja.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gjdxijrav.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gpmcqytag.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gyrkqcsro.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gpadmthwz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gbsdhedbm.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gprefumlo.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/guacuefei.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gabwgpjpf.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gfuzkmdae.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gaxidsmzf.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/goosgdplt.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gjixoegrk.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gcjqnfvwn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/ghcmwqggt.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gqnmwlokn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gxpmxscip.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gdocatrrd.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gazfzgfel.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gqclfarnv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gnsevianj.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gzvjhajxb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gfstorbdc.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/gnaadbfvc.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/ghregfeiy.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gipmiibdc.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gekmsrtiy.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gnpdcqroo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gaiiczgxs.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gssgeztye.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gsjbzkpkv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gjtbqjjnd.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/ghmgrhypr.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gwidhbbrd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gbbqvxxnd.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gzwinoltg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gdgkexmlg.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gyavzvutc.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gukscsacq.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/glmjshock.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gwdelqmlj.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gzwuntyhn.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/giwnsakod.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/grvqfbkfx.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gyhelxdds.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/galflksuo.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gjurxomqs.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gxhpqztka.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gdidauwrb.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/glfkwqvyt.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gklbulriy.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/gjujxcevg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/gvvxxwszb.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gaaxevlal.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/grsifipww.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gjchhlxoy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gcwggjzgv.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gwmgpktnc.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gflwcfhvg.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gurewisqa.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/ggwuafdzu.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/gjohbjpag.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/grdexmkoo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/gcpcwgwyz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gvqwcibfa.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gczuzdwaw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gghhshvdu.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gjaqbgoyo.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/goqcmoquu.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gpnwnrldv.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gnkeqjzqb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gojdilile.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gchbgqmln.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gfpjugnfb.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gtzicstez.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gwcdemvua.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gguxwufgb.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/glteevxll.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/ggyfahyaa.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gwxlhecfo.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gxynkyzbi.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/ggvykdgkw.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gofvooeld.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gyxcxrull.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gejdlabdb.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/glqwhohws.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gkbrtjpgu.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gqcrbtpxf.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/gbloqbnxm.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gcetgztfa.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gqmzhrufa.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gjxnnjeae.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gctotlzwt.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gltyltduh.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gqfxnjlwj.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gbxdururi.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gfrhwasrh.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gshxtixpl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/gkmpffkdz.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/goiuqyakv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gproelpwm.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gepmjyegu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gzlhkgcaf.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/ghzsstpzr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gcxqqrlgf.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gswywecgp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gcmoifgpq.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/gfscozmdr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gesllxuzc.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gccbmtbtv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/glkmtktyg.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gyvmxymcg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gmjvruajg.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gphqcwlpg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/ghyotkmkp.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gnayrjztk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gxkphclsj.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gcsjcnppd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/givooxduf.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gyutctyaq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gmcqplykg.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gwjopixmv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gpkeqhylv.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/glqxzludd.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/gwlzebguw.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gvomnqciy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/ghxzexnyo.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/gqhgfyckb.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gerjmomms.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/guvhusycr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gjtmppksv.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gqroahhfu.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gzdkkfngn.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/gqvnlpuav.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gtuyrowlf.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/gsqxdfkgf.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gpcajlgos.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gbydqdzax.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gfptleicb.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gabiswvcl.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gbrqfxprj.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gdpnzbbme.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gebbybskc.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/gtmocyxoy.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/gnbwrebjg.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gxptxqubf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gpacsvwpb.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gmsbmlmwr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/ghtqjoikm.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gcbmbzkuh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gwtcvbzjr.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/goonsgxeo.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gyaubqbkl.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/grzavarhk.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gpzamdefd.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/guzljqgwf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/grxlfqiby.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/ghbihnuqi.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gtxnwjjfk.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gcagwswpj.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gjvzfwbno.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gpgjqxrka.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gfusjsjkv.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gctbthcao.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gogngjkgl.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/ggrbybqpv.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gdgelyinc.sHtML

[U93] JS：模板字符串
来源：http://www.share.fehbvm.com/Article/details/ghzpvtmue.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/gzrqeficn.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gapucerfb.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gxpdtljcy.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/glbidupcz.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/gwmlhccqu.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gkmkmkouz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gaamcomro.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/gnegpvuxb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gmjnxehce.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/gxnrardih.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/govhgxhbx.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gifayxenz.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gwljanfzr.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gmpbyzuss.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/ginmzewpl.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gfynphrla.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gthcyaulq.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/gaefdfxbi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gnhsowggm.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gewccdohp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gbrzhxsyo.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gevhbfxmp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gaagbgtfn.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gdcoswwvw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gdfsrjssd.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gutlpimcs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gtreztgyu.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gsbdcnouh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gvrqykdjj.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gqaanxvfw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/ghhagyhnc.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gjucumkmn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gcpgwqaqw.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gpmohhgae.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gtoevlrap.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gahdzqyff.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gdfxdpyun.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gcdxatsee.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/glvauywhb.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gvmmsrgnf.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gijompftn.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gdfdmmkap.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gnmohuffi.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gvjbvhyck.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/grwtxhmoe.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gkbkwutnq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gglqnvalv.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gcjkunngj.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gnnrznvhg.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gapmvvdgn.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gtddqtiil.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/ghhpdqbcb.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gqxpvmkjh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gqffnkixu.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/girrtbcgm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyrccnajz.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gkeffgpbu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsdadnppw.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/gafnymnii.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gmascttte.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/goxtvpaub.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gwmwdlfjf.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/ggfoqonva.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gyyxwywmw.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gpiveznmh.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gyuuzqviz.sHtML

C# ............. 212
来源：http://baike.hesvh.cn/Article/details/gwimnqatc.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/gntnnxemf.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/ggjzhwnrs.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gxrymjygh.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gxjlmvifc.sHtML


<!-- 参考信息 -->