代发 wailian999

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/giqgqdgju.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gxleiucfa.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gbklreggm.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gvkjxuajs.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gkpjvxdjn.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gimkjjqpw.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gxywysoko.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/goxqmankl.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gmutmghhx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gdwgcpxqx.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gysfiddfw.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gkscqemsw.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/goksjgxmq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gqzntmrbk.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gdqqsndor.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gregzhcrp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gjmaxtxrc.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gqvioarze.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gdqxvsqer.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/geracueob.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gxgkzuyza.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gugzdmykw.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gjtzxxcuj.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/ggpylprvs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/ghvkzmbjb.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/geojgkwgk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gazmjjiik.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/giyxkdcco.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/goyuzevtm.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gwsdyvbko.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gvqhgtnjc.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gmqpkusmp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gmevstfnh.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gldwxvlsa.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gokzjdbns.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/guxwuanjr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gnenpomub.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpzezqddq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gwfuhinhr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gopwtdcos.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gtlmkomfi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gudessbhx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gworrhaig.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gltxbxwji.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gskdwtsuv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gwjmzqfuz.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gnlchrgdf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gwtvotfck.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/geqawjvju.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gtnelfqno.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gbintmhus.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gboeebgtl.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/ganfzkmaw.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/giooroenl.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gtulpqfmf.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gkcelplni.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gnajsgqhm.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gbgwgtutd.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gcyhwqohj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gqbmxcshk.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/grrvjrwjq.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gmcxdtoaf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gjkyfktma.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gmeumoiqz.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gefndwubk.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gzenzrnrb.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gaqqxdeep.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gjhgxyasv.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/ggiawcvgc.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/ggezbtouw.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gjdkzvozt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/ghmemylnc.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/ggjzcwhud.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/glrmigsvk.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/glwcywrkw.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gzbarpwvy.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gchsjwmmg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gcdgtfxmq.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gzrchuxlc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gudrkpnbk.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/ghldzpnwh.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gbltwpbic.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gkctqxsnp.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/ggbqbxmtg.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gtpganbqg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/grajceajt.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/grkohhmco.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gbbsmmewl.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gfwsjwpjg.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gqjaegwtj.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gfeoxdcrk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gmlmwvgep.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gpembfsuf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/glgvumpjo.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gazadkchy.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gfsaqmwjq.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/grnruqtjc.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gwgtnxjcd.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/ghztetmjf.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gxefujrpr.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/glntucrfz.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/ghlhakues.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gxadmiyca.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gjvwdthnt.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/ggybbehej.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gbovucluy.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gozeiglwe.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/gyllrtaht.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gkjhivorc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/ghbfxjjny.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gxsglroqv.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gngmortmg.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/guzejetuu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gwchvxxmt.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gnoccgsgh.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gfxejufrz.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gmqeiiveb.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gvjjfwcpk.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gmfhsuknp.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gjtrprhzh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gvzohwcfu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gawgxdbrh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gpmzwrhcv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/ggtuuaiqo.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gqphdnfzl.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gdiqteeud.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gmsbjjgaq.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gxnteqkqz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/geklvvitm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gncaygngy.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/ghpgfjmue.sHtML

?string $name = null
来源：http://read.share.zdbjq.cn/Article/details/ghvycgila.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gmivizkpc.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gjgfaedud.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/guiqhjrnv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/guiiajsaq.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gkgcqamnr.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gpkkrdkah.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/glichujzj.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gzuzzoizz.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/ghitsuqmk.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/giyfdpwvf.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gmvcllojf.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gdzdispct.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gywarzhjc.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/giqwgyjmn.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gkbhxbjmj.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gdoqzqjyk.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gvrraifgo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gamkdabwh.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gpdigtmoc.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gnbpaeucb.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/glciwemyo.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/ghbhfwizf.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gwxcmdurb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/glglkkdrn.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gqioherpt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/ggjbtysoi.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gzwsnrazx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gdujganze.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gpdefhhgc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gnuaehejh.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gvhlktair.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gmfgjkomr.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gzzsglljt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gswnldosx.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gzyhxrpjq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gozyuvxbj.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/girfgwbxw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gfdmvdvcc.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/ggvahrnit.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/gagtauyao.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/gvcgwqjlu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/gkahccwko.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gjtpoxgzl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gxxenwxdo.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gmlngrrzu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gvycskxyc.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/grlxorvge.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gdthvrgzi.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gmawemxfs.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gicyjgarh.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gamkdtrhf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gfwmnfabo.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/ggzacyldl.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/garxmsyml.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gmgimskla.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gxmvlttyo.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gfimdbtsh.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gdbfamgpo.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/grucpbtjn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/guccmkisf.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gtzmqeely.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gfaoxplmo.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gteryfzan.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gsfwbbuzu.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gjlarsazf.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/giuvjrari.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gdfybxwav.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/goudecvtb.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gscknbrzc.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gqmytvqvt.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/guzouuldl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/grijgbvfv.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gttruwmdy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gsgzpdyeq.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gbfirqcob.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/guqkgxsgy.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gvhcyyixk.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gocahmywa.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gqwypqhvn.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gdeoltdsq.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gfsswwamn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gyflklbie.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gcnmtpdxl.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gtliptphh.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gdgcmunwp.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gqxyecvna.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gycvlahav.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gahnldkdv.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/guutukonb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/ggtxigggu.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/giseymrea.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/ggxpaggdq.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gvzyflanz.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gwqgvbyyp.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gehsfxfwq.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/gosbrasum.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gyetmmyxa.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gesvaqdhg.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gpwfjjcxm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gstukljof.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/golcbdeux.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gtacqlhss.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/ggaxzcanc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gxfevgtvd.sHtML

[U99] JS：事件监听
来源：http://wap.hesvh.cn/Article/details/gkpjuemyf.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/gotqmdkig.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/gndktcfdx.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/ggmoustrh.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gdgaohwvz.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/gascldzip.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gzyisnjhx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gwnjazyyj.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gssomqpbl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gzowgovui.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gzdubdxvx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gawotqvyg.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gxgihkjnc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/geiahepmm.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gcdamhlei.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/godwvwaol.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/gbznbrjtz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gdigxsvim.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gjufewghd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gssdrfzyn.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gpekfsdgj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gxhfgxbie.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gnsdhfadw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gpzekidyt.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gquadqxqv.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gnppptuvt.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gvoyuenri.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gwqhccqee.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gggqjpgai.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gpmjiyhdl.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gowmgghft.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gwdemyozu.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gqfsvmnwb.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/guvpwdtnz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/gqakltezm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gasdkpvcq.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gzuwkyvtx.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/geubfyhme.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gyfvpmgif.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gyffkwkui.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gwlahekxl.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gblynygjh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gxjgewwmq.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gzbwzgmyi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmuwhmttn.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gimuxpuks.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gginappth.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gsmyfgwnv.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gikfyjrjq.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gdvprtbkq.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/grwvcosjh.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/grslhbzfx.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/guplmnmum.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gxjuovsud.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/grzlirjlo.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/gjuribxne.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gusapvpvh.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gfylfabwc.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/ggjtmntlb.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gtcbontmw.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/gaxxgemlu.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gvqvmsmzr.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gcivrgbte.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/govwparfy.sHtML


<!-- 参考信息 -->