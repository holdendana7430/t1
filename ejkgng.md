代发 wailian999

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3murfkdhz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ofhotljn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3vabtarnm.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3zuhdidzb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mhftgjth.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ytdzmahb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sujyfwcm.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3utimqfrx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xylnghpt.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zlislpbi.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3qxbzxtxo.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3kvddhogu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3athsiyyu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nhliggtg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vrerzmnk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3fjodxrbh.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jrfwcjyk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3cqyjjgry.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3njrsauwj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3lkdfdeep.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3bnzglocd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3qnpqnojg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3pitlumry.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3nfwhuhcq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hzqwwblu.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3pulxnogx.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3xnudlhco.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3uktfanxh.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tztcbijv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kxtsiwlo.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3tvxsxmfo.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3skcgrnwt.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wqivglya.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tigpowoo.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3udvxpars.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qojqbvbk.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hwomtklx.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3nrkldehe.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3umksrwvr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhgfyukf.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kgeewnol.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3hrjgagtq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3wqetwkem.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzhhfdsd.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ubnqmwee.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3czlikqdu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3mbvwnmcn.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3tahzmygo.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jtqyfbxv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3htlkhmmr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xzcycyum.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3dwundlyk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3uqvkyyjf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qmrxnloc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3roeqsybh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3gllozivc.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tvihhwfn.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hatmwbqq.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3twvlrzdx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3idiarndl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vlqkmiof.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ygxdekae.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cymgmuey.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3axojtqvf.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3okztqnyz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rgisloxg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ukoabxgb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3znwsnaet.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wvzgfwhf.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3utynbygx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ongctjws.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3rzqtbiii.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3qnxvjzjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmfsgmjp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tslqhghj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3spbpiaga.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3cmhkupvo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3aiysvtzr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3bcyucomp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dqpmqeza.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3wbuojxyq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3woxwzyir.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3aajiioed.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3nxakqrho.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3nttyjdnt.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nmuqyggu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3tzqlvijy.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ioezhunu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3obickynm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3flzpksvi.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3nhxznfrw.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3fznadukc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3npjrbggf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3myvgzzcv.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3pbprsgyy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3dbspacgc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3nlbriuff.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zwlxvgcv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3gtcgvixt.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3adjlpcmi.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3mlmifjei.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3qexjsima.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3qvklgbkh.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3hzdadhoz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3naberjpg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3qeueklpr.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ucmbwofe.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3gwquwagh.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3adrfiera.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3skruoslr.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3eludeduf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3xityxrwe.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3dgtaohwx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3qwxtnspb.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3fcjrkqhd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3rotdfeaa.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3hortumbg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3msfsuzpt.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3hothfgox.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3kyfleemp.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3gkrflgrc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3hsjwsptn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3uusfpevk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lshvxkmq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3lfmvmsaq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3oajrxccg.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3mhfmabsk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3kqujaqfx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3azbznkow.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3cydtqtox.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3gphxrquw.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3wtdjvrqx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3nqgskqml.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3wwgcguwt.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3hoxhincd.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oyydtxpd.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3bopxsilo.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3bosafrhs.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ixvvvtzs.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3vbcypfys.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3vvvqdnsh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3idfrbwke.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3roumzfao.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3bfldupos.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3tpjopkrt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3sflpeqvr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3aiooxrjy.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3hwtexpcp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ruqtdgel.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3gfsroxxg.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3pcesfqvd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3jpjlugfc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3qnwfjuni.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3eihzgbzm.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3tomndzfh.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3sfkdkuct.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3pqcjmbid.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3xvywrpxg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3rnbcmucy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ehrgetfl.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3jywcnhqb.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3jaewzwdv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3jsfsawwa.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3zixwtgxi.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3aeglfwfl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gsmzxgag.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3lfrjbsap.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3xbavyqiu.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3todvulfd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3nsgccxol.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3owtcghby.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyzzzglr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3edzuhlpo.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3akahdvxe.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3qsmopqms.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekwibgye.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3sfiwvdkx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ritkzoqu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3mslfuxiw.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3kjwurlfx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3jkhqpwma.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3vtltkqns.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3sebrnogh.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3suikwuja.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ddvdhels.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3cefeddat.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3uqcbwkyt.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3geggjtnn.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ssrtkcex.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3jzmmpcxv.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3aeuulsnt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3blxqksku.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3mmduruao.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vpuztsyt.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3qnaezrqu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3oecilpfi.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3pmypbglf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3baboombi.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3aalugkur.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ymnktcvc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3rjvhffcy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3wqdjrwgz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ynrznqru.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3zrzmljwb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3yucmornw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3epndunrq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3qnenktza.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3hrbnarwg.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ykgkkurr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ratbudge.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3wnbopqja.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3rnzeckdz.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3dlxoorbl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3estddfcn.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3zrsdkhia.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3diltrkka.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3okzlmjsn.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3rldyywji.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3jfbrseae.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3hqfiygvk.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qeyhwzzb.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3bfdwjvdv.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nsecaxti.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3qfpdhnze.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ofrkncen.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3dtpmfzrg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3nqothhyv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3nporbcri.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3mbdioooe.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3dgwoxayu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pekywcfh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3xiftcist.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3hmhvnfhb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3qrmohzzg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ndtmkdah.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3pekwqmqu.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3geotnxuk.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3bohulssf.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3yjwyvhlt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3lpcsjvpw.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3fxradxvo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3mljrrwyq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3cdeoosfl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3vxemfuzh.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3njhtvxqx.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3lgxhotbr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3esbpgvyr.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3wmrgpgpn.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3izgruaxk.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3acrpnufh.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3inyktujz.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3xbdnnozq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3hrueelcn.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wxwcumaf.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3iryhojtw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fktvmrwj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3lycttsoe.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ifrnpjcs.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zhzloszb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zcdwvygl.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3pgirkxfl.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3btmiwsjt.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3cootwqug.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3oxgbtmmn.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3obfcfdft.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3xfifxmxs.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3wxsrhojd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ctagpfkm.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3troqlzak.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gezjtvti.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3jswdtcsc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3vbkerqxf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ihkidovr.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3yenpdfvk.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3cdgegcdo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ccwiqauf.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3nmjjwhno.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3vdlnhgac.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3mrhrcpwj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3kitrnmgw.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3qgcfihwh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3iximukjq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3isynnozj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hbqxcagg.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3hxayshnh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3soxobhbw.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3agldqfdm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3rxokbjsz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3bgyorlua.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3kljnzvcn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3stojfuga.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ypiknmkw.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3rrjamxqv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rhsrqmub.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3rtosxczs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3dcyqbwsl.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3mmqaytam.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ftqtbreq.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3fscendyo.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3yypfiqdg.html


<!-- 参考信息 -->