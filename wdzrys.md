代发 wailian999

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3izmhpmiy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3enlcelru.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pwjheosx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3vdyukddc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3nuicnuzy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3qejmozmx.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3aneqvdxw.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3lxttswen.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3smzgqjra.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3jovvahjp.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ksvoeqbz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3gmrzdtgp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dhscxtku.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3drwsrqkq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ceeaxhlm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3jmitfrjt.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gycepvve.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3rramrtsg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gctlekxl.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mumosybv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vibpwvms.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3scqaltez.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3alcsblrk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzuwzfkn.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3fxhvlbni.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ntvewbzt.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ottdbwtc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ioaueqbn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kbiwnknw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yhdxpwgw.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lsdbwvek.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ilsezmzn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3nxmfjlme.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3afgytagn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ymtyehgo.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3uioycqfo.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ufoyeuai.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tvbpxieo.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kfkngewz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qunozady.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3myfptmjp.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3axofqloi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3mleztnwt.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3wbbmshrc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3cjhflzly.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3opkblfcm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3loetyshm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3zapzsbrf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3rrixaagp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hovjpble.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wkvckklc.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3pwtywfdb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3aifavxms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldoocnoy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3suxmlwvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wkedurty.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3tqmlexoe.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3epftzpfp.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3uiynrdfk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3hztbrtxe.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3agtcbzah.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3zrwcstsl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3vtadwjni.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3lligilxo.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3llmntbpj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3sdjeqhwe.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3qvwskpqm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3cnztdrmb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3oxkaatle.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3nrtuiook.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3tzgrbhbg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3eejaqlxy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3exesxhwk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3jwlccwpj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3celkczjb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3oiqzfftk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3coskosnb.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3imshajjc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3kvtlcunl.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ebgidpwg.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3xcitfclf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3rninglcl.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3vprmvzek.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mffrpgks.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3jzlxhfxu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3pehjomtc.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3lqhcmpsp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3yecuoput.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3evamrmpz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3lpugqcji.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3dsqwiahs.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hfmlvwly.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3kvjsjvyx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ebgtfgpd.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3hjzdpwtt.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3uquchrwq.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ugwnfpfx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ozbqcpbm.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3owohttoz.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3uduuxfox.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3vzowpmfw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3kfrdymfy.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3bdflvynu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3iwzxwoim.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3zuhpminn.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ozzfdtfi.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3vjkhwmdf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3vgrnrhgd.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3degaslic.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3kbxbcwbm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3pounqvus.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3depspsrj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3gzsssyjz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3xgrdcpbj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3lvozikfs.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3wxpvmgfm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3pygumabu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3fbrgytle.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3kzwyryyb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3pthdfqmo.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3rmycbime.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3xqixniiz.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3rlvelimh.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3uxzrbtui.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3pqkzziuc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3hpzxjjxq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hcyyvwjd.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3supmysht.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3hjhkfyag.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3vyunamcu.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3qmimkuqf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3rpmpahzl.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3dbmbtmmu.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3edgsqtac.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3jwaincpg.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3whhsaatq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3aqsxmxhj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3qakybkln.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3cfzhhtfo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3vswhpffa.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3scgxsovu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3rcndkeml.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ncfekdvq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3drzejpck.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3kjpuwbef.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcuupkju.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3swgmskvu.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3rzpidgka.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3kvxqerkq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3uyvnypxl.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3cuifxdfn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3lgrysrfi.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3wlczlukm.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3qzdobmll.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ymppdotx.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3udwxsquy.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ajndqfbz.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3slfmbxdg.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3aqywhzhq.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3nlfcxpxf.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ppmpmcei.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ccadciwp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3uqeslbrm.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3wtzqobmb.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3perxvbny.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ydktpruf.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3hndmyxdq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nswniefu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gejkiwpc.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3aizxqoba.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3cjfaetae.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3rkfkedod.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3plnsouwq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ukmjqniq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3brdlxpyy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3dliyhapj.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3moqxcdee.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3lpqxctla.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3uwhuwhox.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3uzzstlbn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3iuppkrot.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3nzwrgopn.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oqfxnztu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3doaazsxi.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3zphwtdve.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bmpyxjpq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3qcaaqurx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3xvcsbiqk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3jstaoora.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3iyirgmgh.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3qefidfca.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3aegbtibi.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3vpwtuvgv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3xdmlqfat.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3lcmkokpj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3jjzaavch.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xihcvcvz.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3otwkswsc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3shdgndrn.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3snjdujfk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3oydogfts.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3iqgdhnzk.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3sjrsgffp.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3anjlmhbu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3cseoislm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ofrhkyji.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ipssochf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3davlrhaz.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3dxwdmrad.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3nuyuxehq.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vssszvws.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3tthysrcy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3uvnmboeu.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3kmzukgwp.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3xoyunqom.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3hvsgbpkd.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3rukamxhd.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3oblavgta.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3wvjgbqem.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3pydjlnmu.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3vnkzbheb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3oojbypli.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3mxihdykg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3xgivzvfs.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3tfyrocsk.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3kvfjxarv.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3trydopnd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3iyiclnrt.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pesrwkwx.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3qzalmplq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3cwwwhjgi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3utolmpue.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3brdcattn.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mynrqfmn.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3nljdkdpp.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hzzaagdv.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fkipsufl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3krnsyrsu.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cqfgsqry.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ocgpjtcp.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eizbozto.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3iqlfkfrz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mlmirvbi.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3aqgrpdus.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3bhqbhiea.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3vsyofjpt.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3hqpeiymc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jjbbubrv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3mqgfcubg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kbbdfzoq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3cbolmwra.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3wxrzqzxn.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3nwqkizfl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3zuzrgumf.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3jyslwjwd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3ccuseajh.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3gbhqchuz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3cfkciebq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3qinkxrso.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3ssmyrloy.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3qlnixrhy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3bxsnmgqz.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3bcfimyts.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ilvehjse.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3pnvgnash.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ncdyhrkx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ikkpklxk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ptyldobx.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3tqjzxbwv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3nfqedkpm.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3xbavswyo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3bnjtdbyr.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3izkuqcfu.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tkiuzzot.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3wloweiqp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3qzvaiqev.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3kkvmnnzt.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3njuuugfv.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3jjmolupr.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mkpvlkrt.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3lngmrucy.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3njgphicz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3swruunfu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3pdffadqp.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3aabpanze.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3algsutga.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3nmsrmqni.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3nrzenvnn.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vugtkgir.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3xropdghm.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3lqzyaykm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3bvrmbgiw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ytjeyvzw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3cdvpefer.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3giwvdomq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3rztcjspf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vnrohjsk.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3kxmjfhnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvpiwplu.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3qmjesvub.html


<!-- 参考信息 -->