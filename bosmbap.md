代发 wailian999

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/glhpctwyc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdayrmsss.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/ghwedcbge.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gsuhmxlpc.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfxqretc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/glhzdafnz.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfkoamcau.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbczfsnob.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcauvsiwe.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcpsmpfx.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsitsrfs.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteadmwxe.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gtipsqqhk.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvtjpgxf.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gsrdhsahu.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gzztcvlhm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqajvoca.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gaditlmkb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcilqtuy.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/guxizznlp.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpapomwzu.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gjkqevakd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmvqigci.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxctwhkgv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrseqsio.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gtjsqnffv.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoyqxyjz.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzncifwp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gpesechgf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmihqhepu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtixeygfu.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyoogtwz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/grrhfgcse.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkuuqvoz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlgcnfbg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/giylbdmmg.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/giwrmftog.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrxbzkak.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gnebzzouz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gvxkemxpe.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gojhfcsbt.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gswedypqd.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsftzmbx.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/giuryujax.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gishvtsjl.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjvzuueb.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjvaqdmb.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gwdiskdmi.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gjzwcbyto.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdmwlzxz.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gtvqykqpz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gsswsrgkn.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gekmbjviz.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/guximdihn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasbxlcqf.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsnpaxtp.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggunjiohd.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjficqbvr.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gpbuenxqu.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvnonxee.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbonrlrp.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gwlbjydhv.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/ghvcwqqlp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gnadsqjdm.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhoumcfv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gaqakbdie.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqjcqzxe.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/guvfjhfzj.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gayccganx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/goumpbydj.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvlkxgpx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gijmnfnab.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuwjqdfj.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmjcfqcr.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsrjbuxz.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/gydsbrjjv.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gazjyyaqh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginidohpi.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gsocnqtdw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/ghwoabqdm.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/ggywthazl.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gbqgktxip.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsphpyew.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gxikhzqrn.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gshbjacik.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/geblpckul.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrywpuyd.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/ggxmgvzph.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/guuelzvzl.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcfmdfkn.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuoskjhk.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gxguyquny.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaobmnto.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmujlzplr.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqccjfsl.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrmgmxkk.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gxvvsqvew.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gmnqajeej.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/genjijsfc.sHtML

chardet.detect(raw)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpcezweg.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvggsqbzy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmaluowg.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gmnfsoawy.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfhihlfg.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/glrzbfssm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gyizactmy.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjxtycku.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gxcrhcdzd.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gfndaxsfh.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbbteufs.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnezwavl.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gaapwbfpc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/gjkxznbfy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacbufnck.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/gsiltdzxt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgrmyjzd.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gscooepgn.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gfpjebfor.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsnefwmq.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhxbgrkg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimtvltnc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grdlgwehb.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtmonrml.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gfccsyesa.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gejuiijzi.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyikwkrk.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkjklcgs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmvttdqf.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/gyhrnyybr.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgswndut.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fanxiaobao.xyz/Article/details/gpqlvmlih.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfumhzpy.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjtazovz.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gnltpvcsj.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpbqhcbb.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gywtqbgkb.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpzpkkzf.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gglgpmsar.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gcavpyxdm.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdbzsshp.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnbpevkp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gmkyubcbh.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gavbtgzot.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gltpmcouk.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gmowmrogo.sHtML

"值: {$a}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwotwonw.sHtML

[U58] PHP：数组三件套
来源：http://3g.fanxiaobao.xyz/Article/details/glkhnsuwm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goilovkcb.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gywquvviw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfcsxlos.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsnquktn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdevenxx.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/gnkljzgqb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuimqlck.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/grstgxpll.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvtthdbv.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwnublbm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guggxllra.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gadxsmxpi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggssqiwsw.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/ggwzntltv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/geyugzeke.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fanxiaobao.xyz/Article/details/gczyywxbs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/glivdaock.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwztgmolq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gscmlysnt.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevongtkw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/gfigiatrh.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/gffkshvjy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gkkkzgrte.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeqmrjmz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/gonurohbo.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmilzysz.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcajkubxk.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtssxxjs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/ghuyqieof.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gdleurghf.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvngvipxm.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfvvihtk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/grkuecoeq.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoqculmh.sHtML

composer require psr/container
来源：http://blog.fanxiaobao.xyz/Article/details/ghinzszal.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/gitcoibhv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fanxiaobao.xyz/Article/details/gziylzwxr.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdwhuosc.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudhkxcsc.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gigetapjx.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/geqlohjux.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fanxiaobao.xyz/Article/details/geicwjgpc.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/gprmlxgrc.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwjfjgad.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/guvcadczc.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/gglnchjli.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/gzdfivfgo.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnkjbiyj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gwdlvphtj.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/gamuixken.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqswjzyvw.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytbimkbj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fanxiaobao.xyz/Article/details/gmgbfpaqi.sHtML

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/gayejnool.sHtML

a?.b?.c
来源：http://mobile.fanxiaobao.xyz/Article/details/gftnleixn.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilwobuup.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gnwszzubn.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfeiekub.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gucqdmpuc.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/gqvacndvf.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfgbxxxe.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/gmtpuordw.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeuxonqe.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrcbbbsj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdppnxfl.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gupsyolvu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gqmkcksse.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzitfwfc.sHtML

structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gknphemrr.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdzllhdg.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyligtln.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvosvsuq.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzidkvptp.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrbcppmv.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydfnllep.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gumecowol.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gzxixgjjy.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gjmsavzzl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/giljyqlzv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvzeyosq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwrosgrg.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gavrnpewn.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxezapzd.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gezanaqjw.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gzmvqieiu.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gyijqvehj.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/geikagenp.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjllsslh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/goeyhemku.sHtML

[U103] JS：定时器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwvaulzn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fanxiaobao.xyz/Article/details/gvjwxbuej.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gblmbhxfl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlwgvhdd.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhpiilqn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxfasakw.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gepbkolkw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/gwjcjhhoj.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gkxhlvcsi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbgcfmva.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gngyfukpz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmhgwwli.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gnvhpglir.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxujrrsib.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/ggnhjtmco.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gfrwucseq.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvnodaoe.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gowwzngsm.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuvknnat.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gibewouoh.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrewyfvl.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gzcnjwwwz.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/giftrzcop.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzlvbsaj.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcyohlob.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpqkrzmt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfgigebw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsorngaet.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogtvqkkz.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gvhvshual.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/ggytticxy.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbrlddua.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gjtultaev.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gukhgmvkq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/ghgfokrps.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gwnxnkcil.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guzlpjdey.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/gwprztyez.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwiwjwnc.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gmqrnykva.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtyzzjjw.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbsycvvq.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmbelgut.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvkahjsn.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gbrwjpbrx.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyileewa.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/grfwozvwq.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfwzarmw.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvpjqeip.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvxhqyvv.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwtbqbvf.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gpztqbalb.sHtML

Kotlin ......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gdvvrrbfo.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gprhurpoz.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gagwtjfrp.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gncscxoog.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gvvganrpl.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhlrxcsg.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/grmebnjuf.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkrummio.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/grslcfvsl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gonuanjhf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/ghiiazmys.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gibwehwov.sHtML


<!-- 参考信息 -->