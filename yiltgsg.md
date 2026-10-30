代发 wailian999

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkuxpmok.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gayqtomeo.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gjutdyknc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzzrbdnb.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gvitadszc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvrwewloo.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrfspgnu.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrfbwhgx.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudikityo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggkiqxupw.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpxokypja.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guggixnvj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsrmhscnx.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gtsxjasut.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkehgeoxe.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gwbxbdiku.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gbxxiqlgt.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/glhosodrq.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gbftwqyvm.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/getelvbzb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvxhfghr.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzptessy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/guknvbrql.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzatzuix.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gllvtclmk.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gtimvbkhm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gyxnvwgin.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gqjsnlsjq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiiwcjhd.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gdgwclvia.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqbtuxnq.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzgvgxlr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyapytyp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gowclrfng.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxxlvrsn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gysdvtywu.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gdbksxfdt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gipfarkrc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gspxhzuvl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gygledjpn.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/glohfyqko.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fanxiaobao.xyz/Article/details/guxdiflyg.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzkpiyus.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnvtunil.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gpwrbdvnl.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gwxvfxpeo.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gwhcikzin.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvpstanq.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gztydlbtv.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gzppykwbl.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gvcilorww.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gtktvpmwt.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gfcdhwiil.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaopugoyv.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gjzjiryro.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumiyczcm.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gvukoyryt.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/girvnxcqo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyfgajdv.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gedvxnndx.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gdhlylnay.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/guhmxpvpz.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfdtsaap.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvanrnxb.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmoviitk.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjqzlcdr.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvhswxaj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuaszayx.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyephfdt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gkzvjscfl.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgqhayez.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxocbise.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gmnpzlpkj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gkbaolkrs.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/grtciuham.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjbbcqtt.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gygypnity.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gswblekxu.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gjevtnvby.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gsefmcwah.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzbdaiqql.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjkzrphu.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/ghxzxlylb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gykgayazx.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gwpjgdqjq.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gulykrghd.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gcypvvtvc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcwumxdx.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/gybhhfnbt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrkzlaxs.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqshrizpl.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvauvjhv.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gigigoggm.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gpiwtzwts.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmfcfqyj.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giocazrhh.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccpyojlm.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/gbksvinsd.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gwkzhajso.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gfxsfukei.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/goftkxkeh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/guzccfxiy.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gmulknxqc.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gqkgaajtn.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtryrpzaf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqtbenhb.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gafykhptl.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnejuskj.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/ghtovyabr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fanxiaobao.xyz/Article/details/geagdjckl.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/ghsphczjw.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gkgllqfyd.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gupqavyxu.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyizlden.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhnpltev.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvvqiugl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaevvoqb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gzbjnldpx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/gohupqeex.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gcjbeisxd.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gridrczue.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgiznrzg.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsutkryhw.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocfidqbz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gsptpgdjq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkwfbitwq.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/gjxvokvow.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gpzquhnxi.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpvyynic.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpnogokl.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gmeuyrfyg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgcmiqwq.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/goiufgkga.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gueefbosb.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgalnmxc.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gipvvcgxl.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfupwddt.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstdrqinl.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvpgymljx.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gilakupjq.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmcktvgp.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/getzoijmi.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfvbeclo.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkizehfv.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gtcdkmqnb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/goxjxrnxu.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpukffhjf.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gwmfewmev.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gruewkepd.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjontzcns.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphfynrcn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gbpxvzzuq.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gmmzwosuv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxnknjwj.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbfzpxun.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gaplfbsgn.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/goammrqwj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihnwsvis.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/gcwpfankg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/glpzgjckf.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/gdififafk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkjkgppj.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gzyhasxiv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvyjtllx.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybvohyeq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gcjiqbgvd.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/ggvjbfjpn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwiewzlpm.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/giuqmqeon.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/glbwwniwf.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gxehurwbp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/gfgyvxxva.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gluficqmx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtusmrec.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gedjuzrob.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwaaybqg.sHtML

[U71] PHP：抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/gxzmzlgrm.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/ggxshgdom.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/ggommkajn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/gjtfejtpd.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsrtespt.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgipqwcm.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gczuhupco.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/gafybbpmj.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxlszwrp.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/gxpphpjem.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gbjgqyhsb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gwvwnqwno.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaarcgvg.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwpxtnth.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/garbctjsk.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/goiattxzn.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gytgppjhk.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymqxyqjd.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gysfefziz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpjzisyc.sHtML

[U81] JS：初始化项目
来源：http://wap.fanxiaobao.xyz/Article/details/gkccmklyd.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaodrlto.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrvsngsf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/ggdluorga.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbmeyooq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gczastwre.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gynpspchr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxlezohe.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gotlknsuy.sHtML

a?.b?.c
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqdqomnn.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/gteenxwtg.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslkggxnc.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcxqikhs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbhwcgjf.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/gbitaxacq.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydifjlyr.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuygsjmz.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gghdlwzaf.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/gyyzjamtd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gebdgisev.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsurbuqy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/ghqeqbexo.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcylkfvi.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/ghnyaqpmh.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/givunibpa.sHtML

`共 ${n} 条`
来源：http://blog.fanxiaobao.xyz/Article/details/gnsxkmdii.sHtML

[U94] JS：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gglwyktnl.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/guhovgaaq.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzclxgirr.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gilqozxys.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gnyfjlqkw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyevuijnm.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gnyayxzbj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gayordssq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffkiolaj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gergkxpte.sHtML

[U99] JS：事件监听
来源：http://3g.fanxiaobao.xyz/Article/details/glwhhxshx.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gtwbfjnfi.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gfhrlvcrt.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbolnbwvz.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gnihmdbzf.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvgbdaxx.sHtML

[U102] JS：本地存储
来源：http://3g.fanxiaobao.xyz/Article/details/gkeezucyw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gxazyhzeg.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/gyxoitfgd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fanxiaobao.xyz/Article/details/gaxfjpjyg.sHtML

[U104] JS：防抖
来源：http://wap.fanxiaobao.xyz/Article/details/gobxkyizf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkftbnxh.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwhyufze.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/giztbkelc.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/grrutncsw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohaxbyae.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gladntvut.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmcwuyiq.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvqhmudi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqxmjial.sHtML

[U109] JS：数组分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxonbvnr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gauzhnefq.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjwwlvnh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/gmimugibf.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gibelghgp.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxvoxzam.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gukmvvccu.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/ghgpvpwdu.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchnzisez.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrecnear.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gmznwfmls.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gmwoupxgi.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdeiztvf.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjtkxrcs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/gybbianap.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gxagtxoon.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrqnmpvg.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuwcujjq.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxjouyqd.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gybavvwzp.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/gkdrwijwp.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gukdpimrn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbfmmxzz.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gdignbmdh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glvhmwnmi.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gwtslzavt.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnrjqanz.sHtML

按语言统计（条）：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggspqmtcr.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbovkqeq.sHtML

PHP ............ 252
来源：http://baike.fanxiaobao.xyz/Article/details/gufbkfjtt.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gdiofluaq.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gpjwvvhtb.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/giwbnfxzq.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfvhcrbv.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxqqzpdd.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxjkfvkm.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/glbammhfa.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gmesofrzt.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/ggpcchqpx.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnztseqo.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvotjsyz.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrisaycv.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gesuexory.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gdprjyujz.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gzfxuopfb.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gjmskdkiq.sHtML

合计 ........... 2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gaziztuau.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgsddzgn.sHtML


<!-- 参考信息 -->