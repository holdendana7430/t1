代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3gqqpkhkj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3snhqqjrs.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wdrnumkb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3inlidckr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3wxbpuiyj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3syatyrri.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3wynbqvil.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3crnwqhwc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mpqwlyxu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3lhcehpke.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3pmmcijzt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ehwwckqd.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3leypofth.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3nvbqzing.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3hhkflewn.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ufdugmbo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3iyrvmxsk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ewnmzkkq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ogeuhsud.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwrggagl.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3urjecvef.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3wccmuhtj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3cifhlhrv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ihbyubyv.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uxmzpwpb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgaztpmm.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xvhumupl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3upbjswxb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwpnooon.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ntrnjfds.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wysjtrrf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ywcssndl.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hweqxeth.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xyxmxyyh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ldybkgck.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3icaljjrh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ekvjowkp.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zwwrhomm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3cdsnilap.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3cxpigqtr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wpcybeso.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dcrvkiqi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ntlkttdk.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3tkilxmuv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3zqgumimk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3eijwavvf.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3usjttusf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ebrjjyrf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3oitxhyhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tkfyckfs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ycplvmve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkantdlf.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3gnhzrnpy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3moooctnj.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3kmeivdrw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nbkpqkbq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3pmpanepo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3tbkxrwpl.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3bndndali.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3coizlzgy.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3zfvypgzg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nfuwxuyc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3dnuppqxb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3mrubevgu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3suczmzqe.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3dsbaikru.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ydqvygli.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3obbyinun.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3xwnrskrw.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3popmsubj.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3cunrdnbd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3fjhufogf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rakqeaon.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3tssrvhlt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3clktrazg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fmngjlej.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3igyhurhp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3bxssakii.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3urijqzkz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dqfayzip.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3zfbdfmgz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3rgdokfom.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3hwctdygf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3bnjbfrhh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3vleerguy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3wfaazqlp.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3fawibgca.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vamxrnmn.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3cdwxohdo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ybmjippl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3asxadfwy.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3epbebqwk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3zpytnqrt.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3lnfhesws.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ncyysvwu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3btruxniy.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3jaeewmjb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3vryktldt.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3qnoydhhj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zzvllbmh.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3qybpraco.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3wiywtque.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3cnxowasp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3oolhjiap.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3qumneqhq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3fkwrxxsz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3oaaojenn.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3pgdnizpt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3skfsatuu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3mebekowt.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ioljhqti.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3njqtedrq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ipbrwgox.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3taaagdrv.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3esolrrsk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3hhbnsyth.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3adamktzj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3efixvihr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3xhyhtncs.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3chzgxodc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3xprywhgx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3uqnqhgcu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3lzbjuujg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3kytilhbe.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3stdtmwlk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3mmgrsbhk.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3hlyxpuip.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3msejwksx.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3feekcrlc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3cqiflnzm.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3gohztpzq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3lzmvtshl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ywlmbeln.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3aetlqedt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3eubxrwkl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3lcyavqqp.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mibpwxvz.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3laldqrpk.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3waijanaw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3umimdihr.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3drkyscfc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gnbockqq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3hxjzygff.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3shuzacyz.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3wrnklfxa.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3cuunpczf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ngasmwfn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsfzxzwe.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3etnezwng.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3hzzlmobh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3srgfowdu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3tepflwwv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3atneilus.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3qktzatzr.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3fdxptpub.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ufelnedp.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3hjhuqpvh.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3qnzqinom.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3wmdeuymj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3zgrdmczn.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gdmtizim.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3vpndlmwl.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3gvkxauws.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3krcswryr.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xzkzztwz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3jjywivoa.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3xzueebgh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3nrdwzpzx.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3hhqfwsww.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3spuwdabt.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3yribnpor.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3hutckogo.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3dtudbyvu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3orhcxttw.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3tsdsfwsr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3iwdxrcuo.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3xfnjrepl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3usywngkk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3xggmrlpk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3uorzypcr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3nbnmkjhj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3osibchrl.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3iuedimia.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3dugmevnm.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ybfmkbpj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3krgphdtc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3rtqewpof.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3uaaszjfx.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3qtooieac.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3lxtuddjg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3mokksmbq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3qlayfdsl.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3vsxwozcu.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3gydoomkw.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3wfhyjuob.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3nkxcpkgz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3rmfqlwxv.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3hllvqgxc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nubauggq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3dqlpowib.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3cojshrqx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ipkcpkwy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3popssxor.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3oyabtnhp.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3lqlqegyi.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3fzfvoqom.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3nrrwsizd.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ioiaiftv.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3blkkedvv.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ulheqhex.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ztonccdr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3zmsnlygy.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3iopfzntx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ilrkpwbj.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3waogvyal.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3gyhuyqdi.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3dxdhhyrm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ymllfizo.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3gzyhjyih.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3kbtdwwbj.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ximbhxwg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3myojmnzi.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3qqbvwbmc.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3latmyuib.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3oqgmagga.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3jghdqasc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3daauemtu.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ruhmrovk.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3sbcglhkg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3peffvjea.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3jiommqfx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lljfrigp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fqykmbma.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3kaxcinde.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3wovnnvpp.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jwqnxdzc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3hrvhodrv.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3rieryyyi.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jrrdfsdd.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vzlgdegw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ekmpbayl.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3vvyueapn.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3jecffjlz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnidylyk.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3zrtnoolx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jabaccok.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3wlfixthp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3vdowcpsa.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3celqsnzl.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3vyoejtxr.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3wflvumtj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3xsrwgsnt.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3sletagxw.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3vdkigjqv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3xowhyeme.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3vxhxvzxw.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3eflxnmot.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3tynkszou.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ndbfhvfk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ivlthsdc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3wlfzlpny.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3whdgdfpn.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kraapoka.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3jeefazov.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3obkabgys.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3irncgzrz.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3bergrkeb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3yqcoyvyg.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3byejcbjs.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3sziywukj.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3omjkfgaj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3lurebizy.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cotmoxyh.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ksfsncar.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3opijpsfk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ecfklbuz.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3vesoohxt.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jjoyjlmj.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3xgumytna.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3trftukkg.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3laozxqny.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vfvjdbrr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3xxizkpxj.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ziypdtip.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3donrsmii.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ubfgvgef.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3hbofanpq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3vvqamfnc.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3larsremw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3kezwfczq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3cbqscjjk.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3kvflxnnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ddnhjgis.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3qndaqree.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aniktiwi.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3qabujzbo.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3cgpbhaaz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3lcunacau.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3umyoblks.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pzviccrj.html


<!-- 参考信息 -->