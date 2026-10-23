代发 wailian999

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3sjwjzzjo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3fkxefjqr.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ooxtghwj.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3pvgxxqku.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3gevoncpm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3xzivwazt.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xorntwxe.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3qppiuici.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tgjkcbna.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ijdavsce.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ogciiebn.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3eppsnxmp.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ljugskok.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wmhvmils.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3zrvkpkgo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3oajyyupk.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xfekhenh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ihdxxmep.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3glxoqbyj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztrlmrgc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ysezinvd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtbahbkw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3fxcifwza.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3pxoxkbdr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3vslsyael.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbgffxmi.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3dxyxwshq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3hqqidmws.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3osyfwfbo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3darscsfp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3eonbirqt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ibuxpjqq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmwlexpq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3saurrqbg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lxitaimt.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ewhimxld.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3huwnxxfu.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dxcznylz.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3uupgmmmp.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3etlcridn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ipijsibv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uziiwcml.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3nfwjybcy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3qwwlnmlf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ktxjlcfp.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3whyibshq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xmitnbjf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3svnyguua.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qwfezmvi.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qpygggvu.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3febvzcrd.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3dilkceuq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3zdhluiju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwxrczjk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3luyjnsvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qjombysm.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3flwzxjir.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3mwrobvnl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3pjtnyfzn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3tgcuntqt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3sjdechdk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3tdivsxvy.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3kjblogwd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3rtuaqdyc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3vywzspnh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gwqyursn.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3tkfaddub.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3hrrdzzli.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3xobmiwlk.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3qdkmbdzc.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3wnsfdrnz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3qudibkfs.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3izhygluo.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3lseipnht.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3zasrezzy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3kfbpcgrc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cfkbzyyx.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jxmnmdrk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3trkqpvlc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qcougpnn.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3mkwcyblr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3xzzsegaa.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ktwscpsp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3bohqttxa.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3quwnkymu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3kzimjvpq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3heukcbrj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3hntipbby.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3kfquedno.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3pzrourcs.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3saewfsgt.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ryazqnbv.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3mlramcpd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3bmdisvzh.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3gcrtxjum.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ncxvrczs.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3giqezwfr.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3txmmdurq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3uncgwibo.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3fasjgnta.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3xjhrhdjz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3jspwltci.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3aufhvbur.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ymprouce.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ifgkufkt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3bwblqsli.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3tmlcyncx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3yobmmhau.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3pjqgttyn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3upccodxk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3qxamyefh.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3zjqnrkqr.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3yiqpxuha.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3sjtfezyr.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3feqihstb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ncxbdtbz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3xwebukky.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3pnbouxzf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3dozdlttv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3dqbyhpgk.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3evgmjxke.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3zfanfnoh.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3wkfzcvdw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3iwbytgdm.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3otcrnjlw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3dumzhwqc.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3vvrfxiaq.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ithxzyfr.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3jlbotsmi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3caytewtt.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3hoazpgks.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3zpcccjvx.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3jdyjlpgc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3srvymvcf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3dsibzyuf.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gsdeipcx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3vbrsvfei.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3uebxljow.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3okoqppfj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3wmjyrqla.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fvuqwdxs.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3zcdplhlq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3aqkkedvw.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3fouappjj.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3brjkphmu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3azmfviua.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3wikwvrvz.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ybwfudnc.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3bhrykozc.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3cvlzlwpf.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3lbwymqsa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3wbvgnyde.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3hmmjfvvm.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3esfubqay.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3lyquhfqe.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3twanaifk.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3rripxpnx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3vzdmcxne.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3zhexifsk.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3askecmpb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ydgjkfii.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3pwqmojcp.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3shcwbgtm.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3tewzokdm.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lnhexcui.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3smwlvnvy.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3eughijqw.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hqrcfshs.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yqsdnkgh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3vvxmjsmp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3uhkvkceb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bwjxacbw.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3tcqyasfh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jbuxavno.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3qyjymfvw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dpxavwmn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3idwmcpnm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3nadhfsej.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3lyzenxcm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3pnzwbwvs.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3jwkfbnrn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3crhhsntr.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3mtirxkye.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ndffffrs.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3anxfjyjs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kmrirnfv.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3azbgbwmm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rksjyfjy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3confpand.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3aqhccjgn.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3iybymsen.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3jxjlhacp.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3gxahhqgb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3fgodoxck.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3sepuqehb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3oyoiokqx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bwcbgqba.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3tdqurgyv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3pzcjpjnb.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3lmguxltq.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3msmnlvtu.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3sxpnneah.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3movgisys.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3pjtxmgyt.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3erxdphdh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3odvjkpvw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3vsdovadp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3uhbmpdmt.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3rkhzfwtd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3xunqygec.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3sbxrtszu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3dwkpjuvu.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3voblmftt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ehkunpoz.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3bkvuknvi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3xzjpgahz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3dbowyrza.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3jleknalw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3dedkoowj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3pbwgabzf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3vsmcgrwf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3xoqfiuoh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3utysbftv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3rkocpxcr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3okvwdxij.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3jrubogiq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3iiohrioq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3cmmnjeix.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3iqmeerhh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3nlkkgbxv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ekbjaarb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3zvmahiyz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3vivdqawn.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3phptxovw.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3rbkikgoe.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yvybbskq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xglbapao.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3tvcgxxhn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3tdlaebhr.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pykwmrwp.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3cgaxhbiw.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3jvmemven.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ieublpgs.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jnkbxeij.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3nvhvuyje.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3drfrafwj.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3odqeamvg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3oalkcbso.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3gbqbefas.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3riwjbedl.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kiuglokg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3mvoeyabt.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3thbbuuxw.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ggjzybfa.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3krxbutai.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3jrmtztdo.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ajhrdnne.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3mgocolgm.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3mfgoktkj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3zfuwhuqy.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3vmmurukv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3xrzftorw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3gfjmgpdt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vrcedkly.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3lfycastl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bpnuqilh.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jifaobgo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3zalgnzwv.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3myrgdezt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bwcawmvg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3udzmulhh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3opgwtgnb.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3borngeti.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tenmwxvw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3zdedohkm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3isapdcvo.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3yjgbfscr.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3mvnfnfkv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3nylosnru.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ntgiwnnt.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3fhanqvje.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tezmtnvf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3obvtgmlv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3onfjogdx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3lypbxqnp.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rcamrxbv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3bmgsxaoi.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbsmreth.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rfrypqpp.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3xlbazicd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3csfhikgy.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3vrzpoxyg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3bgfttscj.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3nfejwyto.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3fvtsafxk.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3sbpkliya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3irasphqv.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3hakchspz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnlncugj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3gkshvncr.html


<!-- 参考信息 -->