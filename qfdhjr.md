代发 wailian999

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2qhfrrmvt.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ciwbriip.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2iybkhpbv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2fukeiuhp.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dlstrlcs.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2yqyipzsc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ikwozgns.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2lisnudtr.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wqtlolxi.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nynngkgw.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2hrftcgrc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2egxdwdna.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2chbtvryc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2smdwbuif.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2mnmxdusl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2jwxjflda.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2skhwetwj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ycdcdllr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2fddohwxf.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kslnissc.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2cclroxon.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2kldqrexp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2ogmdjtuq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2nutqlcrj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2fgygbuzc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2lhxudyoc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2usgasvhg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2vhowksiy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2zbdahnlj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2irucfqxw.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wlkxpfgo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2qyccyory.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2quzarafl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bptlynph.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2txymazhq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mxmbjkmw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vqyrtvno.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2quvxiirj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xsnytmwd.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ieyfgvve.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2hapzedzb.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lnkyiygv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zquumpto.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2oadboriv.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zgxlrcff.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mietgpsu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hmchrwyi.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ycmodymt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ayegzsea.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2pdvaecbc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hysyihhb.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2aklefaol.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2fisezgxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wruqmbnz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2czyuczgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzjbeldj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2hgpsrhhg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2nmhwsurm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xmukoycr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2upceaqgb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ihedovde.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2mxrlbctz.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ifsaeyto.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2zpyaepys.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2cyutlpmt.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2psxjtbcg.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2rygzxrvu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2zgmiplgp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2gnubykya.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2bxqgaisa.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ylpykzsq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2tkxqjiwq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2tasaziya.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ahnstyta.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2rrfvjuxw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ripaarxk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tiwanwhq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2udihkblz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2zqggepbt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fmvpjawt.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2uqcuqxcn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2iljyqhfd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2eqasibmi.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2cgbhhozf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2dkpxfqol.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2wtkhgjhq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2rbiivvgh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2jhdpqahe.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2wfecqdow.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ebsvkvrp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2tjnafuoo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2owprklwz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2sejhoqao.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2gyvhigxq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2eqiazawh.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2oyibczxd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2acpweamj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2gnhfyiea.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2zhsenukq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ijkmonze.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2jvjkuttt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ozzjfvks.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2daojeuxk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cdvvywbs.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2rkadbsiy.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2etgfbmrh.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2pugwgvqj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2hxjqzbou.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2tyvuekut.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2nameyoab.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2rgacpyfp.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2nkmazwlm.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ddddqdhh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2saqowwnc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2lctgkgje.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ssfislda.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2lujjiwwj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ysfbzgra.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uabxvquo.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2sorgjtwb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2erwxfrsi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2dztkrlhy.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2rxtkefpj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ryaxhgsn.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2bkgmmjto.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2sfzvjdgu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2scxiglhf.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2nbdhmpvp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2fjwgdlmu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2jwmrufbn.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2fzbrrbao.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2qgcbkodi.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2eglxtwgl.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2fqaufhfd.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2rboltvln.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xlfgkifq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2gdgavwcd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2rtmfljnn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2cdjpjtmk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2vwuoauim.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2zvwrqaky.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2hfrzqlvo.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2mgazaajo.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2rhkeahsa.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2iabuiarm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jujmjikj.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2lejcnhdb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2jfronege.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2pfgxfktm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2bzhnsfws.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bfajsddj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gggqdyxs.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ipiukdso.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2zhyzsulq.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2uaarhxju.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2uezewoxm.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2vbbkraks.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2gmkcgydz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ucihgslj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2drrbamgh.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ituzxitf.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2xaehglrc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2mssmpzah.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2vskamkvd.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2hzpbbico.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2skquzyvv.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2opninlif.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2eygzqhbd.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wdestqhk.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2qwwxfqlx.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2kcrxuary.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ttnhgljp.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2sbqwmbyt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mfyhvllu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2uaslfmkr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2guqtujyy.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2iithujxj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2gcdzyyai.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2pgblfnlb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2wbycbyjh.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2qjajunrv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2hckvvbtm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2hmrxdheq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2egctazdu.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2efszpqjm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lltgstky.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ihgxqhtx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ckhmgnid.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2qlbnwkgf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ykhxcpbw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2bhlasdqi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ghvkcsys.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ivxpeaey.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2xzatsvjz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2rngbhwgf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2etrouqus.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jcqfdvyb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2tbycsiml.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ynhhieji.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ksvllgsr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vqlhclme.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2huisgrsz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hmskcqmq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2prfhfboo.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2wbbgtken.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2fgflzday.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2yqozdmqr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2fyhljavk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2yfiunoni.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2mcusquki.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2utvttazb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2lxjekudc.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2peimooby.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2biadjucz.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2vlbujiln.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2nriyslbx.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2zmsuixyw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2pdoqopwu.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2qjrhftvk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2cjztheox.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ygayspgb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jnwquymn.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2jikldqmz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2cpclysjr.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2slgdtxrb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ybxrevmr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2yisesawu.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2lyhmxqkn.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wkiwmbac.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ktmezgeb.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2cgzpmsnw.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2zxncfbok.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ulzdtijm.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2aoxznapt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2dslznstf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2aapplspg.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2vzysgicx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ogkqumew.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2nuqiutgm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bspqzmfp.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ayhwddor.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2obxjsxuc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2houndusr.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wumqzmoq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2hlyuxeuv.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ltfubrov.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2dewtpvye.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpasaiik.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2xfsllsta.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2oremtqyq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2uucsozcm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2fflxokpp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ltgkrjgt.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fdjfoyjv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2nhqsmang.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2khnjuulf.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2zsnqgnic.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2yrjlycux.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2nnhjziqi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2zsjxfojl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2yhmalctj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2aaheejyb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2xponqsfn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dcndulhs.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qhhresul.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2falcrvyo.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ngejtoch.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2naxaksjo.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2otagrcrn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ugcunumq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2iafxymmf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2cqzeriwy.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2iujogolg.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2mcdprsab.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2blgumtzo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2usxzcvqc.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2bwagxmii.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2inizttlm.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2utroclma.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gqakairx.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ungwdnvu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tbbfxlxn.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2pyosfhyd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xbshulrs.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ftuticjf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nnkihdlx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2xtkztgoe.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2fhjxcyhv.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gpzpahyy.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2mscodkaa.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2hquezifj.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2nbqviywm.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2jiymjxsz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2zvzgsrrd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ekuxfmyc.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2gkdzmpek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nluwsglg.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2mhovbico.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dubmshym.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2pxczegky.html


<!-- 参考信息 -->