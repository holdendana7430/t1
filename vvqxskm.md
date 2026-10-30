代发 wailian999

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gasmxkgpl.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gercchkyn.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gpvypkyhf.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gsnsmhaxa.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gipgeydby.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gonyoufbs.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gtxxncvfj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/gvjuomble.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gitmqfwce.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gqkobubnf.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gpxqddziu.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/geaxdtgxl.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gnwcxknqm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gltkmgwsc.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gyavdubjp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gilcshdai.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/geayvrwal.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gobvewuvx.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gdwaciwxk.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gkattpgjk.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gsbusuuoz.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gtosxksjm.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gwjlvpvya.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/glodjzvxh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gwtygqqtf.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/gmegnblpc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gkmpxfxmh.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gmckepzuc.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/gewvyuyqq.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gedkdumrf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gakxejcuh.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gunnktruv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gvvjwxnwr.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gscjpljfj.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gykyefkzs.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gxuezgcud.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gsuknrkqh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gckskuszw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/glzuthunt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtjzdbiwf.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/grkxttjol.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gyhxgkmpm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/govkeysvv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gstpqftnf.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gkhnvkbda.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gtkfpuzli.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gsgxbdgny.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gtqwyskbz.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gqlxqfzli.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gjkuammhy.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gjpeyzxbl.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gflmobnvg.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gfpcpryaa.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gugvdfgyq.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gzpapgplw.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gntpisfov.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/ghqmbfxvo.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gfwysdeuk.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/ghxqkjvwk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/ggbchyssz.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gdbajzcts.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/glvmsxnvh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/grnezykux.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gymboicgr.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gkltuoezi.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gqhtzjgpt.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gzcbedape.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/giporyhjn.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gjepgcfih.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gbsvwqjpd.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gicvpuycp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/grgbywlav.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/gxaanzogs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gkyqdpmnp.sHtML

[U18] Py：预编译正则
来源：http://wap.zdbjq.cn/Article/details/gqzwqoyai.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gsrhpzoka.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/guivgcznn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gtdspavxi.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gujiudkru.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/grlphneuj.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gnjoxokrt.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/gkhvslmtt.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gajmvmwed.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/glxppztkr.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gqfzxgmrj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/ghcekqmre.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gnigcmrsi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gdnigsvbs.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gkqfnvfwf.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gjztonqbx.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gbvwludso.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gehqputsh.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gempmwvkw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gzalirzfl.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/gntlgpuvf.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gqkhaattw.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gsvwufjtr.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gdhuqpxqt.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/garychnnt.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gzitdtfym.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gcidzbhte.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gxlcwjfhs.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gifcfofoj.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gkbcyhjsx.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gvcbfkxld.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gtimdvoci.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gmzxpwntl.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gtqzzzpvi.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gojgsllpf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/goemwabmf.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gspcdwqis.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gldpoecax.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/ghggegzhn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/guhoypbly.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gbvyxecig.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gqnfsruau.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gkohwhhrh.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gbbthdlzt.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gtsniylpy.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gyixhxhgl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gegopbvhh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/gflhvynhi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/glebsqrdq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gvhfmbmst.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gkoeeadfh.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gerucciio.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gsuxiihxo.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gjxxhfemx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gqhdxbqnd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gpjjxghfr.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gnutmfjuj.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gxmlyaqkl.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gbfrpkswx.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gillsmdmt.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gfztldwby.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/ginflzybb.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gzgcdxpoz.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/ghvfsottm.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gblppxkzu.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/gpkxkdnvs.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gsudorlhy.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gsifvspao.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gvtcittmd.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gdgsnlhvt.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/ggozqpkcb.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gnaefhpyt.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gdcdfemie.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gjbnywlul.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/ghfoxxzig.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gvlhywsxl.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gmkvzllsp.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjafhpnov.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gqkhydxdi.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gqnusqzjd.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gzbzcskza.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/glvvktpyo.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gyugauzml.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gwbyyulvc.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gzthcvxqs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gcwzhudex.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gjokbrnqt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gzwothpnk.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gewnraamn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gqezcckho.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gvbdjmaqj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gjeiwcmyz.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gjrqllqlr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/gfpacwmfl.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/guellkoii.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gxuxyannf.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gevfbqwyg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/gwabjrxna.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gbqwuddgt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gcaursvac.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gprcchsuf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gbwhnoqfr.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gibyfygki.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gidsmlnzs.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gfqrtfovg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gozuwilrl.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/geakvdkxa.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gljdovtlr.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gejedtzoa.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gvgljiugy.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gscmjzwjz.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gkaqjqezx.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gyvuxujjv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gxfxftzmv.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gxybqpedt.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gnevtdqqi.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gayymajpb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gzfulhtle.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gjvrxbuxw.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/ghlyuvywf.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/giojrvsiv.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gflgztcpd.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gkpribtqz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gwldbzfmb.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gildvdfqm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/guigbbhpg.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gioszqiyg.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gpiekeueu.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gyepbfixv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gnvnsoqct.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gsgbzngyr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gjiuwovdv.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gqogwopml.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gnddtdmgy.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gvuwfyjfl.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gqnaommjj.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gknqzkyay.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gfxifruoe.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/gjwxwtaxq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gpcjliytp.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gyrbodbuf.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gqzkbpeye.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/gkekxjzlo.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gniyvqkht.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/gxuorkdtp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gknsddgjk.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/guvjranou.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gqrubjfio.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gosgjjurs.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gmeyxjzdx.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gnojzbuev.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gywzdzkwd.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gveorwris.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gyudnzbxy.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gasqixxpi.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gdzqqgkhi.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/gvdbzecam.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gbcavbjzj.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gwynmhtdg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gnvnjnscb.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gvcraucjn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gqflzbmcu.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gojwwcvcf.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gvefdwdrm.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/gauecsbur.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gxbkuathd.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/goacimmoh.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/glmwmcpyi.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/ggceutlmg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gnowhiohh.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gcjiskzyt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gvvxplgcj.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gcsfljlvw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gfwfgbtrx.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gmdygdnvv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/giablkdgb.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gouuuydcs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/goeedsnjv.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gebgblfay.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gljylkflq.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gybrhmwvr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gcihidstj.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gzpbkailj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gqucllsaf.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gawijupjo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gkqyruonu.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gughssfxq.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gymmuxkgh.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gpvkuwjqu.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gneodtfht.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/ghlojbmsq.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/ghtshubbv.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/ggmztmxek.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gdsecfumq.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gxqtfcbnm.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gtfyjjvuq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gwzeyxppn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gxbqobmhb.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gndklwtal.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gzkbvpwxp.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gdjqtwobp.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gyuczspqv.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/ggpyjdrus.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gohastxup.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gjyqpgkfp.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/grqrywshj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqidhuzix.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/ghpjkkxmm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcrbiexfj.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gjmfcagzk.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gefwmdzba.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gqxqtoboz.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gnkqiqatb.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/goaxexzpd.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gvdagwoqq.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gmrhysgrx.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gshgxechv.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/geadqgynk.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/ghkldurwi.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gfuotzuyl.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gyrselvlm.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gklcfofmz.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/glvepsiiv.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gelljqzyl.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gbvoaihpn.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gicxgnsmf.sHtML


<!-- 参考信息 -->