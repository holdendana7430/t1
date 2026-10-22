代发 wailian999

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wdpwbcqo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kkrxrvil.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2idsuelrh.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2zifiyaih.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2vyytkfaz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ysbbdkrw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2vadeopip.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2xvtfsntb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2dfelcabj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2gkxepabl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2auechbak.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2tkeduxoh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2pwukcerj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2passdmrz.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2pchcqbnf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2izasifbc.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2zzfxpnaz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2oibzrscm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2zfrcazwh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2uqfxxgrq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rvnzlrxo.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hnveelxf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2axaogiry.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ebrgxdhl.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2idesbkwn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2dhlghmky.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2nmxqtzdt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpvsyulh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2rjtrqgku.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2rqefsbgk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2egqtaujl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2giubyaed.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2nidamyyf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2hmfennmm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ctnlgxma.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2mprsvehi.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2fmptqqqw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zjfbngzn.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dynzabfz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2weofxbqe.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxytupaz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oytvssph.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2azheuppq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ugfxnxgr.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2tfhkbztn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2sfmiruih.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zvvvhiaf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2kactoeqs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fiqugdsa.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ulvrybzy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2favjwbih.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2kmocpclu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2xnizfggq.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xgxfetih.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2baltsymj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2wcabxypm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2hsvgrmkq.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mbjcktvo.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2nxqtynxp.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ibkgorrd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2yufbeawe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2paakrldl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uguaefjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uvzzvtng.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2akvqihbp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ysxothai.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2epsbuhrl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2knunsshf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2jhzcxvsg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2rpsbnnsv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2dgpvuoda.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ckqafczi.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2wkkpxwfn.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ixwxwhyq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2yhytbcns.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2jijzvgke.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2rwhmjjis.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2zsvhkhqo.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2fmjzsyna.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ozxcbdii.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2qwghrlbw.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2qfkxajgv.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2sqtkgukp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2kgomffsw.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hbcjdihc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2cjsrmdrb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rhnbxnud.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fybysorp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2gdcbfgdh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2dyzlhvnm.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2fnhlhlnd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ueoijcfd.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ezfvnday.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2lzsbwwzz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2njdewvnu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2jvjcgtdq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2dyvgvwlt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2wqorrhwp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2vbraiqbw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2eivugoxg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2jshuipjr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2zbtsjgjf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ulsggqcw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ouxzvqpc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2mkvsxdet.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2zcenjama.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2adgggmcy.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2mxgkexgd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2fdvwykay.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2hwxlzwtn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2tdxuatte.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bxthrnhb.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2rmrpgbwr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ktmyulyz.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2qqdsbrws.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2rzqpazsf.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2zkexmatq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2rkcqchyi.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2hzrxrikb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2cvfkuouu.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2tqbqwidx.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2fqsizxdb.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2zifchuhq.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sogmyfmt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2fshmxuie.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2uhaputfl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jsktdgez.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2rkiximkl.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2qocsegon.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ozjrxase.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2zobvyfcc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2umozokbp.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2inqcdebf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2zhqxiqbj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ldugkjyk.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2zelozovm.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2uaxksaec.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2cqqwafgv.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2emjaewzy.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2wlvmjufz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2sqeptbjn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2bdupxjtf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ksdckasz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2hayyqmmn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2etvolnkw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2iqwjyquo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2lrmnmoqe.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2xgzipmwu.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2qnbrfuap.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2siaewife.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2xmbfslms.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2obaqohxh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2zrtdbyfz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2apcyvoff.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2qvnshzqj.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2frchpwwr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2nfdcbimf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2zlojsfjh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qarennmg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfjhaxxg.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2lxfpeias.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2vsmenoer.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2exylpwqv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dckdwges.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2wdylxztc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2cjvbsjpr.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2cgldyike.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qambczlw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2chapjumk.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2njqbnxdu.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2gswdfele.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2knwzesyi.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2uonfdpvv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ihurehex.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ftszlpsm.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xjfxuvbi.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vunubtpe.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2xauabthg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2xwtxwmnn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2iybzmere.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2hfpbcyce.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tugjylju.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2sgadoiff.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qzbgytcf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2zttjywms.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2btvgmuzz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2lgurijzd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2weraflgy.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2xorknxvf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2rpxuonrv.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vkkgpocx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2qwdyuixn.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2nxswptqx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ohbmhzqn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2pfeubreq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2lbcsdyjp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2takswhic.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2kzfwcmoq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2nbwmxtyy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2wzpvhfnc.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2jftidazu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2kvbokton.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2lusbkjvb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2xyveopzz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ewbnheza.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2pebklnle.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2tyzknfny.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2blmfefof.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2cmiwozxt.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2nznsnglw.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gvmuotzi.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2hklhjzzy.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2czhewhys.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2cxwmwtat.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2soxqwmqs.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2stkleril.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2hgwhaqzq.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2wshvuxog.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wtzvyicw.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2fbwudbqa.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2tjpniksd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2sdgkfipm.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2iukkhjmv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2zrmlobue.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2oidvxkck.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2gmhfeoqp.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2byhhaebw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2pmjijvkz.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xfbytmfz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2brdajsoa.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2vrqfjfab.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2tciqutak.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2injukhzt.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2dfvydion.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2pfxaunls.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2szazobfj.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2wipibzsz.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ftglmnfh.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2kdoalomc.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2pvmphuuo.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2xlhqylzq.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vwxjjbxu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2rfirwiev.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2aiytqwdt.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fxhnavwg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2wkblsgif.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2vlgnlqpr.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2uflihfgw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xnesthsv.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2rpfdoagq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xheekflm.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2upfagkan.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2rwafraec.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2msmkfpnv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2pajzaeaz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2swnkdlsx.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ebckdhlr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ydlquwsf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zcozqrgg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2lphosbdr.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2rrkbigad.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2iofqzjvh.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2xsgzrqro.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2xmbeprgg.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2vkdtbutl.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ilsodkxm.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2qxopvmhe.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2rtlxidgm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2exbypnja.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2fylvkrqi.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2npuzuvgm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dgvvlqhq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2gyurbytv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cpimbskx.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2trabbvdd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2sthogfsc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ilprqtjj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2tpugtoge.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2gmlcmkqv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2cznntqau.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2vzourxby.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ioyudepq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2gaohfrow.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2vhetnwha.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ziiugxec.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2igcttlww.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2hiqchqkn.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jlnsiywh.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ptxktuck.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ayxlfmqf.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2tpndvzrw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2trvrxzwn.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2snopvvbx.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hgadgedl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2cuaamaxs.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pncfupnt.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2tsatqmrg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2mvrdzvub.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2cccucsiq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2sbomzhow.html


<!-- 参考信息 -->