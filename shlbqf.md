代发 wailian999

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3egdmnigb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3mocoxvck.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ofgmkoph.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3twhttbxv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3vasusham.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3hdimctji.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3rjikkxmv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3vhbbyoya.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dnpupcvz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ileyrfoo.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3woghnekl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3sjtlanwy.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uwreqdzr.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3mzqnjnqn.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3qnudgkkv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3nmzvwktw.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iuwbirlp.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ihicmidm.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3pqehrtxa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3hqdgapwr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uvjtfplw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ptxhnxon.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3lrfsbchw.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3qmfftebs.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3umflzctl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhqfzqfv.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3wavxwpjj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcqtcukm.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ljcevpha.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqlyzvlz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zjqgdenx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3hsektorx.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3xrbjlndw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vddaivyq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rwsnpmss.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ocmijhid.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtharbiu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qtwhjlcg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tsyphbco.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3jtcxofuu.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3siqbqtxp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3agbenjlw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pjrizhhv.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3scgiinei.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3hgklxrml.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vsjjaupr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3irddvxdn.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3vxwoogal.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3cswtyeei.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3uqbwsxvp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lkbfxskv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3unnguglz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rucygojt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3izaqagkh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3emtkpwbe.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3tuagrefz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3mffilpbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhqltkoc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3azjdefst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwzifsde.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3spnchxry.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3nmerkrog.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ntgpayld.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3mxpytrhm.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3tbwoleci.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3qbafuupd.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3yzyikzte.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ewfqcnjk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3kasabdid.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bxkaidlx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3cettwspd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3lirthttb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3cideiabw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3eceohfij.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3wtinkjgm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3jhutxjuh.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3dxtujrpk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3deplfeca.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3lmcaeckd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3xrzyjcyn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3hdnwjduw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ymjsythp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3nwgyjrgt.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3wkwaatun.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3xgrkavgt.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ikkgkygq.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3idmkvreg.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3pfhlcjbm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3rwsjclgd.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3cahfxhli.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ctwurywv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3gzfepojq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ubhbdczd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3tefiakoj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3hqitgcfx.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3pqykswws.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3mchsdccz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3wdcphfmy.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3wjgoxvge.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3agqfsuyb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3busswcsu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3yhuznute.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3dodoomqy.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3yssjvjbn.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3njptzmzs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3qiyrnmat.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3dnnmirxb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ffozobyu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3qbehghku.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3lzbytcgu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3pdbpkbzb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3iizrmlre.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3nsozqygf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3dpwedyhe.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3nqwpfulc.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3cspbdztr.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3myevycjt.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3lbtihvba.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3iydhpgko.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3fzysejcs.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3tblojndq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3fojkdmbt.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yjnxbnom.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3iymxhdgc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3zkkszdnr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3uablutfs.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3aktsrsxm.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3dcexhkzx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3hyklxhce.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3fjcaxums.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3yerzdlmx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3qibdjkhn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3atqybznn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3huudkkpe.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3psqxkpou.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3xhzsdyec.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3twcoeepk.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3hiornmvz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3fkmlnffw.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3pnofbqfd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3msdmfybo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ibuaohpt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3qmneusqb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3bvrqehwd.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3mfncexrj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3dmewvfpj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3buwaisxc.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3megewwnj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3lqkqhvus.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3anmjlkiv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3daqklvza.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3vsmpogfa.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3fyhuvfqz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3siplsioi.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3dlmdmiui.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cokynvbq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3koeykufm.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3clnnswun.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3tjpyuloj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3waayoney.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3rzhauism.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3tnruxcic.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3woiytata.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vcpphmcu.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3wrjjomlw.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3lxntsuly.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ismqslcp.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3kmxhxflb.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yubedekg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3hiibjqbv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3rlukflzq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rbbsqvem.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3snrpdkna.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3dpaxsxbi.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3rdapwqjw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3gcvyzfiy.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3wrurrqvj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3toulkgcy.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3zquogqvh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3dijddukv.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ufppewun.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3jvlgvuda.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3gaouosts.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3whaiteku.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3idlmvvut.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3bndvvgub.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3aacldbbh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3oyxjfbxo.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3djjhiyrs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3raffsijt.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3jcnwrsvt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3jxgsicni.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3cjysjtex.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3kakqhmql.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3wmqxqfon.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3exupheuc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3uqlaajkh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3jtkmlbwh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3omjnumvv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3fjdjfkie.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wwlxqrrw.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3iiqxgtdy.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ghtzzvuo.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3bqwdhytf.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ryaisrcf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3kfhxzhch.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3zqhqraxd.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3puddxhmc.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3rhwwjooq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3vswrzlij.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3xvdhujzu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3jdpmsffs.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3donvjksh.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3rawzmhnr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3jizeamzj.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3tdtxbdoz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ebjuscsk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3drooqsoi.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3maymnhdp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3iisfoqae.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3bzcoqopi.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3goplasrg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3zjsabbkb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3chvvkokr.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3pqytmlnv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3oowiuraa.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3glfgorai.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ygqjojcs.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3zderirid.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3egxrjzea.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3lixxiges.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3syawrckm.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3idohhybz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3regwtlet.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3uwceznlm.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3hhjoyswa.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3xirrthkr.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cckbkrsa.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3vnewdqxx.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vqudanne.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3xfurdywy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3dvknhsyl.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jcnmvkmt.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3iultiebl.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3pxwlbeun.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3tfknwgxn.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3tnwwmcvf.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jhiulgdd.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3xvjxcccx.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3bpxpxiib.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3zkkxaxef.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dvpgsvzy.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3yyyxslxe.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kytscuym.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3alvnqsqu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3gdzibcwl.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3qtafmyms.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3omiyruzl.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3nizikexe.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3tnclmngi.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3mtkxmjhn.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3bevagbub.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3djoictgs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3culrmytd.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3kpuaiejx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3prsxruna.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ripylfel.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jardosih.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3qjsbulhr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3utbgwxbr.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pvtffxwm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3xrlmottr.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3bflzkyly.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3scnyybde.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3dtajkmal.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3dytvqzoy.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3wrlpxwqm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3flawjbxt.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3nihqeegt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ytcfdyka.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3thxqnccs.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3pckklslk.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3odnfdsyj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kayttopv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3lvqfdmxr.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rwxyplvp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3npjwgbsy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3cqzfujsz.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3yangkpjx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3twqitudm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3zmmgrwck.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3arfuozhj.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fsdqtcpe.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3eaxdekds.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3osswlesr.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3kmnjvfrc.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3szdltlmc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3dooppjuh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3nzhdiszj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3nhdtwnxm.html


<!-- 参考信息 -->