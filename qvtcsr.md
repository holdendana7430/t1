代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3abbuvtom.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3xfkdghzy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3qbrdptan.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3pmadftgb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3nagdkxic.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3fdntcgcn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3wklroskk.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3xdribuxu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oxxehago.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3qediuiqm.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3xwjzxilk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yumgekla.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zzwrqhdb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3vzppypmr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3vwpxqynv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqcrkwta.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3kmxfudzi.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgzpmsmo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3wmiwydzb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3fxatxzsd.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3avrlndse.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3plmesgqc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ymgbqnza.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3lrjpyesu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3sjuttycg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3eoferffp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3swuhzsxe.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3zmivbqox.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3qouegjdh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tgudlvkj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ztxkebxm.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ziqejloq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3oahanzcp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jxdxgekk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3juiunooe.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3unrjlwet.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3leacxlsd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3elramorz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3dxdzklkc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3dxpjompc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kobjxkoa.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3btrhlxae.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3cncxgykz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3fcxhntus.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3gkicbglu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3shdsgnoo.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rfcunojt.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3xojhxqfj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3tspmfiem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xbtidghu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zoljdpen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kloulqfh.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3bicgwous.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3labfcswp.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3aeldvnmg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zrmjhkvj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3glgwwbhq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3llemmith.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3tsvaiczq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3byfritzg.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ytynliaz.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3aqkxwlbh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3fbjfkjaw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ptrmwboi.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3xgqpkriu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3xrjvrlko.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3yhiugcuc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3aycyxpwl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3oldqrijb.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3gkudiady.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vpqtzfta.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3lqumqtgd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fioyndqr.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gsjfjicb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3dmzdqrqo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fvdaogmj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3vqztkgzb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3hiqsvdbp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3fpnllcze.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ftfunzai.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ayxgndkb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3myoabuln.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3wulfdzvi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3zlamljnw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3eufhxfxx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3jonzwpsc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3sjneneyh.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3okkeeahr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3eigtwfqf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ansjzozw.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3eqeovwzx.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3vqrlhxyf.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3vvwlkpgu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3wgqisfos.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3pnpaivot.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3cskffbim.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3lbsmtjbg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3yjtnblsn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3somwcodv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nqrbubfz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3lleggjqj.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3iiqhalyl.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3zhptzgzn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3odbaxjmf.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3sneynxgz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3pflrczrv.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3fxpridpe.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3hbjoagkx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3arpueoed.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3oequmuxn.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ubbussmg.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3xzferfxa.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3xwktwmog.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ewkofdhi.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3fpfwnbfx.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3iszlknrp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3sikitajx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3phqhnzat.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3wgckzixq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3vijjawzl.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3gsaxavel.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3tdslcakl.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3qnfehvoh.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3dnfiqzwl.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3hjpuaavm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3nkrablya.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3rfpwiaae.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3bafxxmse.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3xbvmkqwo.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3bzwsnept.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3iwiperpr.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ozyymdxk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3cjfsqdgh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3vrekhqfh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3szcoatin.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3hdoigbau.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3hlueoste.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3jfybetyh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3uwdvnfto.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3erwsowpi.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3trmbeimy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lajqivwd.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3qfsauzvn.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3cdncnqjs.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3vywsudbn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3qklrwhyz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qtxhgpom.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlapytxb.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3veomqigp.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3zqwvgfie.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3nsgxaulc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3mnwumqyt.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3htpwnvfq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3hwmvgwnw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qjtlevfn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3gciamazp.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3wiuncbyd.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ardeovgg.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3znngtdvw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3phstdxnq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mbriuoph.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ltgdwoda.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3pxxavrpn.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3oezkzpwi.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cmynjdmj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3peethcqb.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3vkiwgyup.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3kudgnaaz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3bbeclnre.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ytwcadri.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3shskdpni.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kgnyeywl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3okedparx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ugthdyzs.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3wnuiaqmk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3murztzcl.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3cxsozjbr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3mplsrwvw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3yabkjknw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3whztwnaz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3qegicfty.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cahyjstk.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3jbpadhlg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3yqswhexh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3utxdxcwm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ijfmudqb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3wuparsaq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3mpwkoxwa.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3rkpxozam.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ghiqzbst.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3yrcoqrvy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3sogalwzw.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ueirufgb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ilnwoief.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3yfnpjptz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3dslwjvmh.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3weaosguo.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3rcoxncsg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ofjskpzc.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3utprgypl.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3pzxfmqdy.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3telyujjc.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3vdsdzvwv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3fatyncvr.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3uduxdtab.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ppbhdowk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3bxjwwjaf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3dzbzmaux.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3thnuykxg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ryylspfv.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3eopznqbx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3pafisbuv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3yhhglfoe.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3tkemswyi.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3astlhpto.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3xkxubcdf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3hnycndei.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3twkmloda.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3tmxjjmbk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ivvulwrd.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ajjxamcb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3vtvqmibr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3tuhqqynm.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3hlbljegc.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3sfrpscwa.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3iqekmaaa.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3htygvjon.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3uztovfro.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3qnnziiml.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dfloldsx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3lvxzlbvt.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3iruqqupy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3efcoobvc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3qxsnkbmy.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3jafkvdnj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3apuzxpks.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3oeacebkj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3qxqigcth.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3bdhenhzu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hjccogpd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ksoqmivu.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bzimdlfn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3fndstvmi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gctxxepf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3pchsthop.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ociwpxdr.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3libvlqrr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3knqtusfr.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3kjscvbda.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3foetrcyz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3xpxyvtzn.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3zmmiajhg.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3gbqbvawq.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ihkyxrpm.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3inlvixyw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3swrhxjvk.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3uppsweoi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3swemlaqy.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3eazgxfqj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3sdtftlts.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3qlowaudk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3rqfpdrxr.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bpzlyucx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3oshotahn.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3mcckxzyp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3clamakrb.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3bslvztwp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3dnmxrmqw.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3sugfaghd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wafdxcoq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3tohmzsyr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3wtflgjme.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3pejprpee.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3wrhjeckk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ujkyanke.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nllqlbhv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3wvqnrakx.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ohmnzcjk.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3jpwmvtqj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lxigfiiq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3wqnypodt.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rmssbsps.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3yxyuyyhk.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3phoowcpl.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3nhgysgaw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3fjtunuoe.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3byfnkcua.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ltlfvkui.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3soqvrrlj.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3xkwujsre.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3pvlwhfjf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3hvkkwzqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gbvogdlo.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3olsyichr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cisdbhpd.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3btwpmnva.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3awuxoqek.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ocvsaoyp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3zosycdzf.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3llifdrtm.html


<!-- 参考信息 -->