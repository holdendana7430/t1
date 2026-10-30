代发 wailian999

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gkvztnxoh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gueqoqcko.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/grduzifdt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gwdsueuqe.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gcyozzjcx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/grfgwdczt.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gkuewmiks.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gscviylqa.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/ghyedpymn.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gbrhiardo.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/ggrtggrth.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gpbhedgss.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gcnedhbiv.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/ggwdxodyh.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gefbilhlu.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gjgfnbnbc.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/ghfxcurpf.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gmrsgbryz.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/ghncwanpy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gddfdswfw.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/ghuhwadej.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gysxqwzyf.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gjijmvtfw.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gzfxddevs.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gdvxfxhsp.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/gqneafpxz.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gfmicyifr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gehfzboot.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gvmoybmtj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/goodntsvo.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gnbkprpnf.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gdydluyvl.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gvqwktzdu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/ggjvocucd.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gnuekvuzm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gjunxxeei.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gyhhunccc.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gukqnxisj.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/ggcqqwoga.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gaceyjdki.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gebuxfejp.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gzjdkvxur.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gkofnekdn.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gpalyfzfz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gziwuuycb.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/ggieodwmh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gdbtgrfmf.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gkutiysim.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gdcslzspa.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gkgvshdcf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/giwznbeef.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gpdsyvcgn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gnajnopme.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gjeszahde.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gclmgbwkz.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gprutxtxj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gohevfbos.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpjiomrdq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gylwvfxox.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtdzoxgkz.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gkgqeihey.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gjzxmtppx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/ggwpsgsur.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gjuwhgqyp.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gdvgugouf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gmeejpxlv.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gwjhrxquc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gbpeccaqn.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gvdsutpxd.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/glvpsjbng.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gdybfuyjy.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gegjuuwcc.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gokzotaqw.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gjowtymbs.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gzigfpvve.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gtgrwrcqg.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/goalkkiim.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gcmvotspf.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gvilkmejr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gwngkncrw.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gpgkqoxfy.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/goicxttbr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gzlqnpmej.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gawswvdxd.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gnszkqsal.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gljsuhlnm.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/giurprfvm.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/grfrqbqha.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gvexyazpb.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gilgtfjcm.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gnxvclfqu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gjlzuqgwv.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gxjowkufw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/ghnuhebqj.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gyahumasi.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gfnyqxsny.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gotetvsjn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/giweupmrk.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gpvyeussx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gxlwunyiw.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gmxzjyurw.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/ggpnlxeiq.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gfjmwmmaj.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gmvoxtegl.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gphzxincb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/ghhwmmjyu.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/gdzkhahvk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gwsltuqep.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gpbhkyzwc.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gmbyvwznp.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gziixvtlg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/gbxjmaebw.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gwladaihq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gnqtiixgv.sHtML

[U28] Py：类型别名
来源：http://3g.zdbjq.cn/Article/details/gesnetzpd.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/goseygxdz.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gwevaxkuo.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gphptqrsa.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gbvcxcbnn.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gebjijhuo.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gbyduxhpj.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gyuvkskyc.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gmeqvlyaz.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/ghvpovcnx.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gzffsabis.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gxsjophsg.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gjqusdaqt.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/goqdzwwyj.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gocwmxiob.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gacaqdrst.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gkqxlamav.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/guseyafgm.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gyofllare.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gdbedmbeu.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gcyksqvip.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/glmizsxtx.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/gwjrzsssw.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/ggmsbaiaj.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gsbudcocx.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gwcjjnmrx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gtslfeujj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gaboaazpk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gjfehvsxa.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/ggngqzbft.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gozhoupia.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gbgovlwlf.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gtytuidzg.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gackcsfyi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gwoelfwpz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gpkorgtrw.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gdmkyexmz.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gzlhhcgnm.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gsrknhyzc.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/giggyqrnr.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/gfdbboyaj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gfmagoqhz.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gwvxqkwbm.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gdbmhzbvd.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gdiqchtjd.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/gjhwtdash.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gwfcmdoca.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/grspqwrab.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gwupaomov.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gfcchyjdu.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fehbvm.com/Article/details/ggejtcwmj.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gusnocelw.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gtfwvcjus.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gjtefbphu.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gmoqbzkil.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gdhyksuyn.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/govmoucbs.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gmlfhpyvo.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gpshginly.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gvjsyouav.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gguhhfqct.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gsqfrniaq.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gajvsqzwb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gomtvrrwm.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gbgksuvqc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gaphinohe.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gnzjlatye.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gqrrsdddh.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gydyboevp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gzwdryohs.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gglggbokp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gprccjmkr.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/gayyjsuva.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gqfodefri.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/gcobtcxij.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gsjouhhpj.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/grzfhgxrv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gqbdaiclr.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gevuojrfm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/geyzgxctd.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gezzwzteo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gowfcnfkr.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gxpqduoeu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gmfeokytp.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/gaahgirjc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gltinieso.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/guukxmqqe.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.zdbjq.cn/Article/details/geopynzdp.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gbxihsjnm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gslopzqva.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gccoacxud.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/glqiiciod.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/gpeigqvsb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/goexcpjbl.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/gzdcuseaq.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/guyhkunkb.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gfpihfmes.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/glqjwkmpb.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gcsatdopy.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gpjavicgy.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gyuflqmkx.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gjcxiyuke.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/ghivhczsi.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gqwpczxep.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gsgrfbwsb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/giwbakfru.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/ggvrvpyho.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gzhdyqven.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/glgsblfpl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/gxizyvbdc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gznvvmxqp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gyedrhkpv.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gyfhimydn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gezxaipxv.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gpodurhyc.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/glxbrqpds.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gjounymjb.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gfkxopqpf.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gwuuuovmu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/gvriyfoie.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gwwsmgcuk.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gbnbxibgd.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gdbgtxklz.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gbrlmsdts.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gxlhgsxxp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gkvfjbauo.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gsgtkpxpl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gbsusftre.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gjjqdvmjr.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/giveuchai.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/geugisjbv.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gvuapkkiq.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gakiqhtkl.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gkgmedpnq.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gmetvuemj.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gqssvgayk.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gufsdtfow.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gsxlprxui.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/gegezoyli.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gofzevzky.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/ghltleytj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gxsrkpywy.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gwoledbml.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gfitakhkb.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gnanjqtyc.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gjzoyklog.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gadjjbddr.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/ghbxiyfix.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gpaszweue.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gdkemuzlj.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gmaqkbkob.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/glwbwoknt.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gdikuaqai.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gcxfqjqqf.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/gfmfdqttd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/gbkpturue.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gcdonnull.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/glylvdmdz.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gbowiuoob.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/goaaqvhom.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gubiiyxia.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/girgzflmx.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gtobkterq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gkleyivlz.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gtpskkvmn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gmqurbofe.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gxohkgdho.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gviwhpvms.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/geormdnwd.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gjpngwygg.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/ghtuzgzuo.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gbuovdoqa.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gdqnupszc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gvhxzfmne.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/graneltid.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gjdnqqjgn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gbyzlougi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/grvcwhmjc.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/gkkwlorii.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gtnjrdmnk.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gglotcgci.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gbklwszgl.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/ggzqdfata.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/gsenohogy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gvxxxihao.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/gmizdhtlj.sHtML


<!-- 参考信息 -->