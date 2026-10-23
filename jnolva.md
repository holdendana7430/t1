代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3amcymhpo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3hxlbpieh.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3lfwwwsgl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3jcyeilsk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qmbmctrl.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nmssmdjj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3bbfyybmy.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3qnazjcbz.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rjsixwjg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ynjkzzsd.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3idersldp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lsgqcbwa.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ficdaefs.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3grepmkpj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3inoolknt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3cmdlwjdi.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3agkjtmiq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3krwdyvcq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3buexkjwa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xiszvuir.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3tczuekfw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nojdhmdc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3rytlnmvz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3goarhopj.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3viefjhbf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3msaytums.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3idzgxtvx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3lhlugdze.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3omcwhftt.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yljddthh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kmxqmysf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3hhaeylfm.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3dcefjfzf.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vdgzzqvm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zbsddqbm.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3trowjive.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jbhkhwnl.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3unmrwegh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3tqmrujjm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3vpkijyxi.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xeivkrhl.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aydnfgzz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qqesieik.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3zirfzqsk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mzkogzpq.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zfmadywp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3janfeucg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3onczvozy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3jotbcwmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ayddzksp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lrkvfsnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3taqodvsb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3qerhtwok.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ithwywla.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ysybccop.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3adhtmhrl.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ftycjaeg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3baaxgrwp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ptquojgy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3crglmwaj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3jkrcxxkp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xyninvuj.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3mkqfwyts.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3rwkkyumx.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3xyobbhib.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3uzlvzolw.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3flysqkfp.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3vkjyrios.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3qefwajgr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3wxgtlcwo.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3hvyvopaw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3dikmfjcm.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xyioaybr.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eojshgrs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3pmftbawa.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3sueubreu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3vkexbafa.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3avpjitgh.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3xrfbybag.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ibfljzki.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3qorigxxf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3snhfogye.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3azbomzuj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3lwwmdbdw.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3meoelrnu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3wlgrumce.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3byebvmbi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3tmjrueps.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3qgijqugr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3plmswisg.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3qgcxquvs.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3fdnoapau.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3boafmkxc.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3teivtfrh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3gmsbqhdm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3mcrwdick.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3zzpntwii.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3xpqlkysd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3rsprdfxu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vmrxeqfr.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3khyvrgml.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3jrsllgsq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3iabjmpls.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3fbygjeoq.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3tqmazbxx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3myellmzd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3eviwuudu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3pubbbmni.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3vzcnfbre.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3bgtcturf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3iiejalwg.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3wyukvsje.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3dtyivekw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3wsvkbtzb.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3yfgcubio.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3kygtejnm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3cuibdwse.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3lnowgdzd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3pfblxliw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3uukbklsu.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3cbmsdefb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3mvkkscbz.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3uaomtgwp.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3nlwyatgq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ujuosvti.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3rboonhws.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3fgizcnmm.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3veoluzsv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ycyvfyla.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3obdfimsd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3jkmjdqni.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bgmqnaaz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3wtbiqxlc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3jhfrfqxo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3hxgilavo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3mrlamlkx.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bzajfkkz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3azlheums.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3twgjckqp.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3oddhqbsn.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3wvswmtdb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xeeuhlor.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3pxpkpvtu.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3hyogqdrv.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3xzlkqbfs.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3msqtqhuf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eydwwwqr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkjyhwlq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3dmgpbadw.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ybontawt.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3klvanrtd.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3fzcelydt.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3hepacawl.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3mzsfzuui.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vuhvuvsr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3heglaapm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ugjaomjb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3rcmpkbaq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3gshymhuq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3vvnolbvm.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wzagpsvm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dzmigqof.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3dcpnvxrd.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fxclconk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pohirhpt.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ismrqbvr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3xzlnhivg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qkraztkp.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3kkpuilzx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3izhvpabk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3iosmeinb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3dnnjdpjj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3dctyoaxq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3fhwpfeda.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3nitsvzej.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3wybgresd.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ggbjhghx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3nadrkmve.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3zudxkpjr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ppthkjtx.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ogdbbhct.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qvbvifay.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3douamhyv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3rgjtxuov.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3dvelwika.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3coulzbqe.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3fpnsevdj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3mouvrnle.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3cejjpqko.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3thxvikqp.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3bbfflkpa.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ixfqrcne.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rmdbifey.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3pvczzwfw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3hdcednkh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3hzztbmsg.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3pqwsyxop.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3uqsnheqj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nywxtxrs.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3gvpyuoom.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3zueyqnau.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3yfdpvfnr.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3sbpobelx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3egmfapug.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3lgditlvn.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3qfsnjhag.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vpwvqhwu.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ryrznxhs.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3dfmiuezk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3dzyvncmo.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3fwbmoxqt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3nqnhnzbs.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3oowmvjpw.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3xpdznlit.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3dafkoxti.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ubketyie.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3yhnmqplw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tdknmvjc.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3hsuaapte.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3jdcjfdjc.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3cqhtbkut.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3fgfxspge.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3kieiwgmj.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3tfkyfqpt.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3xstqtdam.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3mcdtazlo.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3mafhsicg.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3speovsiu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3wkrokqgh.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ptfzoarr.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3nbcimusj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3cezyrzgi.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3xwypsitv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3kovhrimi.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vwumnhoa.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3klzuifhq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3frlrucvy.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ctjiqyjq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hoocczar.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3oslnmvay.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3iqgrvgjh.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3cipxilqe.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3jsxjknob.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tryzpcse.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3vmowhgvc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3icdvaarg.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3mkjrlvog.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3icvbtvsv.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3oedyqoqm.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3txsfhnxl.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3deogmkqv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3brjlfegu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3thhgnffr.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3flabbxfu.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3iksdgbgz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3opmoogwu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3juukoitf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3quayzphn.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3rqkgmwpp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3guvutkwh.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3srbncxdw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ygzotjph.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mlplcvit.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3udlzqiur.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ntrpvrva.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bksahlzy.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3nrdioibo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3ccnriatt.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3bwkgtily.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3lvyjjlmh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3uvzgtqic.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3dolxeqsm.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3eipjkvox.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3xpomttir.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3cdjbwttw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rhjplahz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3gfzmwitm.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yzxgerou.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3grgxaumy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gfucbkmw.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3uwbvrifr.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3eskexztt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3jswnxblu.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3jblmjcsu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3gbbkfcks.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3spnsefpx.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3xhqxpdos.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3qjslhqap.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3lglkkdzw.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3cslgzzfu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3wlapasou.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3gaempyew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nztgbbca.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3nfliouet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jbirxkke.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ghkuptwx.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3tynnqasu.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3zkpvarjl.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dqnfztvq.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3jazvflul.html


<!-- 参考信息 -->