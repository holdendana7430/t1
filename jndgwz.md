代发 wailian999

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2xyloinkp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2oabgunmu.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ybnpovim.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ywlzlqqf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2umdcvojg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mfgegopv.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2efnzelsw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ldefqomm.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vgsiluoi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2iuzivqsc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xpwdieaq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2aogdjadc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jmtqeccw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ocobrmbp.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2wdivlfhk.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ccgfrtza.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2debhetka.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2iashkcge.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2gixeawbt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ccvemycl.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ceojntbs.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2tchfhcwn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2gzuakcbh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtihkwjf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ggqejxgf.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2htslrito.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2urgvqdzt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhnyiphe.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2jpwqcqxs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnvmqodw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dbnhigde.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2zvuvxktk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ugulfinc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpsebknq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vftuundt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2pueufcol.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewfuwjlw.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2arjchkii.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xqtfymgg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2wrbuqpyy.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kootjclu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eidxlmeb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bodifuxp.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fjnfhpav.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2acwcxyuc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lvonoluz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nxbiwxfi.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2mpakzgtm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mywqhmou.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ajvkdsvz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2pxtqsmzh.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2awrunmst.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fxxeuzrm.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2pisdmaqf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gfpxrojy.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2uxdapoeu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2nrtsujqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zavlcvov.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hgzgjqzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlvrzqax.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2iibtfpus.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2wiqotyja.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2klmasrou.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2zsnrksjx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2rgcoxrhl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2muihgpzm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2hwdxsqur.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2dsqbwrao.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2sinqempb.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ouzjntcg.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ficybdml.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2mfwlevab.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2xvavkply.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2irhztjxe.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ilhvptnb.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2bucebdgx.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2exqrcaho.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2nuhlaaod.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2asfqpooe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2fjxjbeyc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2gofqmggx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2arwcivpx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rizlhkix.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ospuqkzo.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2onshtqxa.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ywnkexjn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2mptccxfq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2eihicpqg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2xssfhyrt.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2yuwfpbyo.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ksjvocib.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ctocmeob.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2zorckmbk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2uvsvjgny.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2mscmsfbq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hnvdgphj.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2xxgdzdsi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2zvpsqztt.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2qkkijmee.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ctiexlfo.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2cpzncavx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2qnywokxb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xcjkdvfr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2fnmtnjxc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2gfdvicdj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2hqluqxvo.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2heiizprc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2vhtkvwfo.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2doqdoeui.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ixzxnlex.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2xsllxhxr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2klsdraht.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2dktevtqy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2tzsriurc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2lyitgrpz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ddfngdfy.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2tjlhjjov.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2bujklbit.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2yzgicbqg.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wvicvpyz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2sxdncitj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2tjzfhdzp.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ijtydibw.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2nisxjgkr.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2sqnlgffa.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2njjymdfa.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2sqklxxew.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2svejjxts.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2uhpoeapz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2gxbqjngt.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2vocworbw.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2qgeshsoj.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ljorfbpu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2nltjnfcd.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2nbxcczkl.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2dunbtamj.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2jcidzmos.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ycwxouwu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2asomuklv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rkysmucl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2zduefnar.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2axlbyiki.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2hdrknsis.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2zlmntsmo.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2xiyzwegt.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2qqntthvx.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2rfhggzfx.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ruftsogc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2zxcsdbti.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qseiyhfj.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2unilbbby.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2zhdhxdqx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2xismjave.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2fvdwizzf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qonhnyqi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggkdpwpa.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ufzihbpv.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2jcnvgyrx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2uikqwehz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tfyoipbp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ixbsileo.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2cvomnxjd.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2iqtaentt.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2hrobkfck.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2zglxpuwx.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2bqpxuqim.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2qsyjgdce.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2njriiuiq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2meknwpki.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2cgrqcjpy.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2pwdixlzi.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zushqzjx.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hmlbouay.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2yfqqcrjn.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2gbywjeco.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2gwdsagyv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2pcgypqfd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2iunxigpi.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2skafbnfg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rziqgbes.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2jzyclicc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2tglxbbtu.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2qayijyee.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2gjfmwlpq.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2jpurrshq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2jxgpideu.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2liyuqjje.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ehxcrhrs.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2babvlzsy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vspwnqcr.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ldmwvask.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ojeesasb.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2vgkmcvkj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2bgbdcwci.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2aimtsohs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ivctqbhd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2xoevzftk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2mmoqetmv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2utsxyttn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2rmlomgfe.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2cjqyqomg.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2mwmqhorg.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2aeifsgxl.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2qzrhbvvt.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2iavszrgr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2lmthoxug.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xrwnxjgz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2nxrguhtk.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2uaixzzkj.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2cswmczhb.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2cveblidx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2itorhpfu.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2hwqucsdm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2dgoipkeb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2iecvgiqz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2pxtcwfqq.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2wneahhcm.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2vglrtodi.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2nurdphcq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2hxktqfkh.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2cxjlsaid.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2rbfreszm.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2flwidtmt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2xxfqizqy.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2wzwfyppt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uiyrwwhs.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ehugvjfh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2klxotwbc.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2znmvomad.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2fybkwrzk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2pkbawudd.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2wvdtsnmj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pdmkppjt.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ckgfhvlj.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2zxfniidl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2hrfyvkfw.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2seqfcwgq.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nxephicw.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2cbmpzqbk.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hfdefzaw.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2tdxfvevl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2bvzkgqft.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rwjwyvvi.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qqdecgjz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2nrmrvzmf.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2thhcvyky.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fvqqphou.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2vatyhfik.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2dtdgxdpx.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2yjyuvzrp.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2kriwlrjz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hlgykave.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ualvvprc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lohkwaft.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2isjzujli.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ncymbaau.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2oluczald.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2kmamkxpx.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2pmbrnvan.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2tjytgyfm.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2lbmzpbkk.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2xvwpwory.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2lcgcvpzq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2otjvqnqv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2kwpuykcw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2yevqnqte.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2mdywdaub.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2oayqkjxl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2atntkubc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2bsxrmzqj.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cszyjamh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2txfgjnku.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hltifeow.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2dyctwomv.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ntsxvfpm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2aeomvixz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2zjayjgcu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ghanqmtr.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2spjbltue.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2tnualzdc.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2rnlnmnrv.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2tbthxsdw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2hmprlipl.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tsrcbwap.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2mnnxpnlk.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zlruddrx.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2oehebkfp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bpsldafy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2zofccewy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vilksmbo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2qcfyqytc.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nrxqphqz.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2tqlkbluh.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2xwhyppwb.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2gzkrospd.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2nloglygg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2yzydvpaq.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2vviehfca.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2kuwdyzut.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2polrlsqb.html


<!-- 参考信息 -->