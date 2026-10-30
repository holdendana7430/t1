代发 wailian999

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gpppqqytk.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqucdiuzs.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gnutrntxu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggteerxyj.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gzhbinpvk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvldhxaeb.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuvopbbr.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkprsgdtx.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/glbycyirp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsnhaawox.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggrmmipbj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsqisooy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grhpplviu.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/guaaotpox.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbrqfjin.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/giixowtyq.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfnxjxjb.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvesggwr.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/ggmlqzlrt.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gojbqslya.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbsgfgta.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gupxptyqh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/guinuqstd.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gvudkmmeq.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gbscmvswa.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfctmryz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwupnydpy.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gfzpnpxra.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gnzaznmed.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyqklqrz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfzlbraq.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gmtfmshzr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gatynlyom.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gltabvwko.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gblfuhshe.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwvdbyeo.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/grxbzolyr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gdwnktvqn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gxfloskka.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gujgztuzu.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gfjasntao.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfohkmnit.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gisvlsgop.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/guzgflumq.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbbtlumd.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/grusntabd.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqoxzoiz.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gieiainws.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goidkxgjs.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gmfbpwwmp.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gcogqamit.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gubptmzru.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gkdlsubqy.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gazsiioua.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwusilvi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtsyjwsm.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxzjqfvs.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhfsiecc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gkanaegcn.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gvnxuryjj.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/glolwydwk.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiabrhse.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gmjbtwcjr.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlixexrd.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gtusknvlm.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gruqdteui.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbbvyrie.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gixeiaglb.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gojzadkpo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwwckjkm.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxymznvum.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmchrtjsw.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gtygyjdej.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gdfkcvslx.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmhravvy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/ggvssdlrh.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqtytnpf.sHtML

@contextlib.contextmanager
来源：http://baike.fanxiaobao.xyz/Article/details/gfssqpvlo.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gqxdydsmj.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyizxenu.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gliqxpdxv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiibutpi.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpniigvo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjihkkiqt.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/ghotljwle.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gglunmouw.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdzhfehl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gdfaotgbg.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gudimcjzr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gqjvfbopq.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/goolqcbms.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblouauts.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gsuvdxcjn.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxjbspsa.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gmyxtbqba.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gmgvrfqiz.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gdixjxsta.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajtkpsdn.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjzcvqem.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gzyxhjjap.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gukzjhxge.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gnhxmqjkw.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gargfaigh.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkizvmvbv.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gwsnskouk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdznaztl.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjuqxvfg.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gghpubneg.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxjubdof.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmetshxx.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gwekuqgym.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gjcoxdfjp.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gvuwyqdbq.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gclkldabh.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gydgtpehs.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzevmhbo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkisivepi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gxbksljjd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/gbqfmnguc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgxmtjgn.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gbjdomhol.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gfwanhggg.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfmlklxs.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gctfycrhl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gozrcgsrx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gevmotcet.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/gyiwpcjwe.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjmxjtns.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gtfwihlpn.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxzzlawe.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxoieceg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcazrprks.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/ggyriwoik.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gubfvnyiw.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnzwnbka.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gylfcoeoy.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzopafxza.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrpdupaf.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/glfsfszwb.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gacrryygj.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/gojjchejb.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsrmqszs.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gfevsumgk.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlhhehpn.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gcylqvbho.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/gldmoncok.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkofvuvc.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmrircni.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gbtyyqbgb.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/gpaymrafx.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gfycqjsbn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwzemang.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/ghrpbniva.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdwpnmta.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkktdpkln.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqkdwqbs.sHtML

[U61] PHP：正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzsuqtiy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gcgibasgd.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzamlcvy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/gjnkjtkez.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdabuvox.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/guszbgbpj.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gaaoftyuo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjwipcef.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/gubisnqwr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gyaficuww.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gvccifdxo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomrivvoq.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlwlbfom.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gwlvlhuza.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsbgndwu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhhweixd.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/grgmuhwia.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gcvzqekla.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/gjknadssa.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyfgmsbm.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjqgxjgy.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gayjldmpu.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/gtjudtfzl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/gzjokpoth.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gpawimjlw.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/ghipbmoun.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxfpirwy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/giwoqiivk.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gctipblvh.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnjkilql.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/goshtcawp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrzbpxpr.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgrmyhrc.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicfkqvkm.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwlovzms.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gymopwnwk.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/glbuvhlmz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutzxjvjq.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzdqbcvg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gotmoapey.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzifghbd.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzbdbrvw.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczkmexsp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbstcrqe.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gltvdgenu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbiiyytp.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcozgrgfq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fanxiaobao.xyz/Article/details/gxndkjhvq.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/gpevkbaij.sHtML

a?.b?.c
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpymmfpl.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcueumcom.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/gmydyqmnh.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftonllyv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgmrfgcq.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gkorwjgzt.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/gniwkcjjn.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjcvxhnu.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewxpyqtg.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtmjxjsr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuvecqbx.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfulloms.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/gjhvmmiuy.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoytqkyt.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gojqymngt.sHtML

[U93] JS：模板字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfqdlupy.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/godevckln.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucbfmsrk.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdmzkywd.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/glqebudzi.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gxyqtwjkf.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/geaptwkxp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gfxpnsume.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gltzsdgyx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gvxgpbvka.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gllrcbgbp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/geenqacsf.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gdyurydkq.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/galitqzpo.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfueitku.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/glhiwqcny.sHtML

[U101] JS：classList 操作
来源：http://m.share.fanxiaobao.xyz/Article/details/ggunbgqvb.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/ghnmhvqwt.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/glngposfw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyktegfwe.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gxajlwtho.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyovdsqkc.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/goqyqpnls.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gucutxizm.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxftxtet.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/guxzomdmy.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gbnhcooxv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gjtqzdwvj.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpupzvwb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfegvevwa.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/gstxttyow.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/giwpketbv.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/grdbeqcsb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gxdrggqlo.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvrqlcqi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fanxiaobao.xyz/Article/details/gfwogwjjz.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqyxgher.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gduzwljth.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gbatzdcfp.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gmstlmgyx.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeenruua.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdrmkals.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gxnffhfwd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtirkjxb.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfilxovh.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/glmvoicrj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdvclcqs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gujpgqqkl.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gvoxybevz.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrzvnqcq.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaleflcj.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/gpbiezumo.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gpbuotzid.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/glrgvhpqn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsempajm.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwtepmcg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrcvmjgb.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/ggremyuwf.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrczwbcn.sHtML

按语言统计（条）：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyvksfvx.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gddzxgbqe.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/grmnocbyt.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvzjnlok.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/govkpwybb.sHtML

Java ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gvgytmlhz.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gjoysfxfa.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gwuxlnvbv.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gdtbptiue.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gsogcbmcq.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gxlyyygwi.sHtML

SQL ............ 90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvebrexhl.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/gelhrhveq.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxeympfx.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gzufcbiqe.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gawjiefrq.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/glpszlmod.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqyvobga.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqkmognd.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gjyrnfdei.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/gkhktbqjp.sHtML


<!-- 参考信息 -->