代发 wailian999

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3rksrfmla.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cjtttaxk.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jllhvqcv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3sggynxwc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3lkgkhkjl.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3mdorutnq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3fmwfiwvl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3lpfoiimz.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hulzxqbr.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rkcgzbqf.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3hplylufq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3xtrkdrnq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mlauivwl.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3iqfuhblm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3kgouggge.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3spyueteg.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iteljluu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ewbwyvym.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ikwqlbae.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmmzauog.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3fmubuqix.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyqmmmeg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3fegnbhcu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3hstehoyt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3uoltcphv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfkrbapg.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ehllfvvt.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3wowqtron.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kcsavbxz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmczfkqn.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kxjdafim.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3qgspatut.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3qmskrqul.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3msnkkagg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bqrpxvhe.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3tybichyl.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3sdgwvcmy.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xqevmrfn.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xxhgkjbn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fvhiljqt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3vomywibk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lhhhbewg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3kgxcipfp.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3uuipsqrn.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ukpsqdqf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3clrfliax.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ctncdkml.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3fdhyqonr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3afifmbmt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3zchuytav.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qmitttnt.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3dqsonriq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3fhugcyyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gynkkabe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3veryuxiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqgblfww.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3xkrtbpzu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3norobknw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3qohjwiog.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3idjvzeqr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ncqcqesx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3kciajawq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ymdnncge.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3hakimyuz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3nvpvbnbq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wdsfsukx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ubkdzcgu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3zrfdtqkq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3sbyyaevf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3apdpuiwm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ozeirzrx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3zomsknbn.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ovcwwgzg.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3tximpdvo.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3zwjyuoxi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ucgcehbr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fzsrdoqp.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3dvosmdmb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3swjvcjxn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3tkgqrooz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3fdbfneuo.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3inogdvmx.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ctbblysm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3kswloqvz.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ycbxslbs.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3upledmgl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3qjkqjdvc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3iilvxioy.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3gsigfjry.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3igvoiptd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3vapdvbnn.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3grbhhqtl.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3sivehcwh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3rrftissy.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3hwmwrtvo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3nwiejyke.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3tlpwasmw.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3lzsvqypj.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3nunskpzt.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ytajznmd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3gnbrbhbu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3atzilzwf.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3uobjondb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bztyurvq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3cznzcxdw.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3csizhdxq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3dmazcdob.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3wrvbcsyz.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3pdyytvcw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3zdqpsdpk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3crwbmzuq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3bkdwcskj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3etnbvnji.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ekjeafiy.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3nqrscejz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3lmuiwagl.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3howqubyj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3moiqtqxi.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ynitzvjn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3muavwpeh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3mbsvijev.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3rydcuocu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3djfsrogm.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3dsfbkvmv.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3jsothjuh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3sswvyfuy.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pwmzxixd.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3rpkbcalh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3sfjbicdb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3swebsngb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ppcliqiy.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3bjuheufd.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3mneujtag.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3hyxqzhbv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3wozowmkn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3tvqxsoxn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3lnhdgnbv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3vkziiqrm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3avgskzhz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3tmxcovqv.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3imhdrrta.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3pvabiwbr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3gqrcxqhs.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3lldbwjdk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ziovecdi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cdgnfoft.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3qchytxqd.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3kzyymdms.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3tlnaishe.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3btebaifo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3owlorqix.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3chmpoxkm.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3buuirywb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3kbairlaq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3kpcsrmws.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3xrblibxc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3gwyzsqss.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3zxkxblaf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3umcsflul.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tnktjduq.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3hvlidavd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3akrhbgnv.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3bgojsisp.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3gbamciwz.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3zmgdnnjk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3zaslitda.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3yrzobbhm.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hsooudzy.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bzievjzg.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3xhvjnvep.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3bgqhtvme.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3jzpxfamt.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3tytgiaxu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vzqixite.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3bclrehyu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3nhnjkfjs.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3nkoybovx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jfuohbpo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3lbmxbmdy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3jgabeela.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3drnrvzfm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3stczrugj.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zmqzabcg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3povgjmxm.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3azrostui.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3scubjerb.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ijhqpdzf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lnhmtgbd.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ccokozvh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3crlipehc.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ufngejve.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3crdsjedw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3keyuzbxk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3mroybksv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3dksmixkd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3abqrawrg.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ngtzottz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3yahtkvqa.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3emtjshit.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3kbsruvtu.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3hlmcsykt.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3kttysuce.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3amquqsdw.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3vsfaohqq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3smffgxcp.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3hntxyasg.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3fxnudvlh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3rwbobqvs.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3tvhogkmp.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3qyxojgbu.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3zlybarcq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3dtbvptaz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3fehfpmqp.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3bydvgwzc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3qtanwkjn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3svmxtnnm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3hkmczutn.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3gmfvzpxi.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3dghrbjva.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3xkovrisc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3qrcttqwv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3atmsghmy.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3wccwrcoc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3eeatpwug.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3imavaegz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ouhoxfsn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ewpneuyq.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3mjbnylht.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3hofsevno.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ejatelro.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3cqqnqzev.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3piuyhlot.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3jpvdhqfu.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3aomtoejt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3prsrifna.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3geircxle.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lspdyipa.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3kyhmzfky.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3fshhfrwq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qkqlmace.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3wvlqeykz.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ubnjrmdo.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3oscrlnmu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tbfgztps.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3xpmyjozu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3dvoioltb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ovlsyrzn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xzhaxekz.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3wrojqtcy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3caedmuie.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cjwwkhho.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3hixrlinh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3txyfugra.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3treinvrh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3nsifaayv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3qmvinyev.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3pbikpyib.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3dyopulyi.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3cfazvsev.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3bxghoqdh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3uzqpmsou.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3hbpdxykv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3vasvpsea.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pxclmnkv.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3tqbrvlpm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bbswdbno.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3crdtmshf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3kwnshtax.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3mgqggvan.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rjlfwtnz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ycctlvxq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3iujzafmq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3egyguhfd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3swmavdga.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3sdiiqafp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3lzqjwygq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3tpnvvtah.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3aplgrdww.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ttjijjqg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vlcinllx.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3vatjyatd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fulcjzkz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3bfjbrndr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3avygolje.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3scnvrwrs.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lhymwefu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ivapfpxt.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hzuebuhz.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3aytfkxdm.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3japxeqnt.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3mtmcpiwz.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3wysilptf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3emiihies.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3uxjfdzng.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3dyhokbfx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3coyljcnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3saosiiza.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3pqnoebba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ktlkylqi.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3orpznwyx.html


<!-- 参考信息 -->