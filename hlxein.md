代发 wailian999

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2uysbygzv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2miwylmdg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2wybygmfc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2dcdzbqwj.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2anrbqpwa.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mfvdfnoy.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2qplxzqly.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2tixdkufj.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ufbjzich.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2yhlimyia.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wdnvjdrw.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2nxfjpowv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2sdkiyexs.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ekprounk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2wozjakof.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2cyakbzje.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kcxuhvcc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2wdjewmtd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xmfrjijd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kqoekaip.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pdyfvess.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ygooyiwu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2wfqdtvom.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2opzkducy.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bvnqsgfs.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2mxrjvgwk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2hlkoiado.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2vdukjoib.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2gozatikr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qutmvalq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2uhijyiag.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2anrlmqzu.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2gxxedkkv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkyewvxc.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2boavjcen.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2wuovhiwi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wiyxhyyk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2alkiumda.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fgvhjsdz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2zxowgznz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2vpnwhxdm.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qawjblrj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2uljwrapk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2kacnswlk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2jazgjmuz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uydaoxsf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2mmrjbnmv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2bwggzxkt.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dsnvchxh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2anofasgc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ezrnuyyt.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2wsebnlrm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2mocyyvww.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qwadcsik.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kxoaomng.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ozapsplk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2lqnrdorv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukustday.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kthnirss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sefpvmfs.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2eftokxwx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ayyyhszf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2vbulezrf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mvkpefji.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2fcwzhiez.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2dmbqinud.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2yyfyluqp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2xzwuxusn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2shouglox.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2droaprbn.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2dcsrredk.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2cyvlwfzz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2gfepjavo.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2gzckxruc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2jkhcxmol.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ybhbwzmg.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2juwndbgz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2vwcebtld.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ovzsaorl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2efwnzgav.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2olepuwuu.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jqrjunsv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ogdbrpxz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2gtoxflvq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2fmphvyal.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2mhthjetj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2coepodyz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2nkfyzuuz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2dwfqahnn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2phpttkfo.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2lbyhpwej.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2jrxbyrjo.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2tsrkngmf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2nqaqhvux.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2xvnnykvp.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ootcezvz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2oalqcube.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2xigturjp.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2cssctgas.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2vpuklrnm.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2eggeyanj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2oettewwy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2neaxhevu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2wzioresd.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2hcuxyrql.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2idhsblfn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2hfgdnfsi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kproclbr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2iqzqsmgl.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2fhyjuioq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2oxjfzolo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2mbbnuwwt.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2htggtric.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2szlxcaot.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2kamicbjz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2plpwljuz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2vzsjendw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2qagftqph.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2puuenrnu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2mrsmmaew.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2tqlyfezs.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2kwtqwsae.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2dbiwygeh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2fvmtbxcw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2bczeorfv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2hlrstncr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2uqolnhrw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2uzrcfgsh.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2rfkborwd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2sbeteucb.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2oponvpim.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2beramsre.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2uigxajdi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2yylbpngb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2xwijojea.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2xnrpjtud.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2bsjvdnpn.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2pwrmsera.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2sgpahnoq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2gtorljzv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2qmhtnzda.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2rovgxnwv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2eztkezya.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2mrjxgplx.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2aqomenka.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2zzwkhumc.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2swdojahj.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2kipiwkei.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2mmyvkrrm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkmzovlz.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ixnlssre.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2kwjdmbkg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2vxngouqh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2pnqiefhm.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2putjyhni.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulxrbhvk.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2fujzbusd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2yjnfmmqb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2uhhxfrbz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlqnxygy.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2cdhbxbyc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2mkhnqdyj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ebvtmswa.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2bexgsgvi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2alcjqhyy.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2xoeromsc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2rxsnvxeb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2qwrixrdq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xzcxlpri.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ayjkleeu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2whjiulwm.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wnjluuen.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2odrwvqfs.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ykludvai.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2yahetlud.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2zcmsvoyi.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2nadxcdcx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pvbxvqnd.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2tlnxjcaw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vficgycs.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2vhpgqnln.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2upuqlhxd.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2bwazgsrm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2pcvnawta.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2hezfibtr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2qmurnupa.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rnmotwhq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2pfvlilcg.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2cpohitaj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hhhbsrva.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2fytnwcrc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2gcxuznoe.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2fhozzmhr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2nyqjhxsc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2fszaktcl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2jzmuktxd.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2hodzihpt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2gxbyzknz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2rseaxmtb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2tfvesnry.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2lqpfvdnj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2cmhbwvve.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2xmbgsmht.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2xfhfztcj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2tupzjjyi.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ifaobuzg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wogtvkvg.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2aczlsptt.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2xvugjxje.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2nxbwxcaq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2wqkycgxr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2wekjuwfj.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2zmnctsfs.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2urvoixhy.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2njhpmhfy.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2jxlazzmx.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2fxuccbxt.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2xcvkbyzt.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2zxetnbin.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2kvaojndj.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2goxtjaey.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ckksdhly.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2algyupim.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ednutjtk.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2gqeufzui.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jftfjpfv.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2tazyywzl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2znlimmhu.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2meslqiry.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2nndtdvfa.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2zwshxmue.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2zbowvmsi.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2bfdtutqn.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ianhejcq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ohqexqbw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2oyoyfnbu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2mypickia.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2glcfvpuo.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2qewtknxw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ybwkkqtm.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hsykxmag.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2cykoivzl.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hybudxbw.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2idxwdhpu.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wclzkptg.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2eiccynoe.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ikxwwwwr.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zvqipdmi.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2ywyuhfpg.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2zwqgvuqk.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2wuuyaaxc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kqkqwobp.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2csjwlmnt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cwtxnyyb.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cuqawrph.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2bvyplnze.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2wheljdzw.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2nublmure.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2cpgvlzkv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2lzlzqeqh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2zzxdoxiz.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2yeqwxthh.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2bdetwqgr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2knqddhwr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2kuexjgof.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2rpyasoxm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2whujzgap.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xhfaacch.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2sctfirye.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2nehfegck.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hrfzilrf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2rwkomike.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2lxdciecx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2gawwjzsw.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2szaksict.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2tzjdxuxo.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2hhogoyby.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2sxctjzxa.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2jahidftz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2cdlucyle.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2usdqevdd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2zjunzuaz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2damwukte.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ukzqugfg.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2rmhxuoyo.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zomeeakm.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ycmwokgf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ridasujk.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2hfjdbuiu.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2uvojvmhi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2xspagfix.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpvkapec.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2hbkesvxr.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2tfgtteud.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2szbcczcr.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2tgvqvoyq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2vjfulmac.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2rxdrnukg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2zkunqjgt.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2bebedpyi.html


<!-- 参考信息 -->