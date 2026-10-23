代发 wailian999

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3nsztnxug.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3uwttyglp.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3jokoykib.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3nfyodzhn.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3jftdnnlh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3gdcvdlbb.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bcpdvlbc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3zwdkyzke.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kxwqvhfy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3fswnwfkj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3tpozentl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3sxipopdh.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3eyvjzfzd.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3yexifotj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3yymnmmdp.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3etsyoxbg.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gjonykad.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3rekfkffr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3zotnpotv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ecfrtdry.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xzqoehij.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3jcgvvkae.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3respbyga.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwdlicqn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wdrultzs.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3qutickos.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3bwlsccqb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofexyneu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ctdcvebv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eeexjxnm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3uqjfvzop.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3zwmnjrle.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3axgdhjsj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uxmsdtbs.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cshipgrg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3vwmphlsr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtdgbvjj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3abnlwsxg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3yfgnsxil.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3gpbwsthr.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3apptlsau.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nmyoonkh.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3czofasfo.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xxpxnrlr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3zwrnzzwg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ygorryfb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgycwpda.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3yvnkulms.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ffnyawph.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3txuauohw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bpqjgacv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3dqwwxyzw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3yzuljqyk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jphuetgj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lzkxjhym.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3yilbyqzr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3qvrogzpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mtmebhcm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gxisixru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hdkupkpv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3vfeyhkkn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3cveqeyab.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3sazayfjm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3jbwufrsz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3awadcddg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3kynrzvjp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3zrdjtwts.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ahizjqfv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ujtowszw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jglxnkhn.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3sgwofsjk.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3pqslonkn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3twpanisb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3pfwucykh.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3gjvapsli.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3dosklnuy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3rqlxbzlf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3itecnzgh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3dwuvfesh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3oumimhjs.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3huahqhlg.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zpitjovl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ychrozic.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3phdahxnv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3gvvnxygy.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3dwsmkdsp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3vrlolrib.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3pouagdvw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3omenohns.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3eehgmaaj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3lvkpgosu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3yonmtdwc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3usrhkjty.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3iytlqbwm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3iborvwxw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3xnggiemf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rtmucdyq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3auhdwraj.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3wmgljvph.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3dgbzdpbx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3zeuhqpkp.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3hofwbjre.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3zcwjjjvp.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3hsqnwhty.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3kaiqgnln.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3oipuyuwx.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ynznvcbs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3etjdttzl.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3vdnndkzt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3jubtylzd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3weaiebus.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3gplkxydw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3sgvusmvc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3xjdrrdfr.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3lapzgeyv.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3nqbwuvrl.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3knewrtyg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3atixuoxl.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3bxjguemp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lkqgcfzh.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3brohwtub.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3gmupvnoz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3zoaqemuu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3okxydbfz.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3fxvywgok.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ktyzkwxm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ontntouc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3jrlauric.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3wauzsaqi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3trfduvni.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3xqqtlqyi.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3kenspshj.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ajtqurwc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3xyoubkwn.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3diujvoat.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3shkmsjys.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3egrugueb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3xdikjmwx.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3jfvntmem.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ufmmwltv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3xyqaxser.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3zisjioil.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3kxbieyqj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ggivxfqy.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ghbyfnzc.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3nhexpvbk.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3uhtoqgsh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3fckxkujz.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ykhbonam.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jchqoqll.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3lfypblww.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3dvtdkwej.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3kwowlxnv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3mexoitwa.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rudsbkwg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fymybxit.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3jdborrkw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3cqbhklom.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3svcwkzmd.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3yztuvoyz.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3yrduwsau.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3emmxjnoa.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3srioanyj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3grxcusts.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3riziqfoq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3qthnywfp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3knrwbyzd.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3xviollfg.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wkdxhuer.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3hxojykkk.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3czdanhyd.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gfwgqipk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3degjzwtg.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ecgrqeih.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3cghltpma.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3fdkjngav.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3xaukfiqu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3atlpexnc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3zawmbibj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3avngdtkk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3iwiirqrd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3twuvupli.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3epuoavel.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3nzxzynks.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3uingigfc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3dvdeoiaf.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xjcmevbs.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3fdfpmzzt.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3kcfjhwnl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3byuuevlm.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3jlnncxhn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iqbyizzs.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3khuxtpir.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3kofswpet.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3keyqyyiq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3myyucpns.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ajjgcwbr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3pitxnhbp.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3tpsiubir.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3zhymxltb.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zpewcalg.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3kuzpyupc.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3prdzhsvt.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3rqksdfkz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3spflxqzc.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3qqyqwczb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3thgbefrj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3lwmcjeml.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3becinrgi.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ifjhvqzn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3iabswpro.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3lpnmcqqe.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3jsuiajgj.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3buvzdmmu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qjujdmza.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3nkdqoxtn.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3mfvuivaq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3igyagbtx.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ospherba.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3dmmibgjs.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ryvnrlxp.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3tsbicavo.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3mbanblmx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3upakzyjh.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3owpcoxuc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ipdehenu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3pqorkyyq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ayvrumpb.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3yfwzztcv.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3dxvgygat.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3yzsffzhy.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3bvdawhyy.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3bmoklxos.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3wswkeevv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ojhikjij.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3xinbpktj.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3gfzyqzca.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mjvupuqm.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3tfjtvipy.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uiltxvow.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3cknxzqgz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3qspeysyd.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3inklxvow.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fjkcdehq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wqdvlspe.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3xtabwrgy.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3cihfrwql.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vwqitcno.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3cgheekij.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3rwntiytx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3fnnnoxtl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qnghaysu.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3dllrqljd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3njidtssw.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3qvzrnvcw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3qlikhrly.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ngmggtys.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3vsdnbvrv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3jvthirvk.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3tjwgycrd.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3gyeogkgw.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3nghutwjr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3wyxjwjlb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3aeezbrjp.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3rcjkmqfo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3dxnmlklv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3bugoxifc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3axcrlzpu.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3sqbijeqf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3inrqbshm.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nyxqmfay.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3yygajhbg.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ppawcyxu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pimqbsgy.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3oalreklx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ufxemzkh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ignwmrgl.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3btmhgosr.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ykiqqgnf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3kcqdwopl.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3dxuwekmp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3kfiwkqyf.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3quraqdwd.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lyqllulb.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3euaimvyw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tgfjhbum.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3okkzetfd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nvwusqbt.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kuoggutg.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3irnsnyjk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3xumfnafz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxaguhas.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fyokzhmj.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3yrcdtsnh.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3xvjgtzmu.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3nzzazxvg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3voucicea.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3kegysxzi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3unizbcux.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3yevmpmvc.html


<!-- 参考信息 -->