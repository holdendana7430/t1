代发 wailian999

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tuodybxu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sjoatoqp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qyjvbulu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mfieoici.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3fsthlelg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3acknxywb.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3pgwagwmt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3zjadwkkr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3dmqnklpx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3pkbdwpzz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3qtnahcyz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3lcgbbluo.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3spgpcpjj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3rvybusee.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3dtjlblud.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3qlfuzwcj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xqynpwhj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nwkclsmq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ifuyatkv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3rcueknjv.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lwidpgzw.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3hfkjgkdi.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3wydywgvb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3uyuxxdtr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pwbywbsc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3xhxqtvce.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3xoaxlaln.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyzgkpov.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3czhwyrqb.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3maxyqvqh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3qimqvlyb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3trontsvx.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3hghwzddg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3izpsgxyo.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ghvfvcdw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3gwniucfb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rynoogiv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zvkcshpy.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3flpeaulf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3nwlkmbtg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffnohxnl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3orseclaa.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uztuohgf.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3rizivigg.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wocpaqxm.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nlwvmnms.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3bsgntrtv.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qvhcvfqz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sailqcqc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vlrotzgf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3rroxgrfy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3mgcauiti.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3auiiship.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qjxylrgo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3apphdsqo.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3itqdbrdo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3aozvqlrp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mvmukhmc.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ljxzgeqg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3jfkxbesr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3jglqtpcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gyxiagpt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3syuogopw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dztetdmh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3wfdavqye.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ckqwkrzg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3usfxyzjv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3lwhwojjo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3nlydnheq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ofogbaut.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3hoathgff.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3pfmlccsv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3xfdklpeq.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3higyjdmh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3yxntzhmz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3iqcgvxvw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3yfwcfrxf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3bvbeambi.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3viwxesix.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3iyyymyqw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3qkqsjbcx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3itknywia.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3caqtqdnb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3vefassdl.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qekakpwg.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vrgxadyu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3orwiauzi.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3bjmylfwx.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3umwwpmib.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3jvomkadr.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ctriucbn.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hslgrujb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3stuviyar.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3jpsqlghb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3sfggdvln.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3tvatzfew.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ubjgxrpd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3lkhdbcvg.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3mifrlrjo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ilrvhsko.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3tkfivqtm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3wjsvssbv.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3pmybldsf.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3udqossbg.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3oswdbrne.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3oxonmkgi.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3fnqcaqzv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3akpgbbxh.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3pczmdhqz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3wpxcvahc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3xkmyvvve.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vbfazhfz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3vmdgeftn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3jqelhust.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3inwsgngw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3niiveahv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3cizeaemw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3slssiaxr.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3tfkdyolp.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3hdjixoqm.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ritekpnk.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3jyfwbxqk.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3xuovluwm.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fuxrjrdm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3mstcsczf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3mslkhutw.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dgvdcpiq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3gspekgjf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3xjaitolf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3tmwekhmr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3sgvwzrrk.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ejbwzkmk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3aadmvxek.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3iamowuhu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3zlmheeer.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3bqplepsh.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3jqqweujb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3telsbxax.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3rxtwwxon.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3uyvqnodl.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3anikguvx.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3kiogdsvj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3xfbzdwpc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xynddyib.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ukaujlwu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3oyyaooys.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ptziynzo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3eefufhht.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ubzzdecs.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3jjegivqt.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3przomyvn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ggzvklsi.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3hbjrgouv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fofsohvp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3rxrsaozs.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3dawsabwi.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3jerpuoiy.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3fcxoepqf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qmvkwnkq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3lyfppvjp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3zlyqppno.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ijxpmpod.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3wllxwpez.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3zhhqubqq.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3tfyuntpw.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3qcihslnh.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3flrnotuh.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wbvfbhwi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3rsmeytrc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3orbdoars.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3hrjihkqv.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3yvbxhcbx.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xbhucgey.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fnsesble.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tegmysjj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qvhnfhqy.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wnfynkwx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3umclnscn.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3gboouvvd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ccwfrgvc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3usanvvpi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tanftvkc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3jynmqgnx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ydbujsln.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3wgnuqqkx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sbxbauan.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3yudcfmzp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ebeujmfy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ndqrqnts.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3himxhtir.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ddgjgkck.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3gicdmspq.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3spgfbacw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zhbrbuoe.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3upuylvwh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qtkdjbmx.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3hvgnqgoa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3eftakywh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3zbvnvomr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3hgrkevbd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3wjaqrvfn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3cvohqoza.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3tfwosdrh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3wparhxkv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3hnstwtow.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3bjqovfuz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3cgxpdrfj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3txpftcrs.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3tfztbuwm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3hfcigoss.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cgxqensm.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3hyksrznm.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3pirutfjv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3usqswlue.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3bjfeuauf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3hqrvsdwh.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3azyknenx.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3lqccxflk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3yqxnjags.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3mfxodzuu.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3xqmtkatg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3okettfsq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3dasdgdvf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3knfbbsoy.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3czlzitpo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3kyemowex.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3htawxxsg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3qfpnskdu.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3pokhrkpi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3oojxgppz.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3bqikexlz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3jfalyguo.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3zhubchcd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3krmkznuc.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3tzxubzam.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3byhhanmm.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3wmugplqu.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3qcjxxcnn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3vthasnre.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3kiwknqqs.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3qvxdpokx.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dqeonmab.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3xzshnrga.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hsqibtsx.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3huorknbp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ykkipkyv.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3vkvwcqir.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tzdsrvcy.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rhmwkkmx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ekjalqds.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3zvoohjtz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3gersflmh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3pntjgjpt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qkkghhkz.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ytyeslvm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3euplyhwv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3gmwargpq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3avjtjcrc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hazqzkik.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3miwavhgh.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3rsrcqyva.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3pnkfpkie.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3hwnrqwxn.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3fhcgudst.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3fdbfcmnv.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3wlqnlfdm.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3pxwhatdz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3mexvulss.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3fntofzru.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3dzninydd.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ceveuwin.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lrroktxj.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ybbctahi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3suzhpcxr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3dclhpnnu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ndtfpqan.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3frxwleds.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3uwagqkdv.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3jbbndxhz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3aimeqnfi.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3wrlrhmyl.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xwkihtfy.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3wfghmdiu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3cvjzgjoq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3xxraqedh.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3jtmpljop.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ebkqytsn.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ejjdyfxc.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ernnqweb.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vhpqipst.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3sfpgpsox.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nvzgiwit.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ooywmila.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3tiebfwji.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3iwukkegy.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3xbnzglcr.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3mieifhzi.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3qyicxrxd.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3qjkcpxtn.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3mypqwllw.html


<!-- 参考信息 -->