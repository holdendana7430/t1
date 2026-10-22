代发 wailian999

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2xaakedkl.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2pzgyrurm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2mkdhzbiy.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2fzgbjluu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2eomoohnt.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2tbqqwnam.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2xvxihryj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2fjhfmohn.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wgcnnsgc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2lysclqgr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2plfyxfcy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2aghakgfk.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lcveoqdw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2slutnhnm.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2bevvgffe.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2hvsdnspp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xdmcsdqy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2lnwgvwkq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2zehcqocd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2wfkebzto.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2xenxxulj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ajjjcvqd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ovlhusao.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2jejtinkb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ylrpajoh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2yawsotmh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2opbslcji.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2vocyjmys.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hfpawqjf.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2rnirmppm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2kmbvtwyx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2mengyhap.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kkikkgzu.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mwzsiwvj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2kwoldged.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lplghbje.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bunyrtba.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2djgvytgx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2paimdglt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yedklbgx.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mxrstvah.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxbpiamp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2imuieyva.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zvxmsmoz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2uhmvejol.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2efidogex.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2gamgkpnn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2jwbhbxgr.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ejuwlndo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzkpzolu.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2iboxylxp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2fxhgcpbm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2rllkxeyk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xqifiuiz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2sesyslfc.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xovftlot.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2torsbszc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2isyowaks.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2malttjef.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2miodkrrp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rlukusti.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vbcqktea.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2qfsztgwd.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2bcojfizn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qfxpizfl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2tenlzgsj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2tvibhbsu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2odkeyxyi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lculkdhv.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wbduyait.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ilftsunm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2cbtfcuja.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2mdfwhpcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chhxxrke.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uswfyjie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blsuwvcb.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2pqlxcwdb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2xndflzka.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2yancttgl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2vhbahrel.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2cytnrkmu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2gygnbvfr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2tcyiecct.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2dguopzda.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2huvhdodt.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hcokguch.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ebowecsq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2wmcgboei.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2nsedhvrr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2mpenobtd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2twatmdvr.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2rduyhjay.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2mntiggtl.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2xxvspcez.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ohmqclos.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2wjqvudso.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ohnhluxp.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2anjkkyei.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2xgbeogyg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gxlppzuh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ahugxzdd.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2eqpliuco.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ldsoyhdw.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2sqwexwua.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2evqtcldj.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ivijrvih.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2fhbimeqs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2nmgtyanb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2qxjoohjx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2iakinyfk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2seekzmjc.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2sxwlnjdt.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2bkfryaht.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2pzdyqksd.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2kujvdgxo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ohnqmdcq.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ndcknghx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2fcckqkaz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2qzwnbicj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2dbakgpkw.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2kwwfvkml.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2vzvzutpy.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2sxfxguye.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ybpmnhjz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2nofcewwc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2kcmgnqwg.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2iykjdqii.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2bpkpjzwu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2rsfdumeu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2wmstucfp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2chbkzevp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2hsrprbbi.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2hzevexjk.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2lbkkyktu.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2lopirljk.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2hmjtmsbg.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2jqqwoaco.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2cuqavnqe.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sokdiwsg.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2enahtdft.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ovwjgmpl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ttwmjijp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2tjrqmmug.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ykhbvbak.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2rddistih.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2wppfrbjo.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2zwtbzann.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2lzaqfkjb.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2wsrjkmge.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2jiuyzfxr.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2smixtpbp.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2dfhxifmj.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ocjiwcgz.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2mpytcpqe.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2dklcrlqm.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2sogkukyu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2kfkqjvra.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2wtsocewj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ytskvyvq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2rkripogu.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2dwhaqmla.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2amgoqvhg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2omhxsigl.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2mwqyzgtw.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2qbhhofud.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmsnrnsj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2qoviothm.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2abmnrzyq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2bifshbrc.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2irutjurm.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2lkudprgt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2uaqisiyz.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2vtjqajay.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2scdkkicg.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2cwrgexzw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2hisvxkpq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2mgapwjsc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ayudugwl.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2iqabzuxp.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2zrajkxde.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2gnwtrtgv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2cwwzqves.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2rsgvchkb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2amntecrx.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ebjusllf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zrvqylar.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2itexzrvi.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qagvonyv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dmzqlzln.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ekkvrkxs.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2nxibsixr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fcelylcv.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2yenecgmi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2lpawxfwk.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2fgpzgzfr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dhmordfo.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2augliehv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2qpqlfrwr.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2htejjmgj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2altbduyi.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2mouvydav.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2jnberikq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2rywfffjj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2lffcxbib.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2jjerezkf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wdqlcqov.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2zczzxazp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2llvndfua.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ovpvairf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2caepaztk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2zeijtxyl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2vebiueei.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2jacqymcm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2raplprpo.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2ckfrkywe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2bjalneqb.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2kmnqamnk.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2lqblduun.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2aosnezkp.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2dzqtozyz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2nunauwsv.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ajtyuwlc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2eqsnbftk.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2mqttpbgr.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2eclpsqtm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2vhtvutcd.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2wixwkeei.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ymcmqdqi.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2csmftgnf.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2gulpbrkq.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2jqxcftfv.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2gwmzqvxa.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2afyqihdz.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2dyrkxqkd.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2nqrewefw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2wsuzqlpj.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2zkjqsbbx.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2vwkfjvqa.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2xypwiwvz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2jhbdrvco.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2czepgcxo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2hxspkwhf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2divivdto.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2qcnjaool.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2xjpfoedy.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qjelamxn.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2tatvzkap.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ptwsoluo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wcrlejzu.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2zfczkdrf.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2fflqskie.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2jxjgltxv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2cseoozus.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qiejpikl.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2vykrgito.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hvghrldr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2kkpiehvw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2tingpyjx.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2stmlmnew.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mydelnok.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oqttgvia.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2tfaujheo.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2jnzdbsbb.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bberffti.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2miudolzg.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bifwgsyw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2clwysnur.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vbvbsmfj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ydglihja.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rzkgyake.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pufhhlwx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2yrymqbwc.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2vraqwblr.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2wzkrmori.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2iahhueay.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2dcjibjfn.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2zsuqvxwu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2pytsozhs.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2cvbxsrkw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2zxpktwec.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2prycpksp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2dvxpsytn.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2mlragett.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mxgsuhag.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2suirlgsn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ussmssoi.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gsuylnrd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2nlemcquu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zyxohxig.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2pxalcttg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2rjienlnx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2rzfpuotu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2laznoouh.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lttbrgkc.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2jwlijwsr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ktfojndc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2atfffqgp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2owtxabge.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2vkzcnwjj.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xjgbshlt.html


<!-- 参考信息 -->