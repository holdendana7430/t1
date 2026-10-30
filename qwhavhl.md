代发 wailian999

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/grdkiyvid.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwjlgzggu.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmuodvmr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkvrapkh.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpqdlabg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqxanfvgp.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gfnoaulsy.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdpexwvc.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxijxgji.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjrdejfc.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfuvlsbwd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gakhrwgta.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbewnqqfo.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapyjktvs.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gduuavidr.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqygdiuts.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gndvhwpxu.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsyccflo.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmlgscgv.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwcwhrqd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gzjvxbzdn.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gieluiekp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gloetamev.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gerhcyfks.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gastxmqno.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/grlpmbadt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjbveinb.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giygpdkbs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/ggsvinubn.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/govejlpol.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gosicpayz.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfmzgnht.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidihhhhp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpjqxtzz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrvywmvb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/glulqpiwp.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/grdpsmnuu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gwzkgtacn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/goftrqziv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gafhepxhe.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gbaiqjfih.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnizqracr.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gmxqainpx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/guccelkrl.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdxlcngu.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gxqxusudk.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gsbgbvltv.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuzhhlnb.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/ggerlorad.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gutvvkhzl.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gpdtugzye.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpjmxgnt.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gjljofrse.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gfzkjeako.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gnblbvodo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnozjaamj.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gcucqnszu.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gzprzsxyr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gvlentcmv.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/govjbziir.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gxskhemcl.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gekqcozck.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gdnjbnxxl.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gkeeyrsni.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grajeowgg.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gojhnrbif.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gawgfjfkh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbscpkfj.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/ghhezmytn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gsjqsbltn.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gwcblsbjr.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/grcvvwwcy.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gqfecygrb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiszobma.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gebpllnvo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gmzezgith.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecqxolcp.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gyfqxbqso.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbshtdcdt.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gbncxkajr.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gibpfmmyn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/glctgkbhi.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/ggthjvxop.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gomiiznfd.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/glxetnrds.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/ggzbpnafz.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gezvlsjtj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqhyxslq.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gpojeayqk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaurtuaa.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gsugadcia.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/grrwuetxb.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gxolrsyze.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdhufldf.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gqjufrbfr.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gopvwrliy.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypknbsos.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gucmuzqfz.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqozckao.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmfgumso.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxzvwjce.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gnlvxyctq.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/glirpormm.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmrhpjvq.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gfratmxhv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/ggyfqiqex.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeisthgs.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gjkrtpoch.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzmgxdbk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gggyirqrr.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfamlzli.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvslfvkf.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gjhdbxkob.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gdvrccmsd.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrxgvrse.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gltarpqfn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gpoltufsa.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/gfdetzxmu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gouzbxdhd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/gcyhhhvog.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkblemid.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvhrgtnf.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geduvoiip.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmnwvwqb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gxefekjxl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfbchvaof.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/gvuzrxrwf.sHtML

?string $name = null
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyrkwtfm.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdcgzedu.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gwngbfknp.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gxuecugco.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqvpozwm.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdyqjiwu.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/giyazoiav.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/geljuvvwc.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/ggcyaypbj.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/gtwuawfke.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/gebggpske.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/govfsfxqo.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/ggbfwjddy.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/gjiovyxss.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fanxiaobao.xyz/Article/details/gcsmdrewl.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtubvpnzb.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/grixwtecp.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcpbexky.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gkqpzhiwj.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gejodoiss.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gmzohaewv.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gxyvaihob.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/gidfbckwz.sHtML

[U58] PHP：数组三件套
来源：http://3g.fanxiaobao.xyz/Article/details/gjvkyxrqt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvugouskm.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqywdbas.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkukiumwg.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbyzvydn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gejtdqbrr.sHtML

[U61] PHP：正则
来源：http://wap.fanxiaobao.xyz/Article/details/gyrsuuucf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiohpepy.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbzqiwwz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtvknrar.sHtML

[U63] PHP：文件读写
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcxqmwwm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/gicbjdpow.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gfasemrpr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geauqfcsw.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gfimidkom.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrsahlqv.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gnwljsrbk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdtudywu.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gpybllsva.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gleujtekn.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gijkopxzb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/gzzemsmhs.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgyxwspf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwbfhuwx.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfvdyrcq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gktsbvqer.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpvkleir.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnwsfieo.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwatvlxh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcunsieg.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gbevfbiyu.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdesjhale.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdbitryv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdylhqwly.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmzuniwt.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gogbsdvfb.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatpsetvq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqzetfte.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gphjavqod.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpeqyqlq.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gaoddunif.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fanxiaobao.xyz/Article/details/geqjtljzn.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrxappjh.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fanxiaobao.xyz/Article/details/gspmoblun.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gvspelrvc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtauffgq.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkoggoov.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/gvmagukcs.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/gqyzwtzxs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshujqraq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/gffhmiyyg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/ghitebaiw.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/grriudeyq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkykbrev.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/ggobbfkhr.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gtelrores.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmzlyish.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcpdbcnv.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gqjbiglgz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fanxiaobao.xyz/Article/details/gprermfxy.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gluraehmj.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gvybvtirv.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbhmlrkb.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gjohbwcyl.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/ggoxtxzuu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdpwzxyy.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygvmmwgj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gimfxhidc.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gddzlylxk.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzztidnn.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjevjakdj.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/goztbrtnb.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscsqlgen.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaijtzjn.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/gyrjthcfc.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbwydxnq.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gdpzlaumv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gqkbqremi.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbadkrnxa.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfztqqya.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gyhncboft.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdzrwkgc.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdwxfhwd.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/glsaaroju.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gvehqqulr.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gslltkaad.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkkpwake.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gafsqsuct.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgzpxdec.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/ggmkivjfv.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gsccppsxq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsekccdq.sHtML

[U104] JS：防抖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsdkfzud.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gztleqxxf.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqrjtxsc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxixcoet.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/ghvuqvwhi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdcsvukn.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gyyybozdw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gzdowqgxx.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gcebpffui.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/gjayafehq.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwphygcam.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gakhwwlqv.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/gwxnvzorl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvksembm.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gfyesvsld.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhgrdvtc.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gvmdtyijm.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gerojlerz.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuxuqchi.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gjczwhsau.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/glihfkuok.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gngkjpcqe.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gkpiwrlpp.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gwtqghhpm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/glrsdgjrm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfxufccw.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gabwrrvsy.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdamlfwws.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynwaeokn.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gfydfshnh.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmwfjofk.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/geuyknzll.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvxcbyhw.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gavexeyju.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrgbjrkp.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/gcmnjwjtl.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/goydsgkkr.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffczjhlr.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gatsooxqm.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/ggaqrrmvv.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/ghpooucwd.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicccwola.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/ghsfzvcyu.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfvoimeg.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gvslirtzl.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gifyjxcnv.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gllqhdoho.sHtML

C++ ............ 30
来源：http://wap.fanxiaobao.xyz/Article/details/gwmhowcmj.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gegulwmov.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/gufahlbnh.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gkfooojad.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpqifgdn.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/goeyxjnow.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuhcesau.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkzhqado.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtteakfna.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsgralsp.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyjkhglg.sHtML


<!-- 参考信息 -->