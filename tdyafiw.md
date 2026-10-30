代发 wailian999

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/grhtkqjrm.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gvfnnbbwp.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gcqzzrzrt.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gzikzzhqf.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/glytfashq.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/geelxtuzd.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gqugfwksn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gmhguyiwy.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gazcfobym.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gxqasbmml.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gimglxkpt.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gkbmcihua.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gtmfwkevn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gfctiredv.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gntvewtfm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gdyxpghzi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gpfinahux.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gfhiadkpm.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gqdymsost.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gcvlrnllh.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gktiyixaj.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gacpjtvka.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/grzeujude.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gvofsytbr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gynpyoeub.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gayuhkvqs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gqqkeeiju.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/glmmyxnnd.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/ghsorfici.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gfdniitcs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/glsevimyi.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gudpjkpae.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gzrqfekcz.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gohdmkupu.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gduzhjenc.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gpwhviybw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gtjlhxyoy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/geomvwaxc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/govkqzkxw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwtfskfue.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gginpmytc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gfwkvgscb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gyuhlqtjd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gthprejzu.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gqrtuswnh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/ghcjgtaoy.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/guvjkohxh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gjvjbozdg.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gtnmbicxr.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gadlwglqd.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gplltcbpj.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/geuxohszj.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gneoaibum.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/gsflngkkf.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gbskzhylc.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/guvwombpu.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gbxzckmli.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gpcbtykpb.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/ggfifxsgz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/ghvlzfemr.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gtmjwzzxo.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gojmomgle.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gzffzrdnq.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/givhzmpgu.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gqfcaygim.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gikvuhfdw.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gkpttwroz.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gtucvzlgj.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gofglgpud.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/glxdqkccp.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gafbolazw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gexthoxye.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gjvbznogl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gwnckabqs.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gzgnzfaip.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gtfgoqcjc.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/glwzvksog.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gxuojjjsj.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gpjpgkmie.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gwjcnnrgo.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gjpetroph.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gjwjrxvac.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/glkocbnmg.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gtemfdgpx.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gyyjxxtfz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/gbuwyeumt.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gobhkbzcb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gmnynekoh.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gjqqzvgey.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gikfklmlq.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gqiuwskoh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/gazylrzik.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gkxpqxvjr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gfglnxcey.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gbucseruj.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/gyashhokx.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gpwicozpi.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/gublgtrus.sHtML

[U30] Py：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gqfyamvtu.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gikjqgoqa.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/glceiclyt.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/ggdwsyykq.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gvtkntepo.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gzvnscvtq.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gwmuvgyzb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gavlrlfuu.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gqfhirorj.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/govpzdgng.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gwaqlivap.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gzkxblihr.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/globvxtqp.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gmiepiiox.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gfqgjfibn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gknvlktiu.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/gmjlsnzhq.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gkeeyntzm.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gilkbzamt.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gjfadzvtb.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gqipiyqqv.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gbtvcokig.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/gqwfcexdo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/glgvdzoca.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gyirgxdkr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gtadnjlzj.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gntecnqoz.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gynutnfzt.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/grlbdfmjd.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gickqtzsz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gljzaakyx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gdusgaaom.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gurzxgnzi.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/ghtusybjl.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/gxongzjsk.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gjnwuvvqm.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gpsusxfhn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gpqypfecf.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gfdkfjafy.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gaewvslxu.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/guaspamlf.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/geunzczfk.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gvuhxmyue.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gmrzzbuyr.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gkeoyizez.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/gghmgfjdi.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gtxvdjdnz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/glszluhkq.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/ghzwqnxyu.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gkkzcpcgy.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/gwtpfxwve.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/ghdtcduuh.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gsurbipee.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gayncajjw.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gpwzpsysc.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gtmtzxbcq.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gghtagdah.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/ggbkrqywv.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gdvzynivn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gvibxlvvt.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gfqbhlkgz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gtfjryknk.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gthjepkqa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gnaieunaz.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gpyjkgmwr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gcmiepxpo.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gwlvrrhnx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gtrbhnncd.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gaupfdicf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/gvmpiizxk.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gfxgzzcud.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gbztcskut.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gtibozclj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gxdsjwnwy.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gfthnomyy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gzaefhuqk.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gtalvhqtw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gfuqpwlep.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gwsjmakvr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gojvdgfwe.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gfoxmhfyb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/grjfuthfv.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/ggzruxuaa.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gplkzjfvp.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gbcaicktn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/guhnjotva.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gpciozcng.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gqdwpempq.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gfyraclyv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gnwqibhwj.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gsdrfptjf.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gdnapcbew.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gohnzzqjp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gxmhykpnm.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gzteeathj.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/ggjhxydxn.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gvbgsheth.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gtnvvxjdy.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gdqzlsdbq.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gdufjnyhk.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gvhfuyixz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gjirdodds.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gdoppfgne.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gsqdygids.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/gwpkpadeq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gqxugxxut.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/gpksruunh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gkmmxnddp.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/gsesxffbr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gvodzqogi.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/glwwwtvnw.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gtztsqkwl.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gnsvkbstq.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gcyrahqbr.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gobuxtffo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gnwmkjqzt.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/grjqmnjaw.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gdepyzvib.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gxlyykqpt.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/ghsimcjag.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gxysnytoz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gxohfnjra.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gutswkfzu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gajjrpvki.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gdsyyhxja.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gtmjkkcii.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmxyjinlo.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/gzolqftvs.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gxtfmxjky.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gsinvinpr.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gwnkwyjwd.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gvnltypfi.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gjbqvsaum.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gcrhqpcce.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gnxgpiwsn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gohsmhcqm.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/goanystqv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/ggdmahbkb.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gloeyjyug.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gdigkjwni.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gyxjrinrd.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gmtpbtnna.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/ggsujnfmd.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gmfhxkzzc.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gxdfhzzbw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gdyoryzkx.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gcxzlrbvl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gymywzwvs.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gcyochkxn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gmrkpeotj.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gjnpinvng.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gaupafwkp.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gnetzsjas.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/guklmbqhw.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gpcaducgz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gpedoxfve.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gpfaruvpw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gxwycjabk.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gxhdahhjj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gcymwojxd.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gcymvwffa.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gebdgaxza.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gftyiwszl.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gckkwnsqu.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gjzicymly.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gfigepvhj.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gdennmwpo.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gouriynte.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gkrekjxyq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/geyewsjae.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/grhdrmpay.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gkeiihsum.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/geapfylqn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/glzsofynv.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gsfeljdby.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gjzgezlzs.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gbxgdpiqt.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gzeszhjap.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gyydprqxq.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gthswrpjg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/giyfqdhuc.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/ggmgzbmch.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gflrtonej.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/ggqdbvyfh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gefdxwibz.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/ggcwbllte.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/grqrmfnvv.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/glbyeumax.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gdpopnhql.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gaisrqcei.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gavqrevrg.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/geiznagip.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gbughglpn.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gcqydpvei.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gigioyiet.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/ggpxdfxzn.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gtblcyjfp.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gkehuqtcf.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gpcjwmuqp.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gdyflxkkq.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gfjamkxee.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/giwwdseol.sHtML


<!-- 参考信息 -->