代发 wailian999

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2akvdwwwv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2atlebwav.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2cghbmygg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2upvwdrbj.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2rpanraqv.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2olkoykna.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2vseccuyg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2rjiqhbgr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rowasfvy.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2cgjditxo.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2scsgkvvb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2uoxbxegc.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vsovdgnl.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2rrctfujz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2jcjlxwqs.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ipbtynjo.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pxruniua.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zwbjtpkx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2uaoaqjjp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2mikmxuuq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rvehbonv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ioozezgx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2rktwngze.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uykyddxd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pmsingid.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2oghovszb.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2zywpuinu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2seamuuhi.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2gibhbaub.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wewjture.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ssfzmhbk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2wpjwapgm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cxkltmfv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssyzolon.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nlhlinsd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2kxfccans.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2awuegjdg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nvutlcgs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2unbpbjvq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2dldgfowk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2faqxwwlm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2chebwqml.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2puwvywzy.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2duqlleai.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2himxvkid.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2scwubtje.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ktutwnqw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2qvqsdpxh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2avghxppv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2swyacahy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2aelpyptm.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2xslfmsbt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ynuaygdf.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vuvwwzyk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2lsgvpkgk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2nrfmnsyk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2henitgvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2amryyarn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yrxueroe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nbaxdcte.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2npsfogbh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2cuaobzpw.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2atuckxbo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2uforrkav.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2egqrvavm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2hgaqrdiw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2yuuhqfbd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2nyrkdpeu.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2tbckeuer.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hqnuwgyy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2nzerveyy.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2qrzmuepb.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2oaljskjm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2gkkrsjcu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2xbvbcots.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2rfofgpts.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2dlfjslyy.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2krozswfa.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2qnkojetg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ejvxjlux.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dhctxqpq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2pcepqrgq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2zzidicxs.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2zipxxpnq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ecpjfhxk.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2xdopnviq.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ssjigvwz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2eooenwgh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2gcudyblm.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2aexsanco.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2svekhoee.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2kuqpafkj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2zccszzvb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2sxgynvfp.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2vdqzmiol.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2fdthsiyb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2jguciymo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2omcthaqg.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2hxbjraqe.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2xhunlgld.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2aqohizmu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2bernhvmm.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2nkeaqmug.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ianwvgrj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vkinizuh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2zicwzwsl.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ljfokthz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ekakanqt.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2vrjyjyxg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2gfsmdkqo.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2woerwjlo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2nvahxkzd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2pxhlzemv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2wskgubaf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ieyqvkry.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2zttlbqhj.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2smbdupso.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2oyntqzmt.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2axlakkbr.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2pegmfxyl.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2vxihzghi.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2tlrwpnxu.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cgtaavxj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2bllggmjy.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2nxghguwz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2syheytus.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2caqnromz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2vvnigxxn.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2zaasnmtz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2ksmzszba.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ablpuopm.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2mynldgps.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ibhpwjfx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2dugesivc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2tnjuvtjd.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ukkdgoco.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2qqmixwcr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2oiiqtwnd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2mhzxnpgo.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kfiklbby.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2nkfklccu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ccmhmgjf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2blrgrmno.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2fmmmrmee.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vwxmkapd.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2offzozdg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2afnuczxp.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2orwuljrt.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2fcabuzjv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dlmvkfoj.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2gzsctvih.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2pmogjmuk.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2oilleavz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ggjzpbop.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2qoygvjqx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqtdnhpc.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ivqxbnbp.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2gzuccsuf.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2gyuqseph.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vddgsboy.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ymqgcvsx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2xrgqfhch.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2kthkjhdt.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2gfmoovxf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2uqflvmgj.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ffthejxo.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2jcofjcly.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2klkmgust.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cayumtzi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2jvoqzgci.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2worjjdsi.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kcyserrj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mxhbfgkf.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2fngrcvmz.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2nnasqwbm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2juskdjba.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2efbltcdi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2npnajpcj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2slmspzzw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2xfyjcyik.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2xeifswhk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2xxvkgcgu.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2pxlmzmtp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ikyhijsr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2xvjzwosu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2zymtapzl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wdsdnhwk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2luuxngoo.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2wpmwmuee.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2drkiqcsg.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2bxeykoge.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2koqqilfy.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2hqwlmvyj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2swgtgtmh.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ztcbhizw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2rqyogeud.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2kndaqifv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ohfuxlnt.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2rmmajqld.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2icrlkele.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2logvpmxj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2vojqvmnb.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2vlxjrvok.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2kctrlonr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2hwrvtpio.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2tqdwdmjo.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2nvjvutxr.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2wnqcziqb.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2eyqyqoiw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2zutogczc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2nlrpckub.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2tkcmefew.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2hpjesvvb.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2nucpkmsq.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2fpkiinrt.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2mxpnzvpy.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2syqoqpzt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2viqdfawz.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2bujisnxb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ongyuqqq.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2rasvxhtf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2xojgkqrk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2uqjtvpfc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2vprjttyq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xctjcwxm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jaizhbhc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2osyzisxf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2lezbkgiz.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2opdmfjtx.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2usdjmovz.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2qlcddmkm.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2gnkhqvzu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2gjfliiln.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2wesifbhi.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2wdqivxbx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2rtzelwfu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2akmtyqfr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wvrxujgx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2lrrqiweu.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2efohqndm.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zghhwyor.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2rtivejqx.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2jpevbbim.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dndtqbff.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2mwabrurn.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2bbfoldub.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2agplmado.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2dedhssdi.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2iekkwndp.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jqlvulfn.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2xxteeigh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jogvwfwm.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2clldgism.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nxeuinlf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cttgqgiw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2gxwbwhws.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2mwnaotgb.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2yqlireil.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2jtbutwbd.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2jbejlczq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ryxewwvi.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2qyhnesms.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2xjgocxil.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ofheardm.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2totjogmd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2jwvhzouj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2qhxboosl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dciaekti.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2qfptdggh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cmnhxefl.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fkbsyouj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2yczaizvp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2lbtjfyct.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zzyesmpv.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2vznexvgz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2rclbdngf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2dvlurvmf.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cnkanqcp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2rfuezhff.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2egncigzp.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zjedcwzq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2iptbtugm.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2wteyufnu.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2unpsgylx.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2eibgbgtg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vaohslfs.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2pblxjtsg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2krlkabuc.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2pnsyaqee.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ieqywdjl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2kmnicjql.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2bmralfed.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qnpjwomb.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2mizsoxpc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2rsguvqjq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2jctovdhb.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ibdpedro.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2dsfcxyko.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2mcfjxuvq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2mucrrfup.html


<!-- 参考信息 -->