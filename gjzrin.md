代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2yeexesnm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2zsfsazwk.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2jrnsrmbq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2yddalczu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wwrmljgi.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ouviljpr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ekfoxrbb.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ajflsfth.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xbliimaj.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2mykqkyda.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2nptqaxyd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2fabokzyt.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nypyrsla.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ywfdnfhk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2jgrmghef.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkpujuhw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ukuiktwf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqxgmdze.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2vbnvmzzi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pglejjbd.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2yjiluouu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxjlkyxd.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ugblyvke.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2cmjkbhhf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xybizzmg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bjjlwdkv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2odfoizmy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2wwbsthhx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2qwyhfvef.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iwgptldr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dqyqhhqq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bzzcfcnk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wksekndj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2aetburar.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2oagxmysq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ykerpnit.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ruuezatu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2tusebukk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rrtpbfvt.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zinqxjgj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gqkbscaj.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pjrwdpno.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xzbkxkdo.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2hertgxns.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pamjmnth.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gpidczsr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dmycvdzk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ycdonlgo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2zwiuzazq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uuoihknj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gkghzeri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sisvfsml.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2jqlxfbuy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2nlvrnxaa.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2cebdqucx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2bhfhdxso.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2szhsgvjp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ffbixwqq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2vzxbscrp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2nmosvnuh.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2scsimuny.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2elijuqvi.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2lnrhtawl.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2kzbykhgt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2dlgojvmp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2aegkzikj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2jpkixfdm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2wzxpvrng.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ixqhxqmr.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2rszatzcw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2wjvtgpmn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2kxsejzwq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2slaxmefu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2dukbncbj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2qwqraljm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2dayeexfk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2izoiudtc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2dbnantum.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2faspxsgt.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2daihrbyj.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2pmnmveto.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2vluplxph.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2vxetrrxk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2lymkmhwr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2eyrvcmqi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2llmfdgho.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2enlsdmkz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cyldggpu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2zumbkmtm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2lernjswl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2aytyqvlj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ahgocsav.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2vtuegolg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ciclgvku.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ghbqqtxs.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2cwkpnsmq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2fbskxwqf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2dbwzojsp.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2suioizog.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wjaoatfj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2atncbfty.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2oqltunxw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2bbqsyudr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2onryitky.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2mxzgkase.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2fwgwdddf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2fyhpxugk.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2dhsrnjnl.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2ktnjonuk.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2yheeowty.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2cfsujrhm.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2xifgpdyk.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2lrqimdwc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2whxlqojc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zxrfbilf.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2mgyzvtyj.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2qtkrwsfy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2uuogcqiu.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2rmyymgrh.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2uilmgvlu.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ppygqfbc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2hbipeihx.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2rmdazanv.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2gejnwbdg.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2qxjnwozl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2aljsjqhn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2gukdqxzk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ibjkbusi.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2zishuusp.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2cvgizecl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2zuykbnas.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2vhuphioo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2cenzfstq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2zbqpbdoq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2izqujrqx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2llbxefrm.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mzrlxnug.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2udrgptyi.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2xkjaiulh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2xiieipfq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2nzunjqts.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ippuupjo.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2jdzvzwrp.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2lqpwclss.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2tdkipotz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2bmyosnaa.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2tjbanbxq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxllbfsf.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2drifopru.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2umtjxjmy.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2xxzhuqhd.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2hpysslqs.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ykweegzs.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2kjuiujqt.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2dffjgcrq.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2lilpozea.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2faanxtlt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2sctmdxjl.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2qkfgbugg.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2yaxsflrj.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2dgsxvtsm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2qkelcjcn.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ruceosoz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dthtczul.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bhxwnhnk.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2zzigwhja.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2omhuryvt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zrkrjnnr.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2bhsgeqgy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zbpgcbdh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2renknhlg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2pmcwnwsm.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ljyouxjs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rgvdrrza.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2lfqzxjox.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2xuouaupy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2dwvmugmg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lwtniuma.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2odbiqnvf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ywikhxrr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2xlhwuxht.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eddxsfzi.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ieuhqbpl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wohzucwj.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2eepobxfe.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2scacoybe.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2bpakpfjl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2hqijcwkv.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2gkdfstdj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2kqcmizhe.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2bzexzjpa.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2egyslmbp.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ikadjfmk.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2qhafajof.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2mdrpszyb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2rbwjxxfb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wqlmhjvl.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2gjruenja.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qxhocrdi.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2zcfbedsh.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2mzswxkje.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2goejhkxg.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2lnapxuvr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2kgrimgji.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2sdaqwwsj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2uygxfpwy.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gtqpkmiu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2gvgoxait.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2qakaowan.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2qltxnhrq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2kjsrgwej.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2flyxsnam.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2pzdsmruu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2kycjdeht.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2naddckhg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2daiwlngy.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2soedjnft.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2eythkihv.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2xfypxlij.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2tsdgxezz.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2cbmczjlx.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2lbapgoqz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2xafrfzps.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2usjdggwo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wewmvqqn.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2efmgilal.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2envsavcm.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2nwewlfwf.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2hhyljdne.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pwhkoeom.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2wsmimlva.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rsbgzufz.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2bbwfzilt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2aruowzsm.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kshsgenk.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2higscipl.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mgwljtvx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2qyvdfdtl.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2mkollpsv.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2voiaxsob.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2clgpaawj.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2tnbjxnrk.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2wjyvmiqs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fxocfhvw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2laeupohv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2icxkftjv.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2izdvmdhq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ybttxqwg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2levyewun.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2pxdrqafn.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2iytyvepa.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2vjqiocze.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2vcirtxtx.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2nlgjmwis.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ltazpsju.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2cwiszmvn.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2rccltrbu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ckoeayfx.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2nznjlcrr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mjfnbiko.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2fezfriof.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2svqzqfkr.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zisqoyuw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2mesgcjcc.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2unjdmsqk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2unmukuoo.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2nrgeorsy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2kzfnlwlc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2hngyydqe.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jdasdfzh.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2vozhckys.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2isagcfws.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2nkicumik.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2mcynyczq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2aguceftc.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2noqieuhc.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2jxhveqdh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lzniukir.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2twmrdqrb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2srjcxwlp.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2fdukyerb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zxlnimrh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2tnocqhec.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pbwgittg.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fgainrqp.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2segvfugk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2ynhgtaev.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2cjnhtwha.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2dvqlzmvz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2lslrcxzy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2kxnoruaw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2mbgbiwpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qpxbrfsk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2aijvcinm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2guzwwndy.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2fpblfgpk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2opjszlqq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2vsyxxbop.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ptsnwbmi.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2olvnvywh.html


<!-- 参考信息 -->