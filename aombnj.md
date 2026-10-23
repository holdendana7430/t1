代发 wailian999

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vxmrreyx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3jtpcywnc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3tynzzjwz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3xlwdsdvs.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3rtdfqyyb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3mwsciqgi.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mgbxqdwl.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3jsbobpew.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3kqdnwilm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3fxjxwnyi.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3lhfjbyor.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3hdhjrvdo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dklyqxkn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ymjizgfx.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3asfwnqou.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3hjtalikq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kcyfvfkw.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3uearyibd.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3mzsxwfxy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3iiurhwdk.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ryhhdctj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3mfzqpuhp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3jfgifmxz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3opqnmsyk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3hctilchx.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3hmhecdun.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3wcjcnwgp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3zfwsgytd.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3jnhlqhbl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnxmnejg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3oepjlihm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ablhzpnf.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3sgigivci.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3obpwtjqs.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oksnbwar.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3yxrpqnin.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3unuojkvo.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3joxejprt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3izqpxedt.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3hndrhwfk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3umzblnjr.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qpzpskvf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bbhgkcrp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nwnvxexu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fehxkrtn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3violqvyd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wkkmyajf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3wpylnqjz.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pvucpkpi.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pkqkpnzf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lrixlkhf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3fmhljpyn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3evrduhpo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3uizjfors.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3tylqctru.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3lwyspzcw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3lglnqmmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ledtcysz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3udfwdgjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrddtifi.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3jbbaaint.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3kclavqjs.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3rhjwqvly.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3pvrqocyf.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3mgntsgvx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3xvqxoxvu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3eiurxhoo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3selniujy.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3oloofakn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3agvfkyku.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3lwddyjsu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3roiymzhy.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3jeoifyfh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3qyssncdq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3lbqedbqc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3lgonxszz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3oydszxbv.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3riymoxyf.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3zggvciih.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3losadrij.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3owqerypz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tudcqufa.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3mkzylmkd.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ynakzxnw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3elxjavoz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3rugzkkhy.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3yddnzxit.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3paucjhme.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3wqxfelrq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3wdynxirw.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ksbemitw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3wnvzijbp.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3pstjulcc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ytsujiup.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3unpnmjmh.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3sktpqdtc.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3qucwkocy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3spexvfmy.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3exdsfxbb.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3vuiojdzv.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3wcmzurgh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3zwzgblac.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3armtmuor.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3akmgeavk.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ktkvzltp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3pkrbecbj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ymnaktvz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tbvjoqzw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3zsolsknh.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ukmblbij.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3coqqnvbw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3jaimvuqs.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3jiuqgoxe.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3slazfxmk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ziydxxjx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3owrigzrh.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3rhddfzav.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3yeudmtyt.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3kgfwuzql.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3qkpeyexu.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ptkheejj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3zdlxfkjf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3senkdrks.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3sbahcjin.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3frhbkbql.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3iwjupejw.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ajbrmfhw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3iwgqhrft.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3yphtvgno.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ytthhryf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3nvmfzguc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ktdibwfg.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3otglcshl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3zopevotu.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3zfcsrhdm.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3rbvhqqar.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ldzhsuso.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3cpqbzesj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3vkcwphih.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3nakeipxi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3qpiyhquu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3oejaygrq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3fnuoedzc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3xghulued.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xuovwbiw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3kqlqfkpl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3hkpjbzqg.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3emtiroyz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3frfhjkiv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zeqxgmhd.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3xttgoeso.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3mmlonlqm.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3gttclmld.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3xpjoibyv.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hyktfhpf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpghkhpu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3mifaylhw.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3dmkscydq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3oktzjsxw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztevxoii.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3xctqrgas.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3pijoyfbq.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wcndtrfz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3imubpptf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3srsnncai.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3czipwfra.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3rcxxegii.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3xawydnry.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bewctafk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xqdfqhxl.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3wivszhtz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dzpwowof.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kbxehpqt.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3exgmobwj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3vtxifqwh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3uplcyumr.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3doxxygoq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dfvmfers.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ezapvxjq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tapfhdem.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3cmxitrhg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3pevhwsir.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3onsnhexu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3nuyyekqm.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ihzxjjzw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3flzzfpei.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3bpuqaapy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3venahzhq.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3brujoeye.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uqlshxvx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3nbleufgs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3rooxanke.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3tlknduna.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ikouwpkl.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3xmzgskus.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3mgxrzfeo.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ivyrljzi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3jmpslhiv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jrvpfyob.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3axuronrr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3jzxiqzzo.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3hzztcijl.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3jbyghgfd.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3xqzowgqv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3mzhxwopo.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3qoxhbngp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3btizqooa.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3jvshbdqh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3kkmfdfgy.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3mnwralla.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3kyqbwlpx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3mcihcmwb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3bgumfrod.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3nehqviwp.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3tzmdyclb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3doecguqr.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3alhhuaww.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3hxiswrry.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3hjwzspkl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3vuyuwusx.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3mmxeaifd.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3veqnjusw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3btxbcmwr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3auictigo.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3kosuakun.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3mvgdhdvc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3srubnhni.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3eommexke.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3yyydirng.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3zccuarcv.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3vifjjxbp.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3fbqqmhgr.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3dkwnxyok.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3xusdahzd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3zkykuvkz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ojlvwdgr.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3uannctuv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rlcqudvr.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3opkgfdpy.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vplnoyxa.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3qqsdnyjf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3mibeefzn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3tjndqyze.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qkwlmofz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lmblywee.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3mulvrvjq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3afttdmfg.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3rpajqjjo.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3duvehoim.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3xdsrnwwk.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3epvvemid.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fjfxhkze.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3leizpspa.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wwyniggv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3vdmqfcka.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3csmpuazk.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3muobrfkw.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3boajanbi.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ymdbgclk.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3flgivwas.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3jjqmccuk.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3wksxcrut.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ppgctako.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3aawjlzxv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3rajpbhow.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3mldnmfbd.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3qnlacwcj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bracbxpl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ctwfoimw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3jqbawasb.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zvowvfjw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3uqthnzeg.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kcpvlvez.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3stxoaxsu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3yqnpgkzy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3tsbgsvdg.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3vbfrolio.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ghvxvvoc.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3qtoralhe.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3fnoaydib.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3qyckjjiu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3zzdqqham.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3rftviema.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ccjzsksc.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3awxcorpw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hzvuizha.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3fkpfnhyj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yztjlmxp.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3wapmqpqw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rofroxok.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3mnouwvyn.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3dtknfipo.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3dgpmkinn.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3kerkklls.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3bskavham.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3zgmfzoky.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3cnfliuul.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ayctdhej.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ecjfvhqs.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3nzngkzsf.html


<!-- 参考信息 -->