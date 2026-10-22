代发 wailian999

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2odmvovov.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2gvannszz.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2hgxvmpqe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2liyitegp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2nafsjiob.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2eigxncna.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vfplznjr.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2mtwhttyh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hrzljqlo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2njebmjek.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2daeyaeoc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2tvcdrxca.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jefpkfzg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2sqtxwgpi.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2tjyfntdc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2igyltcvw.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rpivlvtf.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2mkrrffmm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ujtljpfn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ogiewaao.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jqjivsrf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2xyyyskqd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2epvtqdep.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2gclxsuhe.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vyqbizsa.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2cdedkile.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2qhfldlcd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2iyixwsxt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2pxibbris.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ygxsclqw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ixekfpaf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2nxvkxuow.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wyewyjww.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ydftgvky.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uzlkclet.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ucnprmka.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlajzwhm.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hpdjltak.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zkwszthg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2iqfclbig.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ftowpgpe.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mgqmbcwn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2tckociqe.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hthcpojf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rklqewwd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hsgtdsqn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2fyqlfova.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2egcijxdg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gxgwkkgb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kxfsmxoq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2unpnpuly.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ygedwvpe.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2zbueadqr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2wdkmibdz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rzjaqrdm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2wngdmhes.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2smxnhvwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ayekzmwl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2upokggty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgmtrnjq.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2qvuhdtrt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2mebnyelk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2hupxoqyw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2btdetseb.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2amhriqwh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2uxlhtsiy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2rtqsovaw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ubuxsksd.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ubimpdjb.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yntmibhn.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2gjrmitrp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xbydcnsu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2leezahko.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2jjyezrmy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2qnbkeejo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2nwwinarv.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2amhjpfeq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2jsnmjmqx.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2zdfrgvhd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2dnjkvepo.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qoglzbmp.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fnhwllmf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2fmxauzvc.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2nrjtvptx.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2evkdauti.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2junokbtp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2jiwtlbjy.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hvycewzs.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2anyjxral.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2gwareoeq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2mjrwfklj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2dtxwsmfh.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2rqbxwoim.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2vgkfwtks.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2wncbrsps.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mxhqzcjf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2foxfhgce.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2falteogb.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2eafzjclv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2glzdufoa.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ilfsxlkt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2kaffjmju.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2chaovgwm.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2pvinmdzv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vycbdguq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2uscoqyyo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2xemptuwb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2alpkmwnr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2edmhrffw.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2hkeetbxo.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2wnysyoxo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2qmsivgff.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2mwztvxig.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2gbsaxvbh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2fzuzwpad.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2xynmpkts.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2pctpfvnr.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2rxqbwgau.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hlayipdy.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2bdmouskr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2sltmqkpc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2uhhwamlt.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2fsbmsdcc.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2chucpllh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2jtjjwihy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2cejqdiem.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2jwoqltam.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2icevtssy.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2houiinnq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2dkhfqsdm.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2vsxqfvjo.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2pnavzkgn.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2fwghktoz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2mpmddgtl.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2hztwccns.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2wmpdqech.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2hpbckaap.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2gtnvndbl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2dovocxlz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2uxmetyqd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2yngtaifx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2wmkikwlm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2khjhnsfu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ydvzydlp.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qwgtuian.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2zaufgzfo.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2foupqnyg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2lgjrtvax.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2jzsleepi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaogvqos.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2hzidzscm.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2lrqwjsqj.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2libkclhy.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2fkzizghs.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2okqcsmxp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2qgxkjfab.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ckqgqlwg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2npkousok.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2vmtcejyz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2twdflrku.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ighuvdos.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2pxnhyhkf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2pknekyfh.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2kabyhdjm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2tpdletnl.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2hhpzplqo.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2cneztplm.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2hudxvowy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jmekqysc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2nesduedz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2bpwkmopz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qdnqhhoj.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hyjhiaww.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2lcxklxak.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ikgwykac.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2lszxoyfk.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2epumbbya.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2crzwoygp.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2dkuvuwlr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2zbgwxwdw.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2fpdlihhq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bgqcuxep.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2xzhastvj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ibivnfvm.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2eylaqlng.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2lgktxbqz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2bbkxuoji.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2takzshhs.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2xxtfynfg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qvznfzzm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2iplflajj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2anaeqvib.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ebwyuffb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2mezskiur.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2fgctjkrt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2whgnmjte.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2pbudkeyi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ppoagpfp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2bwxzapce.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2zhdnhsbx.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2suxujsaf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2stlyggcr.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2eoqghqch.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2qbrxdfpc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2lulrkvkb.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2rufyewch.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2chtpavve.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2oedhncmh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2fbnqnysf.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ncyiluwy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2fhcacphr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2vomjttbl.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2xfxqtrpr.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2xauejdmt.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2cyilkqks.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2blsalopm.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2xatjidnd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2gyqgqalo.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2guiipkuj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2evlefbyz.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2irigayuk.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2dukrtrme.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2gepgpzjg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2sfyrhlpj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2qmgqplen.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zkohwwlx.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2vonkurzj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2uhmhtrxq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2pxuwltdh.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2lwndrjwp.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2poidgtxg.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2kucgtkxa.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hfiyoasp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2erdzgilh.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2oaocdvlj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2nkvcgjit.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2wtgqbbtb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gbifkkhh.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2dkotsvut.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zcqpeyqc.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2avrfmywb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2vulmusvn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ohjuhrkw.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xkqbaalj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2wcjgihpu.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2raolceoa.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qvergzif.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2xmddreaa.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2qkwfowkp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2jqicodcj.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ckxgqkat.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2prmoknnk.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2npgxhgqf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bozlayoc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kesqphwk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2elarcodx.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2aopjsexx.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bszqjlkj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2rfmvfgbm.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2vviothxd.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2yvdrphjn.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2fysgeolu.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2xztzgofi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2jthrrhfg.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ltxngltw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2uwjyfwcb.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2nxkjcrec.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vhkfjkrf.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2paoxjbii.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2bncufsux.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2oykurdhk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2gvtligrp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2kggrqmks.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2myqjlrjh.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2gqetfbaj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2gfabrapj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ytvyurbh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lxeucrms.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2bvgvdudw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2gmbtthdh.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ubhsadsw.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2abahgrzv.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2joduflwf.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2piwvqeoo.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2lepfiuiy.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nlqsagki.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ndvocwas.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wwjgscau.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kgdcxcar.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2salfnwfv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2rjbdkmll.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rljllpad.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2nljuhwgd.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2czxftjbg.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2opirfjbb.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2nptldjrx.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2hmzrittx.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2nzolyxtu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2egomfnia.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2huspztwr.html


<!-- 参考信息 -->