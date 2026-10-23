代发 wailian999

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ucffqoiq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3rmplwyqh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3khgrawhz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3aqfgkwid.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3rllzpiis.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3oeeycylh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3flrgmdgh.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3dzvjkbkc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3lbfogfvf.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3xbqtmkuq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wocovmst.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3avxrlivy.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wkazfona.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qdohkybq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3irjqcozh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3hmnfwcoc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dbmmfoyb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vvlyyggv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3brxpgmnj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3khmoufgi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3anampzql.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3akxxwprz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3szlktdzl.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gyrlfjoq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3cfnrvlzx.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3pvvposaj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ojyhjliz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iblurfsz.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3hlfqhgva.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgxhcwap.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3fljzoazq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ekjgjznq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ulropqbe.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3padwptjl.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mdwlzglo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3smqpkjmt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3psgwxblu.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3eriwdavt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3txdidwdz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kdtnkhjo.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ihaiuovo.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hanjxduy.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wkvhggan.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3tgimdmua.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fqahhrdo.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3oxjqufkw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3retnycua.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3opdwilpm.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wylmefvv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dopocxmb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jxhaftpp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ghwrwtmp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3eiadvibz.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pdzlzpxa.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pcbrnwuk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3zwcjndqb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3oxngdhgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvkrrwgg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3czielvut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3niwywpzi.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3khcaslcc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3tzwvrvkt.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3pyghvyba.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hjrcwbmy.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3urchkedr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3dbwrdgfw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3lqpzhomb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3iimxfvyw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3unvkvdni.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iexkohqa.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3gxdoehzf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3xtqdiekp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3nfkceljx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3rhiimhda.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3esohokrp.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3cbqqnfid.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3gqrekyru.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3icsihtjg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3dfkmzivb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3xixaeoce.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ytjigxxx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3jlchjrhu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3gkaawisc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3whbcntdj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ntnpekkg.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3cdekkhxu.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3bkqxgeds.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3xytnluvu.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3wxvxccww.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3uvrovcop.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3mcnncehp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3sysozjyn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ucmxmznp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3tvwmlqmv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3bmkwtyiy.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3rjgxlgqt.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3iuthrpcu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3wmfaucuf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3vgqtfpeq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3famneovu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3czrrmmoh.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ivlecltn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3hfyzsluy.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3yksowcny.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3oxyqveir.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3vkheefbf.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3mynyjqvt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lcosbpnh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ypceqgve.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3tkdylmzx.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3emvhyity.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ctrmukqz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3lxfdhssw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3vdzyermz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3wziaefgg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ehsuscyt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3wkbjysnm.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ueqkwchu.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3wxjppnez.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3wttwuoqa.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3tbrmmeun.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ilsdwtpv.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gyeexuwo.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3qgogkgwp.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3kpkgoxhy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3isezfjay.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3znixmbey.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3tprsjouv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3pogpmgwl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3irqgkwbm.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3qdvtrmyj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3tciylxkt.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3shxydrgm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ppogohbi.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3xjtgfwec.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ilkrkfqv.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3xjiuvdrg.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3thffwjzq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3aftewmvn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3drrzczka.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3irbozylr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3nmfuslwf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3keszvhdr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3pouxcibu.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wudpkhxf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3djlcnzct.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3nkzjidyz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3lyqbtjpd.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ubjoqmft.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3klhrmtqc.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3znsbmdvu.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3abkuhoaq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3wzkxpvvv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3qqdbunaz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bfjeczgp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3xwmutxvi.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3oztsvziv.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3huyjollf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3imenwvze.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndenreys.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3lmopgxrv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ebxlccjg.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3aesmevqb.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3qydoqkcy.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3njehpaad.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3lrfbxqhk.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3vawgkksp.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3rlvvwftq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3okhlezdy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3yciqqwqo.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mgwmmeuc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rnvnxdnu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wyncuchd.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3qzkygasy.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ulniieov.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vcbogtud.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ruzvfmnc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3digwhfwt.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3udwothsw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3gxrcvxgy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3emlstuhx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3eodervgx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3sknhwdgn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3zjhoxwzc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3nvffimfz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3egaqbziu.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3afctodai.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3mgudqyxt.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3necioaha.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kigqxdli.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ojrxhnrw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3azinqdgs.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3gdnakmwz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3lifknqne.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3rcpjxbid.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3nwnozruz.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3gqpzeexf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3snuasfwk.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jwglcqck.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3eyoznoer.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3dgvcwgvz.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3lukntuvl.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3smvqlyxz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3vhqenuik.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3kfwmufnr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3szqiismi.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qddjeiax.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3qyjgckqu.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3egmmltoa.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ryehqcrx.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3tyuxfvfg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ilkxkuig.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ybwwgmpl.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3wismcbdq.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qwnjbgys.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ccnjkvmr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3npepiaxl.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3vatgfpmj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3dygxpijo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3rdkiprhe.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3vrgsbpok.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3xngznmuy.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3szghhzxo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3xhlpappv.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3dwdlfgyb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3smesoqbr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3srhryxol.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3tjdzypiz.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3akwodpzf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3bmuavkyy.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3pgrvcida.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3fmlakllb.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3rxtjsxpx.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3bavyrjxe.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3azqogtqb.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3duqxejmj.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3rlafnbzc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vdzyfiml.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3qdqxoknb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3plzmqaaa.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3kaqylcnu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3yvsehrjz.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hhuriusm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zrtfhmcc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3gdhspysv.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3vwvqjuym.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3xvefbmjf.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3trsffcpu.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3gfymxvgj.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3lzclykpm.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3upwpoarn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jwgsvpxc.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3pddbxhdd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3soajuris.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3hfxhkysj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3sfcutvqk.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3hymkruxu.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3skyjjpwk.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ikohvhya.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3hxhttxbv.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3scfketlb.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3jukdoiva.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3auwdkwca.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3mmjmcilu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ojkdyceg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3svusqtdk.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3mgykavqt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nnvlnkyc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3xjveteqo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3kgerfyvr.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3faffltgo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3osvjadlk.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xbkbcsnj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3soafhghi.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3knlekuxy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3djceqzug.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3bnxdrxfg.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qaqnnqnh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ufrrlqgv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3hcycqjbs.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3uegfgrnf.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3wudlemdq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3mwevyfvk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3smbkvjif.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3furrunqt.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ojfgvfpx.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3mqcgdxrs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dojjtaxe.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3whayqepe.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rtduhqtx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3aefgcbau.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3epcaxzrv.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3auutaiox.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3zgnnmchh.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3wdemvwec.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3kouyhjxf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3sdvggfbc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3wshzibvv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3lxqgmawd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3simwmmhp.html


<!-- 参考信息 -->