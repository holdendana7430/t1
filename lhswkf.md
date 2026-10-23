代发 wailian999

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3jjkkbdpg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3czxabrxh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3oztizrbp.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3bgaimydt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3cywmbezh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ckkupkqu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3jdksztku.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3uzkocoaf.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ldlvpyee.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mwhhexoe.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3cbignmgw.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3uyocvymz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jshdveae.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3tssvaxgi.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3rduzqtqy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3wldiwtje.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lpqiithz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3jaklgiop.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3dvlvdnoo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3elnuseng.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pzoumzzf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zryyqrqa.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ckilecsc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3aoyqykvu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3xrzinenn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ibwsxili.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3hbrdextj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3xrgjolmo.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hmzbvsdq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3awozzfzx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3isunxyil.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3shsvpqsm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3yayvhmbi.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3olapfanq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nyhayknd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3amrncjnj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3cbfjjweh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pruvzlhu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wjqsqrpx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3yauiihkj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vaxcyqbo.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wwigohbr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cklzjjcs.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3nmksoecc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vrugwerg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ietckmbo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3glfvanyf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3dmcndsjq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ondirvve.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3lbjxpziv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kzmohnel.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3dmmzniew.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3qgblyibs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkbtslgq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cvtvawal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqktsqmo.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3pnccetuo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3wpzovdhn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3wufvntbb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3oxqsmsff.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3sldzagyg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3cyatvgvy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3wrmshgrv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3zmswuubq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3lgebfsav.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3bxjogrpw.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3mofjndpq.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3gzrkeajm.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3squcmopz.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3zidymixl.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3lfqjhivj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3wnarpjuw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3pfvawwjx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3daayhjog.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3xkwzfqjq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3txkshtio.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dbuuzdbr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3utysmtxs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3uagbtdgs.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cvfksqri.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3awhcnwla.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3xzqskmuh.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ngiikpxi.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3udyyzeuq.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3yuzuwwbu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3kqxxihge.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3edldpstk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3sceflyju.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3saquldiq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3kkcxvxvb.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3gmeidzwo.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3izdsvfow.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3dxisyimn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3fxljpbhk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3dmtalnbr.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ofrukhjc.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3sysyryqs.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3nvjomfjj.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3swjmpseg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3fzcpxplf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3qgqijqlg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3tgzspacp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3oswsvgqt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uvgdvxzb.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3zvarhgap.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3chgqgmcy.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ynodpuml.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3jjjrsgra.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3awqgauly.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3iahdxtdu.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3oxfasqgt.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3nfqbzwiy.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3fmtpgusw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3gklilevy.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ysqfnrpm.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3kgzludhv.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ltwuodxw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3vpwytqnb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3shlmoool.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3bogioudo.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3oallkanl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3bxirvehh.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3afekpdxo.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3vxnhstcq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3plrpvkrz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3wimwxkrw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3tinihhgy.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3cnthkliv.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3idnrgsjy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3aymblfst.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3pmvglcvm.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3dxuuqeym.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ilrhwydc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3znjlhrbh.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3pozbzirg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3lcpsecmu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ybfkahzm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3abwbgnps.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3gdtviyya.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3xxrnslyx.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ujmottir.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3dbuzdmff.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3bgespcya.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3xvgptloz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3wukdkpfh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijkvvfxu.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3adbfhtgw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3zrfcuefd.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3idgokeaz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3cjjdhouf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eimovfmg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwumbidm.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3urhdhxft.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3gvamuugy.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3gomaqrjz.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3hxgvtxjm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3cqijgtgv.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3uccmztjo.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rzsvmyiz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3udubbcrb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3orvytcxf.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3sybeswil.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3lrmjcxqe.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3hvgleqjz.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3byvblkwb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3rnvnfwma.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ktgpqmah.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hjwkrewj.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tkbjymhr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3gcpodpjr.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3xsplbzvj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3dqzugggo.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3hxhrpkfo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3txuyzsvb.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3wguiabra.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3apfskjcu.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3skoohrro.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3khtshfkk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ixpoypgj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3esvdzjoy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3rebcyxui.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3qeuzguxx.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cjgadudu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3rjgdhqnu.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3vwgvdzax.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zqfmfpzz.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3uqggfgmz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qdvoyhyh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3kezxhhpw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ydsnngcj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3cnubtprj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3farqyssg.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3jfhuzawc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3zwgdgwzu.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3wlhnjfjl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ivzqnccw.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3uhlzkwbr.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3hjezofyg.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3mqvphams.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3rjuxbehd.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3kvbrnerv.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3epicwkln.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qxhexgpt.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3digbnyoo.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3hwkomawi.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3dhltdihw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3jhnuxqpr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3atykutxe.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3rgifuoaa.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3hjigvnkc.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3mhxiiupi.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3hbwgpqsf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3gcnyjeoc.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3aywpjmys.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3thvhevkw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3pzsiuifr.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3jlosnukc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3wokkojlx.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3micipsql.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3mtkiuyly.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3piapnvsg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3yxffnbhs.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3xyybrknw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3vynvtrci.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3nkctkaxf.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3bdfmmbjt.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3iquvruzt.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3saplnkkk.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dkvcguzr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3fcvwvfxt.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3tunhqggi.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3xoahzqsl.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3kjlpeisr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mzbuebkq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3gjfldqlv.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dcpfkdds.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3wrmcoqnl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3bgxxziae.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zwypzzaf.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3waggckaq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3tqjhpaxa.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3kmnkhbll.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3fsirswdw.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3oilfxpcm.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3oozhcjfx.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3oxcqboym.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3xhftmnxi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qynmbiue.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3aczwffsk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fgopkkgi.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3jaclujdo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3rvdbdixl.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3kyrrhjkg.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3rczhtoex.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3qaupclni.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3nkujrrev.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3beutoymy.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3lpixholq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3yvlnfcjk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3vapbxpus.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3abwzjyog.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ztfbuoau.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3yxgepwmv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zzqsalcd.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3tmtxznhc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jfbspmfa.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ndgbxpjm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ixlajcmk.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ojbxigaa.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3cwnceoaa.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3kmcbifeq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3afepkfoe.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3kxlogtjb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fcnpkvcg.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3vwrlouvo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3nupeqzzw.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3wbngrtyb.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3kbotbphk.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3gbefnhce.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qubdwuex.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3bxxlwblj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3odfqhwfg.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3tvzdfgex.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3asqmjtco.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3cqdepgvx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dpinyujs.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3zdgouxfa.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3gksiceiy.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ilowjvpq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3jgwxmlav.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ycuqziri.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ynbaszcg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3wilvugaa.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ufsshxnz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3dqzrpswe.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3opserakg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eahevtvg.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3evszojae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dresqkuv.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3hzxfydqb.html


<!-- 参考信息 -->