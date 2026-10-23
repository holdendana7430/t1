代发 wailian999

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3axhojaht.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3jfvhfudr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3gxtljfnl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3qzvwhbto.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ojirdpzz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3zwuwidip.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uhvayhtv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3mkqzvohp.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zodcpava.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hkcavxvp.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3uubhykfg.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3bbnhmwjy.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mjzfgesg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wmsnptfk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3uqjkksnr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3odputzju.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3xowxkqet.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3bvlkgnut.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3qzwkaclh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3setkphgo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3udfanwvk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3mxkgmetb.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ejzrfftc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3zzpvznen.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xxxejdks.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3euntjgqe.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mcbzsrna.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3tzepahhx.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xauogpyf.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gcycwwui.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3hqdjnlzy.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3wfwgnlln.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3svfiepjn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3knkgtzgu.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3dyrzfvvy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3turdrydz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gvbwbeju.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3gxpytfpu.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3baaerryv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3agqbyqdq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3xwozmaao.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3jffopbeg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3gtjadbuz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhjtooef.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3kitadjzq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rytnwqdt.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3liejpqms.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3nfzfgxol.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yoyaumws.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbbegyxq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bzfrzioj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3rvfmfppu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocdlfuln.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ypsyhmgi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lfvhswid.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3jrxymwvx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3dpcufvgo.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3phzevufz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3svldmgri.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3mmtrenlg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qzetryye.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3alkfkqvv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3wgehyybk.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3nulbgcro.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3dtjnwlwd.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3spvigmyt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tzjlmosq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3lqjupimm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3nlmamomt.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nnytdqnj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vwjwpsok.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3cajsiqmy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3gxkzwera.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwhaqcdi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3wadsmxbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gnwzhwkk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ynuvizeq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3iqztdvns.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ayrwzxju.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3odrtlovq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3mapuqlnz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3pvcluwqb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ebnmxyyl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3enoiezey.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3zvxnzhrk.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3upvqugiy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3lbqusrwn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3pjqigdka.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ssxnxakg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3whivhxld.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ztklcnmp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ykgqlpqc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3wqgervxi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3mschzshc.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3eikdylbc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3aqcoxjnw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3njyqjpob.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3usbtfbsu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3hytvumqy.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3uayhqhmf.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3mppourby.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3uxvjsphn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3rqovwzke.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3oadsckzz.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3tkiodgoy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3thzxneli.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3tlzxoykc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3bovajuzr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3hrsuijws.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3nuhznkns.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3bxuxjkmy.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zdqqpmvy.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3azmctrrr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3jtrxhsbk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ncqohhjf.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3lrtorepn.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3kdlsnlxo.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3sbejviju.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3fasulkxi.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3oyicaqyp.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3omsfzxzi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3vpccbdgn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3lfdggogy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bvomvpjr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ksqlgxec.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3jptvjirv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3zvqmfzug.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3zethaxah.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3zbrubyuz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3lyezfxpf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ywowjbrq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3kxwezubk.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3lztwxmev.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3gnqrkxne.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3pjfaiubq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3uolhflzj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3tvxqjjyd.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3xtbiokkn.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3issweyiz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3qklppcfv.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3sabhsbqa.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3vvytsjzc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3vauwiogc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3fwtdqyti.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3tcvcpwkd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3nqufqewl.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3obetqsrc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3mfxrbvfx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3mafypcca.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3faajrvuh.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3lkrefdmy.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ggwfjbdw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3dmqahpib.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3qlyzuzdh.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3qpcpdqwa.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lkjpzmxr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3oxnxsizl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3whdwekbm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3porayviz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3kjmoxkku.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3iglvyaaz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3bbncxqph.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3dnutlzwf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ebwmkacf.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3avvkwuhc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zssrwszn.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3andoyaaz.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3biqqtfgh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3fwnpwkmd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3gidxzxxw.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3membjwrs.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3bnvtdvvc.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3usbyvnnr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3phmlwiry.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3gsdwnuyh.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3orbhliib.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3mtsakawe.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3dhirbnyz.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3evqdladn.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kjsfikwr.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3gicqesgc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3mtceaqaq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3hksfzpcj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3xmuanryr.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xntizhxo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qdmopxzo.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nyiooler.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cgyuxgwo.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bvrsbrmt.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3bpvveihe.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3edfvqpol.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uxaclcxw.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3yvorqyhn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jpubwcfr.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3zwdfjimu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3wvudcfkx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3wqgqveil.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3xaeumxgl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3rvhxpafo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3eunajapg.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3fkzwdhit.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3zitygobx.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3xkjauqav.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3lylbbnwy.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3lwoultja.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hrpsgovl.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ktjlutwh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3wlqvdcxt.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3kbqnzawm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3xchrmvov.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3fwsmtirv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3gfonulei.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3sihqwryw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3otxuyghx.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3chyagcgo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3fypqouap.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3royexmnf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3yzluhqlr.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3zjagbjov.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3qaofqlgr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3kbvrzdyk.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3uwgbpnwf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3agjowqxz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ekxdijjk.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ldkfziou.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3xscffuih.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3gnjczmzb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3jtrdtwzd.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3hxiwjgwh.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3sujyiokm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qjgefhrf.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3tvyawvgn.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3rlahjgap.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3lyoeyfen.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ooajdlsp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3vdrgkdpv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3cjeiwzuu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3zoiuvrbu.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3gjdlvuuw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3bfgfletp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ipnyzumm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3aghaqgsk.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3myiqlvvf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3einfttce.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3zbuxddeh.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3qxhqsgjg.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3iekqarhm.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3hofbkaif.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3erreqoyn.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3hcekoyhe.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3obxqnliu.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3tnnwnezp.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3adykxkom.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3yghapifz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3xqkluvog.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ukeruoun.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3qyubffsy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3inuznebw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3mvucgkff.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3cmvtywyu.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3rhklgmbi.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3cmwhybtd.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ncagzjxa.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3waabgbli.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3taklzbxn.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3fgxyjgeg.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3fwjrymno.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3purskkpc.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3kkmqbhaa.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sdokypvs.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3fbrafela.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3jcrkdcpr.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ecgptgmm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ozendmhb.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3dzmnxiqn.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3jckkuvbi.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ctflzxuy.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3cpkmvvef.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3wcsvckcx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3wfecarfz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3cywaxerd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ydvjbapj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3uznkcfya.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ijhkzjlp.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3jsjinfdn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3hxvpftlx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lcxizgri.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3egkcmgin.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bnhnuwci.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dhdiemgm.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3yjyfqgqd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3iqablmhl.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3oxvjrwjl.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3tthbwlnr.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3qfnywjco.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3suobfays.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3uycobvkx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3debmrefl.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3zjfxerlj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wecjaqhh.html


<!-- 参考信息 -->