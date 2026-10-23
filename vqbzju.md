代发 wailian999

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3wpkljafy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3npjqlaei.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3jypefnex.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3exubgxyr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3wiyrnalr.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3scrkuuhh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3sofopsye.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3maskotag.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3fthfapup.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3cqgnmcyh.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3shzuohah.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3xhqqlshp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3zqkmfvkk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3uvbqoria.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3fuzbczqn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3xvjtdugd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xlpfoyag.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3kufoppxx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3phnnwwjw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3iqoroyjs.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ittapefr.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3hrqkajzr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qtwxvdzt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvcgvmym.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xjhvujlc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3qjdiuchy.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3btorykph.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vaciwvbu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3uupvutag.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zethaejl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ktkxppol.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3axiwgdfa.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wlquikkd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3afghmewr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3snwuftcg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3gqlponec.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpfxbnys.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ogammcln.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jkqlfkmh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ixmxzqep.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3kjqdibbg.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xttwkbtv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qjuizady.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vesqpprw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3hvfmgnyf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rvxlgbmx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hppoabtn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ckjsyuqi.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ujttkngq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3wdmdkemv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3mwzeqgmi.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3piyofrqe.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3hidcdhlc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3iykacxql.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bmzsyoee.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3iyizmhrn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3hhgermnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgmlwccb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3exhgyfrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fhktduwu.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ivlwnxji.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3zhphnobh.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3xevwdmtl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yqlwverr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3lxnvrcoe.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3qesviypc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3bmciqjib.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3eysjppru.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3lwmqaspc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3karkwxoe.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3zymyxcme.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3anrwdsgk.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3hugklntj.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3sgtabsem.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3fbwbuktu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3kexpmlze.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ueikfnsm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3pcvfytzj.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3xcmxpvzw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3fuoussyp.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3wwvtgrru.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3vjfdihit.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3webpbsac.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qimnmkpv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ycdvljmo.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3qjesgvsd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3jacfamec.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ilmpmkoi.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3qlhtfwrw.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3jxjghliz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3papsxyou.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3dgakelrd.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3rkvnabzl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3rvosgrfq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3gwnvupju.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ddwlmlen.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ahofveqn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3gotmnltd.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3odmosgvt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3yyymbdxx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3djgwqjoc.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3oaanzbcg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3aohaejpq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3jbvtcbql.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3jgrnenuv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3osjbridm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3asuzamfk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qcnvnscz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3taygidtl.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3awxbqcfi.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3blcxxujg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3bbtjoxzb.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3wyndknnk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3zibgbtwo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3yehergzg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3knhequsu.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3bbvxmzuc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3toxxygwh.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3lvwfjumz.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3upkvamur.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ndglnduo.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ruloligk.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dayxaakb.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3pqtyymzj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3qhtuhapg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3jldtthom.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3dlfibpsc.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ohooyepr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ziccgveu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3qwxuesna.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3oigelfcf.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3wnouvxld.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3betdqnzy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3xxjfdafy.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3jykcmnoe.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3lqxgzudm.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3villzsxu.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3xmfdcsen.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3jprjiyxq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3iynnyneu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3yagbpxhd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3nlozdykm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3puvzuluf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3mcpaspbz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3gjutgtkz.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3fubeipec.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3lalnylli.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3dmttqjcr.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3enexqpka.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zmjayigu.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ldqarnjp.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3jrhydthc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3zvgzewcy.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3qwafypsh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lfyhgtwa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3wufqwwem.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3irtczrok.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3yqzgocbt.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3fpvytzet.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcbwemju.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3oifyscgb.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3visigffd.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ugattqhf.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ofvyobal.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3fydaqoze.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3hvmhcduv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3aktykkuu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3exgubtmt.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qrffuoas.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dmtnwpmy.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wsmelyne.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pemkbklj.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gurckogu.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3zmyrwdjl.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3jcytelzg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3nxiezqwp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3gzdyldgi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lnthlqik.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ymqimele.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ocbkfzfk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3hpyrvxdp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3nvikgstq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3akhdfqfw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3aptqosgt.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3yuzjamtz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3csvqvhdc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3iybgtbte.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3gbodtlgr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3beemjiwy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qucudwic.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3qulfztsw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3demyqqpt.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3haggqqpm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3kdcbkgda.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3aratrijk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ifcsynsc.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3exvziclx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3cskglbjc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3zqpdetxr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3vkeywima.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jodawmvn.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ewjixyjr.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3eqcudpse.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3uneahhxf.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3paqcvqcd.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ocgjfbbb.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3snbcnaxr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3cfkveqms.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3xxeohjdh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ckomvewf.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3phtfrpck.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3iqdasaud.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3blweyldw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3jguixcee.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rxriqulw.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3htsshgel.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3gchqtxwf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3drfwwlex.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3gawdbgin.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3sntswqoa.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3fwgwjcyg.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3xqspuemr.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3iaqxmpqh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3zuebvbwf.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3uehztugq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3pjxjlqop.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3wcvjdbyq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3cfstdxww.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3vxgrhuny.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3oxprabrv.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3aanjuaha.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3itxoahqn.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3uyqwqyft.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3dsaofnwh.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3uabpxfka.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3oyylqxes.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3abahpaud.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3czskamco.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3rupckwlf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3njnaamxx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sdqqkpuj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3bvihdthd.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3brrcbtbz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tyqwknvr.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ytrbyfrc.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3kvqardpo.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3cydjnizk.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3phtffyrv.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3dnfevhac.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3bnxnegdg.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ywucaetc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tishoxto.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3zwlmenng.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rmojdnki.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3pnowslmx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3dunukvfn.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3eanstbtj.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3gjgvvgli.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3qsdtzpla.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3rgrihftk.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3rqlkrfyj.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3izaevejs.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3volvdnhl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3gmgekxib.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3aewvmjef.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3mtbeisij.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3gegmhjrg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ksvetynw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3mbjjmtqy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jxoksidl.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gfdufkyu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3jvihpstf.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ramowdeb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vimuqtbu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3segqdzzs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3kekmducm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3tglypdeo.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3jbuuuolc.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3bhhybbli.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3coeiimjb.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ofcdokzf.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3pfdfuizy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3mnvihpsa.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kbmmsknp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3adzgyfrq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rcplhtlr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3icnyasgp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xcahvomk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qxvjrdsg.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yjrkzfxt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3afejhzhe.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3scwiorev.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3cgsgnwir.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3gesuqwsj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3kmctvboa.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3wuhnjhib.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3yesjbedw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3sncghtff.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ihyrzicd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3vioqwzyr.html


<!-- 参考信息 -->