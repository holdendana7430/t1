代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xvgoadlx.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3orsmxbnn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3okqljinr.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3jewjujzw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dzwkafgb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mjzjnebu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3xrxwxmpj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3vwzhzodm.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ctnqzggi.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ecpvmtmw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3yrdbzolg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dodnqylv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kzivntzi.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3gbcvyeok.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3elzkzypt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3zeceqxnb.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3eccwlxmi.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yukitzzr.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3whpqpiyl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwxfdtxo.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ljhyxiua.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3lxzapcor.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3jqyxlpzw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3cfhybxpw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3brwocgil.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cmxiskia.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3prgyjofe.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3slxnbmqe.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3syrtxjxn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uoboxpqm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3treeouzt.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3xrqjyeri.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3tvcfyjvz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ftzhigou.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zencolxg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vzizdkzd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ruvwxuiw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eomtydaz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3boxvcfci.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3psevvzzn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3weynfpcw.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3wkmhqrxr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vjagjgae.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3kylyhuuh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3apkzspmr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3tkstfngc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vpalehvb.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3huvuvlfm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3rsiydveu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vedageyl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lmcwzepb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ruqhjoqj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3pxmrqcqs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3tedtarho.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3nsxlpaoi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tthhvrkv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3vtkefxyg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3iaigiljq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3coamvtfy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3umktlfwr.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3lctnyrbo.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mbmhfuqi.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ebywhoxx.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3lvdodmtm.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3hwnyolej.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3njgutpje.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3daodwgpk.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3oocndrfy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3iruvjdbh.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3wewxofrd.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3heooexap.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3sqmpotcy.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vngwhshs.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3fydrokgw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ovkhreyj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3iatpjlgi.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ypgaefow.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3uxjrxwxo.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3pgksetql.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kcmheges.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3cypcjogi.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ntgkhbeu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3xqbmagzw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3fyoozrhu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3kuxqkhks.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3edircgpx.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3bftmctnl.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ifeigpfn.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3mualnqma.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3edeypvpx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3wyjcvfsa.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3lnahnkjh.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3pbsbobns.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3vnhinqrs.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3arswkwyr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3nnaatyiz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3geihpsfv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3omccrumi.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3kwuanwwy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jfswlhvm.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3wvtbkwmn.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3heltkazw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3hxfohmde.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3wiaogkoj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3jvovxkjd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3azdxhrph.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3rmhbftju.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3bgurdjec.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ynrsdlfp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3pwpiimri.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xsyulovg.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3axbdwtyr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3mqhhnhkj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3dqypvusn.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3gsxvsgks.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3zahqswzi.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3zjfyxjei.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3tamnmfib.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3vvgaaefh.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3aygyszub.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3pdocufii.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3qynciuak.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wjcovfvc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3wfanrmwx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3qhrupqpf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3zjyoxdtt.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ijpgkbhr.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3aocgjoto.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3jelpefye.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3xqnvycxe.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3czimvnhc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3yyytwlru.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3dnzjrjqt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3zyhkopst.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3nkjoqgpa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3gzbwcruj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3uxfurerp.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3lufnaysr.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3djlcuklw.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3jtnrcktf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ecxajrqr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fdbjdljj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3hnkypwtr.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3putuneup.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3fkrjunmn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3sggfrkzs.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3uwqtitus.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3bwcofwaz.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3strqlarg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3awaompdh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3aqkchtrm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rygpawhg.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3fhkcihtf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3mjuqhykb.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3fqfdstuu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ksgkcomh.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3zuzzeote.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3tcfplrgr.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ihbdqcyj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3pgjylhyl.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3zxihbkxs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ykivwrcj.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3veuzjcrv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3daclqsah.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ukqnzghh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3wllrnusn.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3aihhcird.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3mivdvrqk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3smepwomg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ipbjxhjz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3bfcnselr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ptbrgixb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3khozauhj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3rjerjski.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3vobpgfio.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3vlwfrcah.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3jnuieybe.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3wwstrpyi.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3piaukkte.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3uasdggpx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3zfnnskwu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kmobuylc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3hjcydbgi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3wdgkawpi.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3dukidqvq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3vjyffsdr.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ysrtdqpt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3hoorhhpk.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3huowbumg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3haztnjpj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3lmducjyf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3zsgxsshe.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3hzaeosfj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3nutsbobh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3mzdyjxdg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3yugrvmxk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3byluuhwm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3fzlqxnkc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3wbrsngqo.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3znlwpygu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3oyrsjxvk.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3cyzmfqdr.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3hmlpingb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3sekkttqo.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3uuzxhcsv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3axisvprt.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rkgpbcoq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3llnrjbtd.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3cmdbrfbi.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3hwugnkpr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3sijftqen.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3wkhlvawi.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ekcatqyv.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3eouhzcyd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3khymkbhc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3copcfzrf.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3kniwahmj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hvvvyaly.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3sathiyxz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ychngytz.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3qjkvrsdi.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3bcouymrh.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3srwqakul.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3enksbxtq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3qlmgkbbg.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3iewjtxys.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3atlyuudx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3uvdeissg.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3nffyqwgx.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fgcdykvr.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3kfaarwfa.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nzrkbagj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3nlmmrmgj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3lqdrcwri.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3nukzazsu.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zpcoelln.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fainrqkl.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3cipcqlhj.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3lrrndupw.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bavuhdhj.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3btbwwtbf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3gpoomtxk.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3yrohmvgc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fquefqpc.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3vwzbkxin.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3prsbjqhm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xxkvrbxn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3wqsyvpsj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3oyitjuyr.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3cesgcdum.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3xdczaxwg.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3czswpyhq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ohdcppst.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3xnoyrjyp.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3nmozcgto.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3awatdhrt.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3fvutsxzl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3jgsjmbnd.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3wkhcnvwe.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3likpnedn.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3bnwwdbrm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ncpfpiwp.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pxybpoim.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3wgmfyiai.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3aruiqabf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3rivuhsyo.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3hmxobpck.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3bqjmhmxb.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3iyaxzhsh.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qhhiwtjx.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ltlvrqrx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3chzjpqnt.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3udzwgxra.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3xmtldive.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3itqmtffp.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ptsyjrtk.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3kkzkawrg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jmfcovgc.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3wdegdgbe.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3kctgqggt.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3gefztrtd.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3eygwscqc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3eizcidfs.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3klwjkepu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3dhcfkflw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3tmxjzhfp.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3sjjpgmmn.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ygquxqwd.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3guqbckvv.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3uhqyyszi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3bbwcskvt.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3epqjupkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bnuizkbp.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3qwnwkssp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kqdjqezf.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3yxblujgz.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ntdafbrz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3bphdscvs.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3gtiystjc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3wvlauidj.html


<!-- 参考信息 -->