代发 wailian999

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gakflzati.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmelsejdc.sHtML

[T46] Perl：哈希操作
来源：http://wap.fanxiaobao.xyz/Article/details/grecrhpfj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeudxecu.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/ggvbpuyzs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrssejdp.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxxkivvl.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gqjpkfyph.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjxqqdip.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmwdcyct.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggngsutpz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gzmcdkjdv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrfgbucj.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gedqzoncc.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxacsibf.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/grsapoowi.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/glwmqksis.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gfkpwwurg.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gbfqddrlc.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggskzctoa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyeublqh.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gkjssjmno.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtwbhang.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmomzqswh.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/ggoubnasa.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/grmylvbhn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlbylszp.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gdimhbudx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/ganleqdqb.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gqvdfahjr.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gdozmlpdr.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/ghesnbafw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdesjwwun.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkwfzubz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gzgqbybvc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grergljvi.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdlbnslg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gqvyqgski.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gaxpeobjv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdaacuika.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gzwumtmcp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gwxwxzwbm.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/giinyvzke.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gotqrvghb.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/ghkvxzooa.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gkylzetho.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gejuggigw.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiwqosoo.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdxntvwn.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gkbatpppx.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggewlcemi.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gaminokst.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/glptofhcl.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/godzujphr.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gziiyurke.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gktnaajrn.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/geocvmadm.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsmttrqh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gqivucmds.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhmwuqnu.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrckwrmv.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gucbqepfl.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwfijfek.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrnvntah.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaeumudp.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxgdxbwg.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrvwxnla.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcwzenqg.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvaodqnu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gezfvcqws.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gnpmiblqr.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkytadpdw.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gyttmpyfd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/giygxmvtq.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gfztthpcr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gyefkdtga.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytmitgei.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeugxvgd.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqoqzxvv.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gebrjrcra.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnudvufsu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gfsgksqfm.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gsduopaur.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gwtxhsmjl.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkoksekr.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcokrjkdp.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxfalmom.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/gvtjwoihs.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclltawxn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/geixbpgox.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gqndtvlys.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqelgmmgy.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gudduhvsg.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/goscvbcmi.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gxiseminh.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gejqfpxdn.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gwesoeylf.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/gbiqumrrx.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gjkeeoxtv.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/glssxqnld.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrklcuvt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/ggpbrgaeb.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafyritgi.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gblvptiny.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/goquaybql.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/grgdugyxz.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmwcycvb.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjekaqsk.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwxrknsv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxiltczc.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/glmgjdgbo.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaqhahtn.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gelejizpc.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/grwskdspc.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbluxnxfl.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gelshgxyf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gblnbovjl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gdpnjxnay.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gehhabsao.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gqoqqnrta.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfpornpx.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/galsjakzc.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/grkyqqyrp.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqodyszke.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gohduwkxa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvkjedwe.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gvajhqnwk.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkvzmtkr.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/gecnyynmn.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjrgdrvu.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitwucpdd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/giigkcmlr.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqewddch.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gykejwqde.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fanxiaobao.xyz/Article/details/gmwxrubge.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gouzakzre.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gunlcsnrb.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/goiiftive.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gizsokbew.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gxnohzyjk.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/grdaptato.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfbhspvq.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/gddjvhuqk.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gninkbgct.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gswiflqvo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gsubiupca.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkgcmkds.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/grwtndkda.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/giebddpsc.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgiwsqso.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfgaequo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/ghfrkxxrf.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgdcbtuj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtpelwto.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/geexololx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkewvebul.sHtML

[U61] PHP：正则
来源：http://wap.fanxiaobao.xyz/Article/details/gtgkdigsc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gmfvpnkzc.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzbynzez.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqfcsadq.sHtML

[U63] PHP：文件读写
来源：http://read.share.fanxiaobao.xyz/Article/details/grmaserku.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/gyuuafqdd.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/glqokftlw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/gugprbagd.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gzezdpstr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfghojmgm.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/gizecuqiq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkumpuizp.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gqapjuqac.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacynyiwb.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/glbvjwwqo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/gnpqupijy.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjripiag.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gglsvibln.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gtiduuzer.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxmgbhqx.sHtML

[U71] PHP：抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/gvorhcwgq.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gtqyzaozs.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxsyzfqa.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/glwjrczmw.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gjmkzcgqi.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsebprmp.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giruuevpw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxfregbr.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gihkotclk.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqzfzpvi.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/ggpzayaqp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/glwzzwylv.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gomhcvyll.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsomxmrgf.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwfpbxhh.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/gprzuygeu.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumhmigzg.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxrfmphc.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpikppaod.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkhpgaqx.sHtML

[U81] JS：初始化项目
来源：http://wap.fanxiaobao.xyz/Article/details/gdgelbnnc.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjimaxxci.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/glaxninfc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfrjwfbw.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/gijlfqtef.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gpqsbgjvp.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gybliqmmz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlnulpms.sHtML

[U85] JS：可选链
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geygfedeh.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavjhyvxf.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gndcbrwve.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhavpdgh.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gnyqxdsmn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gnwyjubsv.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gcjivqdmh.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gogrzssap.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gmmxjhnmu.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/grdoubeii.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/gokxusobd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuoayepw.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdeewujnq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/ghrfzxsat.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gzvxymtbt.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzktaejho.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnyseioc.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/gmxfgpafn.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasxybldn.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwhgfuyg.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrhdbnsr.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyefvgidp.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/gkwntnopp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gdedfykbk.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/glxnddgse.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gczlucxve.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gapyrmsvm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfymebsz.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/gwijnrcgg.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gdzpsgiwj.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuzzhnce.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqsscvga.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcdrjevx.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/gtzzyqoil.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/gotbbgpuf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/gvrwiuqlr.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/gftlohlwd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/gchifrcbn.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/ghsjvaxdr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gzusfifkp.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guurfsuji.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gxmzsykzd.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/glkptbdws.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldiecxgv.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpjmfdzz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/gsemuszhf.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gqqsupwsj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjvzuraa.sHtML

[U109] JS：数组分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gczdszqzb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/girwoghkn.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/gcgwqlded.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/genvkdbsq.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gxddjaucc.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/ghqqzqkgu.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/gtuqrjymu.sHtML

"7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/glcnaueri.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpvscbvn.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcgbebge.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gxltlmjiu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/ghjqaghaz.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gyfavxyjq.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gufudvbjc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdqshmvk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyuuzqxa.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gexwcmupr.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnfqdiip.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gzftizlvg.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcvihvik.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/ggldnbatf.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/gavxldzsh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/glgbtuuak.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/glcbhvowc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gveryrfro.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/gwhnztpct.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/geondaybu.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gclzhyacx.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gyntzeepm.sHtML

PHP ............ 252
来源：http://baike.fanxiaobao.xyz/Article/details/godbwvlwn.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gighvmbli.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnsxdrnk.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcmceomd.sHtML

Go ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfhcrrra.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gdxndoubr.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdjcnyho.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/ggixchmzp.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gogsrcmrw.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gajfezubt.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrjpajsx.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohybolen.sHtML

Swift .......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glciwxecp.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtxbudvp.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gswgormyk.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gybbuxwqm.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoaotffi.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gckdiazqu.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbjhalgl.sHtML


<!-- 参考信息 -->