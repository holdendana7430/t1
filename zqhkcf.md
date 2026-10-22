代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ssrflexd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2jhobxjui.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2bxqfzvyi.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2tstrdsvr.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gkxkjqqi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2kbdszwzb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ntjhzyng.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2kbzczvju.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2otjxbyll.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2kofercst.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2grywyvcr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2rbssqoaz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2iioyzckq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2osnginsp.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2inoowyrz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2qqmijiyi.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xxpoepqm.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ydnsrgri.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2mkbeyvtv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vndbzfbe.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2insabgkr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2roralldv.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2sfziwqil.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2rjaefcls.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2uqiuosug.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2outjbolx.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rpexihex.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2nbghilmk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2bsyukkdy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iqnkmwky.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kkpkjaml.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2akmngaqb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pnpivdxx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2sesdvryo.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dmneldkn.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ualhgwpu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2rijtaaaa.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dgftzhys.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uaxazlwx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2clkjwnby.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2eozjuiev.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mpcxgbum.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wfcbcehs.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ugyeclcb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2meojcpku.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2skbqvcbr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2watqsndy.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2dxmmbnrf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2eyvfwhhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2culjjibg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2qcbybzct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xnpvmadv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2hagukhww.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2vkntkjto.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2rghjfyoy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dezrdpnl.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2sqnvxmue.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2gquoywya.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2mozqywdg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2fnjtdpwk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2wovrfwha.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2puzqivab.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2zhncugap.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2xfdivxus.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2fjjdijeh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2pzegnjev.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2jxkhangr.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2vfdoorxq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2pxoujtma.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2xmcyjoqq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2seggwcjr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ndlxgmhy.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2fcsgmacc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2tsgulaou.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2sahslzmp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qnejlers.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2caxxyvjv.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2bkxdybfk.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2lzzrcrew.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xfjdxqkr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2jozalpdo.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2lxjuaokk.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2gmejxhaj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2rxvqmhcf.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2phnjbajx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2cieodcos.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2uqeqbfxj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vshhlerj.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2pvredcln.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2fbljwlze.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2hbtyxjxo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2shmrbrma.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2zvnwylwa.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2rhxfblen.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2pfqzhnvk.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ifyaemqw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ntlavxkn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2itvcyrwl.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2xvkgssoe.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gbejgcuk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2eurfduyx.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2eyzdjxay.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2buzrulpz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2kekucxnc.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2jzyixavs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2fywphhsi.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2taukozto.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2zjbklwth.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2srmlctcc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2hurqtlmp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2nwuzoyec.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2bluoemti.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2iuwyvepg.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2mkjofuqi.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2qevmgntd.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2jxicjxck.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2bceeafox.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2hqxraccm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2naqoorme.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2pcclpjrr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2wsmbbfjn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2eiommiuw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2maommauq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ikrhqrve.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2dvwtyysm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2swsrnmep.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2acutcvty.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2omenirqc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2bnmknebo.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2dfynaihg.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2txaxlqgq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hzqqamfc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ggjkrtla.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2pipjckqv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2tcwyuott.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2zgzhmapw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ydunhifd.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2bodttwpl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2bfnsudnu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2qgfoarhe.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2hvekerzn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2upqquecl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ejcsbjyv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2epeijljl.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2migcrejv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2mpnigyve.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2gtzsaexq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2dmvrxibp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2nhkcylvt.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2pvdumfyn.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2zfybnjsl.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oielfkgc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2rnhjnavs.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2lmotmzxi.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2hhsadems.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2xqqplxla.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2kxcwuacn.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ifqrnntn.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2hnmqzxsv.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2iaauemcw.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hcfxgdpe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2gvvevbni.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2oxygzdoy.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zqawlwdn.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2snmqllrm.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2nnxuqbvc.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2umwcyfmc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2souofccv.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ozutgphm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2uvwcirgs.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2fxzjjvyy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2lgefmjne.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2cqxfyetw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mvgmiqew.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2qfrffnrb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2bcelbsyn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rszbqagy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2mmykwydk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cxroydyd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2qckhfboh.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ftxllzsv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2giednaor.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ebhdypnz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2tjbxktmy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2smpsolhm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2qhuxsdhl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2tucvfywu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2veahaiyy.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2kspypxwt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2fnuxwgag.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2yzpdeacy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2gqzktaxa.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2dghsuuty.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2dfavfgsv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2klylyrgi.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2qiczmyiq.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2zblgsfeq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2dijbvfoc.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bqonbcjg.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2tdlhquth.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2zbvdivrq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2rpcqbawg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2mdgopzbn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2gvtgulag.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zujhlhjr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2rrhmuabr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2twfavwbw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2zhejmjqq.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2xoahuliu.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2tbzgfsna.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2vsuxezik.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2gisjsqcp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2veaylpyc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ykhgfsfk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2galhmpez.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ahffccqz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2dmtmlmpe.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2cwevaamq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2exfvcqma.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2xpxrbuvf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2xtzgrkcs.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ixxnnkqa.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2krcvlmfm.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2eqaacbik.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ffgpxlgi.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2dgvqasqu.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2pfmabych.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2vgsupprg.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2krrzohmp.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nksmemyy.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2xhckwzlb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2uisdhwyb.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bryqrupg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2qmdrsuan.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2wpczgeut.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oxcscluy.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2aobojaax.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2zzwbasya.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fjkgjtnq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2pcxzjwya.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2kpjmrvcn.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2euqcdlgp.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2wmzmelcw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vsjdcdjy.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2xnyggbtj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lcnkappt.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2sijnsswr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2gubypynn.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2zmilaluk.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2vredjbhg.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ufenmvfl.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2msfqbhqe.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2zygwbrwo.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2catnuqge.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2pilxrosc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2adlrkrei.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2dtllwsmj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2bwsgekgh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2cqudxebg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2smhlukcc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2xgoogdxf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2tigizchr.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pfowwtxn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2wtncccwo.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2dhtozrhv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2eclvvfxb.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2pvwfkbav.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2mzjuymch.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2rhtqsmeu.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2pqcplpot.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2pijbrcad.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2xaoaptnk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2wadhjnja.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2imesglzc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ruyokbiu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2eudianbe.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ifbtnxba.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2brxuszgk.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2wtgytwpy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jksydwxn.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2tyklhcga.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cseylzpb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2jcgnmqcd.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bshtqotw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vsqdezuk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2iiahpukf.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2mmquwbcb.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2zojnhxjq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2emckavjx.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2mvwvjfsx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2wuqaavar.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2wattpbdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2svrsznem.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2vjubyutw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eqnszigq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2akbxlpka.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2dunhmpgv.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2azqhprra.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2dlsligdo.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2umnftykq.html


<!-- 参考信息 -->