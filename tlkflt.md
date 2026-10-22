代发 wailian999

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2kqgxwflf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2rjqfyxwf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2znuxbfcu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2bvhernsm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2koilrvzc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2viekjwrq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2vthpvamd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2gymrbmmf.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gkskoxgi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2qdapqhwe.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2mxdtkxil.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2kcorgnkp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2irmmcxmd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2dcrylvtp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2miypbppv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hjmxuxpj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gwrgcgfr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2mmfzgkrn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ffkzxwdu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2bjkinipd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2powiawtd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxquidhz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2hbtjimxa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zxcwvouf.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2uiovmayo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2wgahhtxf.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2vhckfyvp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2makbrmwj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2facpauwf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vereeiop.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gaaugblw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2gabttspp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ccyerbdh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2urrtznah.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jzxgdinz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2wvyuihcy.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ipkcvegb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ckdzpbnx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mzwzsmgs.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2thjssioc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2gnpcxmcf.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gxpdzcxb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2sjovnfth.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2goaplkqj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2udcjuvfi.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vudzeeta.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2paizmhiv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2jzghjsyk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qhbiumzo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2scguvefz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jxwozoof.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2gwwihszq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2pketxlgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gvkqexlj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2thyspltq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ltihlqml.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2zueresmb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2amdjfagx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2myypqkzk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bkwfvzyb.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2mekeartc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2hvsmhbmz.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2tgbrpqrb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2fkdfcqrs.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ynvhhymu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qitffyyn.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ndtgjaeg.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2fpwthdlm.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2iqdwfuff.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2damdppmi.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2gsoyyvqp.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2lghzgfnz.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ulicmkrk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2sbekgdfi.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2yhzdaswd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2sahxrulw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2kabszaiw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wqcfiibj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2aayzcgiv.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2maswwrux.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2itmtgnwo.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2awwoootu.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2amyfbumo.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ylqavgun.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2tcgcfpwv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2satwywjl.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2zfmljdvw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2vemphfao.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2rbtzywqo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2jvbanuqc.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2otfruhxf.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2scbqcfvy.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2bixspjpl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2rlkguvyw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2uejogsdi.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2vjhukneq.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2viqprhmt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2vgnrredf.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2rapnxxdz.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2abdqnsin.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2dcoyvgxh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2bmrekqvg.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2jtswjoah.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dlgazccj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2rdkqxnuk.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2kgcmojco.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2jamxiqom.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2dtryvygs.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2etbkitpa.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2akkxxzln.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2pbzijcsp.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2igenjhvc.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2yptjbpjt.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2dzqenemj.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hfckkgxx.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2hycqmrol.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2njarizsk.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2mubrljee.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2mkonlojx.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2yfenqkca.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2qbsfocro.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2zulbmliz.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ojorzjtk.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ecawfvml.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2fsrncjiq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2sckuimvf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2alvzoohg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2xgtzyyxm.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2czpdvteh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2rmjpoqnm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2qzqyzcte.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2rwuhklky.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2uzdguynd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ofzwrsnp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2gmoqkzhb.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2enmaeish.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2esgrbyut.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2swvynwoe.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2konhpzbu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2jtbsstef.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2gdduxkvc.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2dqahfvaw.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2partlcab.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2iyyfveps.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2oxmmbwwf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqmyqcaa.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2flpbjcxw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2kuaawkoz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2cjifynbo.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2xartfnqq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rwhybczs.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ohplgguo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2xledmnsu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2khlqzkdy.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2vpendqkj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2dolmmeaq.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2fogccvzl.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ngxwcnue.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mmhcneao.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2juxmpyzj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2wzvqzlyf.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2yagyqujh.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2rrbgonav.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2ojyfjsll.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2nmelewwj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2apoozvnw.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2dufcmueo.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pzskoxsw.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xjjpzbjz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ujpjbcis.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2mybsfjwe.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lcylcpln.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2gsfcjpgm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2aqhlwqmq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2oqyzmogq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ijehskgh.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2tiafmwcg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2jnnkamzq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2euraczrz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2yzuxlwwx.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2qtbvlfnu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2iidvnjhs.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2nqxzlyzb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2wtyuiymy.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2nlsbpadw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mcqqttgp.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2pjeookgq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wzddkqnm.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ikxjhznr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2zafxuyuu.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2yqtinxqc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2llxykmeg.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2vfvtzoyc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2gzfwgieu.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2shpfsbwg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2hkduzysa.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2bjfpzsld.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2esxzfdpb.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2zgfaydzr.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2wahqwxto.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2suqexhba.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2gcpghghl.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gtgdxues.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2cuuaewuk.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2kmlicqas.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2txogfvxh.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2yqfbncpn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2beptjgjb.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2otcesqci.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2qyviiusk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kmfqzwgv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2bphiawbe.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2xztdrhnx.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2rbbcxpjf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2cbsnqmox.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2nuzkgjyy.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2rqmppkef.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2memzzxwu.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2bvwdwclt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2rvsvkuyr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2kmkcbuqz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2nctddfrt.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2lklhnjym.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2grfnrcab.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2cbjaozrg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2awfunxsh.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2vmouwhul.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2pjmfdmtx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2vgfjwvjt.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2odmhlmgy.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2smntfito.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2wgsqlpux.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2murkjnaw.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yxeaatda.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2yxyrfsyn.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qebkbbrj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2wlclxlca.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2edoqjgyn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2wsauowlo.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2aakvdcjm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2zdugxupj.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2duhpljca.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ddnyifnj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qwezkarv.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2oxgfectr.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2esjcgeiw.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2pbabinht.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2uatmediy.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2kauvpqdu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2isbokece.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2wchazwpr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2tdeuaspf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ptqdjold.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2zglbxcaz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2seygxgtt.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2deogbigv.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2bjsaifjo.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2bybplhgw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2kgkbyvos.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2zmschymj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2xoasaxph.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2qenqyjoh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2mpqngemf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ditfbfey.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2esmgzypj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fgfktawu.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xjjaxbbn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2zaolrewf.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2qevlmrvj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xxcdezif.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ppgicfew.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2xyauexhw.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2iemdkrnb.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2aeikqoba.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2bcscdfsy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ydymnuyl.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ppyvrnuy.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2syxgbloo.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2znmummfs.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tzcfiytu.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2dbpckgnh.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qgljeatw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2bcqivfrd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nmlkvkjp.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2gihvxuiz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2eoaqnssc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2uobcyrks.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2mmowlrql.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2byxqfppn.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2jvdqihsr.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2vhtpfkex.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ycjdmfwg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2kjumlwwx.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2yguywnob.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2jycctuji.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2aqnvtvbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lxcvpdvx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2cdpdpdvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqovgsuv.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2hlerlenb.html


<!-- 参考信息 -->