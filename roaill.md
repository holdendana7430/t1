代发 wailian999

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3rdqloxim.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3dpxurauq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3vzqzoqrk.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rvpqvrlo.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3fasdolii.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3gssgggwk.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uxifuyrt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3febmlnih.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3wvunilaw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3fmxhgqnz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ldackims.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zyjgdfub.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cwtaqrrs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3aehwitmy.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3sqwyoakp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3xfqglert.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3oceikhga.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3khsplyps.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3cteqnhgh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3episknda.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3napbiyxd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3pmuqalbl.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3lppkafzx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3cgorzzot.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hbzpjqit.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3vneviqvh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3egjvmtqf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3gafslkur.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hpltvgwt.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3plemmmpp.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3bwmztwsc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3drgnigbc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tnfvceub.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3vfbrjrdv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3frusgvlf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xwnlalxj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vocdodig.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3jadrnixq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fkipjiaj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3xrxmdsdj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3uejtrjcu.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3olykucln.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3kwdiovdh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3shdbxjad.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ebaugpoa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpgsrrga.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3sdthsjvg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3lqrnqgdy.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3reddufdh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwyipajd.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tsqfkasq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3lmiyehpm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3roydnbco.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iogtrohv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lzmbjolu.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3zgtsdxcs.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3xeczmxgp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3moiblfzp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xdqqwykg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ldqjvzwo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lgcvyqmr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jmjjsrep.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3bbzhgqwy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3znrrzfei.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3qrytifmz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jpwkjbjx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3qkwugqyb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3qchlrzei.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gksahmei.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ounykfnz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ewuqtqby.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3qwjqameq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3qgyvlmxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vdxwyhwf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yiviopro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdbpiami.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ceznzlyf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3gaswnrhj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3tdeuzicf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uhzrxjmd.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lrewqsjq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3xilencjl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3osldzzhl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3hfzemdbt.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3bbanvdmy.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vfyabvyp.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3potrfoyb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3gzylpooj.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3sxivfvlo.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3jhjxjckk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ibkhvffl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3yivuexok.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3sngifadu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ozahsclz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3anzyykjr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ctrlvxbb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hazxxbgq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nydsawew.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3lyfjzaev.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ugnpioje.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3jrtwvfrb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3iabqyhuj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3nazxbfpf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wrfhqmjw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ccxtqxtg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3zbhnqcbc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3fisyrwhb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3okdjqjpj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3vxjoiryo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3cfjxjbgg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ltmdddux.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3fuomrkhq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3qioopkeq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3vxemzhxe.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3qyxwcvbd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ojnvnfud.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3vskooasj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3qasayase.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3efylcswk.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3gurlktjc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3rgaqjjhw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3dsbjvqmf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3rujoyuhk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dwvsqvlb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ibuyutyj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3puxunfqi.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3afldtwkx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3npixujzv.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3xjvmgnjf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ttszthvl.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ccnccota.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ibaqbqlt.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ymfxpdhc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3hbfnpyqx.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3jroeqxtw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sefbkdby.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3gngwljjs.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3epjqjvvf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3eljhumhx.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3rugrxeeh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3uffdhmjs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3mjwwfzbt.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3purlagni.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3iocfqbnh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ucicyzep.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3blfamgzh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3nsuxolsq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3pierfhjn.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3lfzscuys.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3nqgrpddc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3pfqrlmxg.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3sthnajfb.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3pyleocsh.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3xvirvfyl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3zkhrzqah.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hvtmyfae.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3wxdigvsd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ltbmwdrm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3vlfmevrn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3romwwpeq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jnbuhxet.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3hmpacnqx.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3tmhazhlw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3tawwkwqj.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3bzermxco.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmqmwpmg.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3eqbktpco.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3weoiunov.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3txggkusj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3detcjgpz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eqeanybn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3kzemyaft.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3tdjjrect.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3jyivjnaf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3etxbdjiq.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jtfxctns.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3gsrmqogg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3vclkmiyt.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3etgabvmn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3gnjlpocl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3vmzduypd.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3nirvzxzl.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ixmdpxnu.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3qykaiiyf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dqwzuppo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qvsfgtxv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3rvruyctr.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sqslrzqx.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hfqvgfjp.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ahtfshbk.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3pqgruyao.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3dyivyqxz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3bjlqsowp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3rxmdwkpi.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3rgnunxhk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3zbzlkotk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3gakakllh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hejehavb.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3xihcsbbl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3pvvbxrni.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3tauvrvbh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3rwpucguv.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3zzulmcoh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3xskrdmin.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3rjotiwmb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mbvtjssx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3mjckqwom.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3efrdxyap.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3bqtgwfzc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3cehtxdup.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3lhoruxxx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3bieepfbe.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3fbsopijk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3sbbmytmp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jdrbzrcy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3rwaywpps.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ffndztgn.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3cgngcxlz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3qmuwakho.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3rflfbcnb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3etsffkee.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3mkglodtq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lzsepkmu.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3dylbkvme.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3elwmjpsb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3jabpogkp.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3cdykrwpa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3neuqpcba.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3qhgvhzvu.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3tozixlqt.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3tviggtzg.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3wqtvfsbt.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3hfjrrtpb.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3jdslskre.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3wloswypb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3edgnbact.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3bfimsdsa.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ojvbhlki.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3hlycspar.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3htqhkepn.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3merdfxwq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nxwzbjts.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3mevcrssg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ktdaekjv.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3qeexgpua.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ratyzsox.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3elekwhzg.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3eyigdbmv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3wammpviz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3sgwpthja.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3xwdowxey.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3hscjzcfq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3wvccldvp.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dhcvlxmc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3wvdnszme.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gcfeqdrm.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tentspze.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3yaitddki.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3qpnhlqrh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3dqrbgspr.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3robfnhed.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3tcmtljwy.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hjmrvvqs.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jtkgtpoy.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ptstgcjr.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ldcpmigg.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3eorknpje.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewhsfcid.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3jzhekutn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tdyqrxjx.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3cikoiqpc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3fqliqurl.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3dhvmuumv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3iivyoxtc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3blsbfutk.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3yxaqusrc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3huyzrtcg.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3zdfowsrr.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3hycwrwjs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3terldgwd.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3gubufxuc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ismtpecq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3tgopjxjv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kwcyniph.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3fmnqyyzr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zcqmkbdu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3iekuzyfv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3asuvzjrn.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3pqbsomzw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3keziusnk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3bkatkefv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ddsheias.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3wzguyynm.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3rqrvfpir.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3cwdupiht.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3gjcffcyk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nbmxaanc.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3pofnqkjm.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3cywjggfq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sfgofqbk.html


<!-- 参考信息 -->