代发 wailian999

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3acfknrod.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lfnawtnt.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gdcuamwa.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ycmlfoje.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3aruwmnrt.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3mcgdluzc.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3hhlrbirn.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3uewaueek.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cnhoansy.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fnrucshr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3htromfyf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3uwmkwufe.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xqguywro.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ztdumzxl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3pedetfqk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bbsfepce.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jvvzedbp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3sziicasc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ejonvxxv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3azetxuqj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xteaxali.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3shwvpcjm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3jmeppyol.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkdoankf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3dgzpurwo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3gardwxaj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3bsjybjib.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3btmarzie.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3nfwxghhh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxfenxjm.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kghwwyul.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3qymscstl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgpzpuhq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3voqwmdex.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3awlvkxvo.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wbdazysh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3iyhmzkvi.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3inksxpnk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3yzyqgcjd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3evpjkmqh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3omzelyim.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ibhlwsia.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qgfihmqg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3sschxwra.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3rfmaudic.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3zlxzxyuy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hlwcddhf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3vqkmnbev.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3mhyyaojp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xggdivoy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tqbldrsl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3qhkejeqd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3gptolwuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkcejfuu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pfloajgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aofwlhod.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3dghurgvv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3jwzpwfbp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3wzbvypjl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3bbhgpexu.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3zoltygrc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3fbebmpwy.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3yaidugyl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3raucsuzp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3hlhcvmwi.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pwhbeoyo.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ntfibwpw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3pfumdves.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3cydaypez.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3afyppfzq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3vhtjihuw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3dtlydxnh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3qlyzqmes.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xulodedx.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3rdnsfivr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3aljzkufz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uiyimyna.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3psnewvqn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3biwmmsth.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rmjdgnom.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3tdvhqtkt.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3xkryfask.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3kfwripwm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3htbrampq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3rlpxthbl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3rljkghzy.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ciadxzlj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3bqmbndex.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3lzdxhghw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3taobfmte.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3uzyqyokf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3audmrfla.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3kofaemop.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3zdfsoeyt.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3vsjbkgbo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3cwrwisip.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3fpcwdpsn.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3jrpvxbdu.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3mtynirek.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3twbqgowl.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3kanltszj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3cciwzbyi.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3alnggxtb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mpdriwvn.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3tvxxbbjy.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ndbelsal.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3xxatkbzh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3lhffldug.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3mfwlngze.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3lmyxregc.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3yskfxiac.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3giahyjad.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3kxlxouwq.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3miwgkpxc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ipopmtzx.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3xxfxapxn.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3jiqhmirz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3bdtdzkuf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rjgxizzt.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3hhldeznl.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3higvtphn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ecxonxfp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3fxgbkmwl.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3qlkjefzg.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3cqspylcc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3fohmmrgo.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wjtlgszm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3mvkhrydf.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ovvsnzyh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ldtcogvz.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3wcsuaabj.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3bozcdgfm.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3yhmivutz.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3hpcrptij.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3arywvyyz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3cecyyvtp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3kmfaevao.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3akqrfpal.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3rpzvfpiv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3dvqtwgpr.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xgumacoz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3xrnkjgfl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3sxjdflna.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3zemseqyv.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3tkkbcvyi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jxcngnwe.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3wpwzcrza.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3etmzltpo.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3igpshyol.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3cvhdpqcn.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3wehsutdy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3csypclyv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3dobmnlvp.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3exbwnnki.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3znlusfyc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ezngfmre.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3flveydao.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3aavdqqzh.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qlhworiv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3zfpabbjo.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3fmupyfdc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3tsyjjlss.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3vyxkcddi.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3anmjcvid.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3alfbqaps.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fscwheus.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3brxjduya.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ezlivwwl.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xjtiotes.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3minnoegu.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ycofpjuk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3djoflpvg.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3lzerhtcl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lcbrkrxg.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3erebmemc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bnmyhccm.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3lzgkqwmz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3uoedbkpf.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3wzdsjhui.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3odgdqlaf.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3eskuvufd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3nlfplbfn.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ocijwqqo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3bvtbdyjs.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3mrrmaaev.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tjcuxzay.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3fazljkzj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rowuacnx.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3injpylcq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ofhrnwil.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3shdjwrap.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3sjquxfmd.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3vssudtot.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3iqgnibol.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3asotndun.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3vecifdis.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3lyicnkoa.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3waiycrqr.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3iakfmgqq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3anufakrf.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3loloevhk.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3tkaouylh.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3dieujrbd.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3kvcykysi.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3cavmuyyl.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3wrbgfgns.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3sdeoaimo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3poiuppti.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3nousuyfx.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3lrwgpvss.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3zbdaygnr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3cllbcqfg.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3umeedywl.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3mtspsuwk.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3utunsvuu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3yjczmavf.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ruafzaxh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3zbvfbayu.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3xmkocqwo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3tmenfwye.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3umgcgxnv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3csptarxn.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ttlwsryg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3uiqgkuow.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3yvnjjtea.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3uigvmotb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3fzcmlgph.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3rhltipbe.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3vkdpogza.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3mymspnvt.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3jmgnrumo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3awgdcoei.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3fqlnbpzg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3chofdakz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3cydphope.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lzqkemjp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pulbjipe.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3jybflvzi.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3moqnomkh.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vhrsegnz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3isxrmldf.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3lvrrdlji.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wwbkqfol.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mdhtxutp.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3annfbtep.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3qvqevegg.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3rcqadxtw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3hlbixudn.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ylklfopf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dyfygyjr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lduqntne.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3twxqdfgw.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3uswsjezy.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3vzvzolkp.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ielbhklc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3xcvrlsde.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3qbudhcms.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ulvnjpcc.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ynupucib.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3dmoikefw.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3hojtgxun.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3yokmgzcr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3mwhmkcdw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3sgzgnyit.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3pwzazdpj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3nsfkwznb.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wkcsvmcr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3zbegeuqk.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3crfuqvnk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3hrbjjxhw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3rhstplwb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3pgdeznjy.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3rvcnozib.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ykcbixlm.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3xeemrwhf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3gdnmdkia.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3exujhuja.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3jijtbsrw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3aebnhiex.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ojobytal.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3qsyhtskx.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bxrtvgyl.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3fjjblgos.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3nnjbpdax.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3yeqqikpi.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3erzftlfq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3idypdmac.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzecqbkv.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3spvtudan.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ozuszmqh.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3avypexuk.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3vgdbsaoi.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3qwfbyubm.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3wtxhbdjt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3jomzasfe.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ssnxukjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rdcamwez.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3zgpqizqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxwhmdzn.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3sntqzihm.html


<!-- 参考信息 -->