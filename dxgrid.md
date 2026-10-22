代发 wailian999

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wdgvebel.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2hnboximu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2wpcwfkga.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2iotxfzaz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2vrnhdtwo.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yfbhfgfq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ygstnagx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2jqyfzijl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jltywjrg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ldbbpudn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vitzhkvj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2rzutjsya.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ccfisvyw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ubvyfvtr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2cpcbwowv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2faelihki.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vtcvgidk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2jergbyiq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vildizrl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2jbxhqham.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2eihwlwmv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2dgbdpjkp.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gkjrdvqe.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2huvtcqvz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zpdeuoii.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bihyagxs.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2btauhqyy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxooygul.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2vvslafar.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdwtxskm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2xpplwtwu.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ljyhuyxs.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2lcnicxwl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ingtktvp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vmzcktlj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2noislevs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2rtkionvf.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gcyvwawp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yyccolvl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ooxwspgm.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2osnrkxww.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pesjckfb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zngmpfea.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2oyqqdsko.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2txisvtvo.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xsoxzlvc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2vljnfiiz.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2dhpddfcb.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zljnxxky.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vjivrdci.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2iztgowsk.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2mjxefmqr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vjlpymbf.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2tcfkuiuj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nqwfjmfk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2gfmrvqgw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2oireehiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2edcnwjcq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2kxwphdnb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bwdfnllf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2dbfrkqxn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2mrihwrqr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2qeqkfebf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gqwzwpki.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2caqzgflj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2oclkrtzx.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2quhoxgfi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2vpkvncnt.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2vajlwbpg.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2afzvwxxe.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2lhcccpef.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2dkvjrhse.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ccpfyqfi.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2legqurej.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2cabtfrwl.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2hlazfbiy.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ihmlccag.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2pwzjkopf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2agacouip.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2izofwshr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2veuerxkj.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2sizyawxk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ywzhqhbl.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qfcllime.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2mlytoupe.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2kpwtvjai.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2njyjkiic.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jtfuifzn.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2xfyspwvk.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2zvdzfidy.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2iemiimmi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2omisrlyz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2lczraxhv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2wfoacuqq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ueqylukx.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2muoxictc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2yyegbacj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2bidewxwc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2fcfmoalk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2tudgnfcu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2tgcgjuwk.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2bhjcnnlx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2aihurgmh.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2oztcyznf.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2lverwojg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2slawaxpq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2qpwhhmnv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2onhihhub.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2dfippvkr.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2qdqvylwp.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2jjlqlpke.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2nppwshlt.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ofonnyke.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2klvvafgi.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ffuypyit.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2txcdoans.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2zsgkouvs.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2egvbdlew.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2opztlupb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2miugkrze.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2vqzqelyg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2abwynqsr.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dofjigyj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2bfqenbxb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2bnycenqm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2rehmkgkv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2kbedewmz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ksjvimbt.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2dvnwpsle.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2egatgicl.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tecsftrc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2uimfbpzw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2lhbujpum.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2qqwfngra.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2fffiowch.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2nqhefdnp.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2thcstcyy.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2diudosgi.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2fxgawdda.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bigqfkoq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2kzhdgzdy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2etjcykjd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2pjgufnrt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2brcpveiw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2muclctfe.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ccqzkjuy.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2jfazyjcn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2bbckekqv.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2rgihshkc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2drsiszch.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2sbfflake.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2bjertrhq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2osnodrcs.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ksbvmkdj.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2vornshic.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2prtkypae.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2qgikgyzp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2hibbenib.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2cqrgcxax.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vsnrisrv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2lpcdqeot.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2mtrwncfh.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2aihaxypk.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2mznbyrfd.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2scotcuqc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2pkwofpgu.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2fwxldzlg.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2bysfamgy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xagkqzva.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qjzlqfit.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lxeujgxs.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oxrfnweu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ppbhnaoe.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2cjzctkyx.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2mrzexxrj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2blkykbzh.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2loxzknls.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hrvtathx.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2pikurjcy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2menoxqdf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2abiancme.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2umjdznav.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2fqmqjzsy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2vallduhe.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rljyttdw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2uwzckhou.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2loycijgn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2kmkhxbxk.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2zyogefhf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zzehdais.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2oalnckzk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2teefiryh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2usrggaum.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2hitsfrwg.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2bsaqdiey.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2emmmwsrr.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2yuymwxjs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2pwixnugj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2nejgkdjo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2vnotarwv.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2syrlxyok.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2nlsyebat.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2sgwscprv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2akqkxbon.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kzwedyag.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ousvevlv.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ofjqstup.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2tzwlqxzu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2daoafshn.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2mndsuwzp.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2qpeenhzy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2hrzfwcgm.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2rorwlcgh.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2kcmohqmu.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gkkwduug.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2yfbrimbq.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2sscciisy.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ltshmrey.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2jubuqjgg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2tjdfkxva.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2zcnsoxfd.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2kujqsiwj.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2uasqstve.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2rfudtoac.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ujsjxswc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2druqbeuq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2xyvxahfw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ddxoyqmo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2mubcwnrg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2zkeyzyru.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2tpskdste.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2pjhxnpea.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fznovzkv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2xlkxntpa.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2vzrrzasm.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2jjweddsv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ldpshguf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rzeomgfx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2xuyiqvtv.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bfvczufj.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pgpxgluw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ypwjdylg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xipnozvu.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hpdrgggk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eowbmcnn.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2equkxbiq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ggiomcpx.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ztmfehwv.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2odopnfmw.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2qazcbgnc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2hpvlcafu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jnvfzksy.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2lcrcdtcd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hmivlwqr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nizmuixf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2pxkqnobs.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2kfnbasjm.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fqvriwkt.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2saguoxdg.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2fxwlmxhi.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ldzkvztv.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2nuycqbvq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2gjdevwff.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2jjatvzbi.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2eqmmoips.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2pgzdzlhl.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2krwyvdmf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tgwduugu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2khgkjxuh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ckoxajvm.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2evyjznoj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2scnzcqzb.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2lahwfsxj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2fxzmpqmm.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2dqvplsts.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2xodpennj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2smtcoxir.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2brlxubzl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2mcimtete.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2cvmfnynn.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2qcnqaxvh.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2oocyvrny.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2avbaxyic.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2euquhimr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2apzbpcvh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tivbskbh.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2essayezt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pfaqanjr.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2katdkuvd.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hcbsobqx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2efnjmrzn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jgydhrrx.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hyrxttey.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2apwhemue.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2hbgzrnom.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2bdkrfabk.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2wgtkeuhd.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2rdacqsej.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2tiuhzafi.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2uqpywthm.html


<!-- 参考信息 -->