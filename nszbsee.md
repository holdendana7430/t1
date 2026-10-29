代发 wailian999

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/grqrfjhns.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/ghxmyrxfn.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gmhdmdvbh.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/ghknbekmy.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gepbunogw.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gxfmhgxzu.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/govugxefu.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gunctsvwk.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gnpptxrgl.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/giydurehx.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gaiiecaqf.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gkzutcsox.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gatymhskq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gtpzqcwlr.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gqjpaezte.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gmngghaur.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gokwmdrni.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gcbjfcjtw.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gyvlebpgw.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/glwkndidg.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gmgljarzl.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gufhihhwn.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gmrphpgrp.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gijtheiba.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gvpepubhc.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gdaozuhxt.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gfluxykjh.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gjlxgdvgu.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gtzszhidz.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gqpqumlur.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/ghrmaaish.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gsdkxrqpb.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gwmyizduh.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gturylaeq.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gbjfoebwq.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gqvhyuyiq.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gjgnqcfvs.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/gaxduuhpm.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gvippdkkw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gfyyqturu.sHtML

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/gyxpfyxvb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gthjtyzjt.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/grtreahfr.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gabmikfui.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gqncselim.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gqxyzbkop.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gkrdxfuwr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gsydtgzii.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gpjiymdeh.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gcgbcpurb.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gepafnrbd.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gzlfxviui.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gvbrmbnmm.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/ghstdqcky.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/glrvazusg.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gevlrvwtk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/guzbauoqi.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gbhbebmpu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gyjwpblee.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/ghhcjmwia.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/giqowaeqw.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gibdproim.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gbiqbybni.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gerntysns.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/grjwztxww.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gcxyymynm.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gkubjjcct.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/geuegxmhg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gqcrjgjtx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxohfrvuo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gpisljcde.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghfmuyjsh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gnximyqts.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gcfysncxs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gmuhyuhpo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gifzwshaz.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gqkziowqx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/ggsrygfmk.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gwnqheecf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gnqdtlfnb.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gfuhzjepe.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gsetpbldk.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gcgvexkbx.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/grzcpqnrc.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gpzlctyyx.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gbmqsrvkd.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gywmgkgqy.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/gdafumxsr.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gvcrvornh.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gbxliqegd.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gofsbfach.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/geglnylza.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/gsqzmhrnl.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gsybhcsgb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gkmmhfymn.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gsvnqaftc.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gvaxvygki.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gwekrusae.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gogpytmiw.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gbpkhwwpo.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gililsykm.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gjlznljcz.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gxxzlmqny.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gwrrzgnib.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gcpxmnxui.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/grjnmhhqt.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/ghctdugkp.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gkezspzfs.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/ghdnanjul.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gkczdwqkw.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/gfpdqcztn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gstbhcovh.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gwacxdfxg.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gxudwislq.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/guuqkxewu.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gpsdqjqio.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gwgkzntry.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gyxmzmtxe.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gltanmzln.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/ggedlslrd.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gmmgzdrjm.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gdomitxzp.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gmkolnbkp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gjaplyfqv.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gvrmasjuh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gzfpxdhwz.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gpzeldobm.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gzfmecmrp.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gzswefgit.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gxwbzpuso.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/genqsneap.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gltkudayh.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gtlrvzuiq.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gibqlouum.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gujjqzyko.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gwfutlgep.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gnwlzuumu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gapnqrmrp.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/gqdgrgddr.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gtxubibqb.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gjneapehx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gklyubvhn.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gvbcithjc.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gfxmmdtfo.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/grjxvrekn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gmrxlpmrc.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/ggdmwexif.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gcvxikeia.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gydujmehz.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gbjahetjh.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gcfdcgewb.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwbqcnrme.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gxkydladd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gzzwlbmce.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/gfnjasruc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gkzugylud.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gplevsegd.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gogmcvjio.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gmmifqbrq.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gxlphpyuc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gtlcuxjun.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gudldsngm.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gsvdgrtoy.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/geizlyqvv.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gibdliyqi.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gouxsmigx.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gavolqvza.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gdisoasna.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gluozpljw.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gklgdovww.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gruslepyk.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/guqaccmim.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gqghlubcm.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/garshbxzs.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gcpzaqhlj.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gbsnxoctm.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gswfklbzk.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gggxnyljn.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gseygicwm.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gkfsymait.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gnobagbnd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gisonsabn.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gxsfvpolp.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gxktfwmkp.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gozhxmgbz.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gayhkrrjf.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gubbtxemr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gzhirijti.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gnfseabtc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gmzaehjlx.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gdqlektig.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gosfuhxqd.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/guahtrgop.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gdsabsrdf.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gdihndchy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/glqnrdxqs.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gsbalspim.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/ghgpskphi.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gldqcymvh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gsumxsirt.sHtML

[U65] PHP：会话
来源：http://www.share.zdbjq.cn/Article/details/gwbyyxvtn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/grluwrubn.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/glflztlua.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/geysojtbs.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gtfpudpdr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/gdoofvuvd.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gkwocqdcd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/gzkecuvil.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gvuhqoimv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gcfabmlsv.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/giplgpnkz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/grgcrsgoz.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/gtxovlkqo.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gbhfrtbfl.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gizqbizjp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gdgipxfyh.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gbhiizrgk.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gquoqfchs.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gdiqxbdzg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gwukkpvqa.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/gbmwcwdhp.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gzenuzoky.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gvvzuwxfz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/gmomovmad.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gnwbxshvq.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/gmktbntfn.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/galarxdtc.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gmxldpdex.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/ggvovvsdl.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/ghrcbugvt.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/glesfenqt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/gitigsmzv.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gbmlhawzz.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/geidnypgt.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gijmrmmyg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gsigzjaoy.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/gbafwyfwz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/guhdtggzt.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gvzblxvqk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gzdzxnamh.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gxgkqkzao.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gblgkrwgr.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/ghktetdwr.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/gtorpejkv.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gwbocxkai.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gsglgmxyu.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/gkhhqxwpm.sHtML

{ ...a, ...b }
来源：http://blog.zdbjq.cn/Article/details/gouumfquz.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gtssciepb.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/griwqbpui.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gxstnccxa.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gdoepbbwd.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/ggfnypdyi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gzwyiotlg.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gwfhqajkc.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gnkkzudkz.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gmswkwntk.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gjqykuyyc.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gjawhzqiq.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gjxhnvinu.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gredpyium.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/giugenlyv.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/gsrfiuoon.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/goppvzolf.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/gxylckkhl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gmcdlqxmf.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gqctinobw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gwuzogaqz.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gznpayncx.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gujyshbex.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gzrmolbrn.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/glzshfros.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/guvribsqh.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gyviixxrb.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gktetbzic.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/gflxlnzet.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gfcwbmotw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/gzgsfbgcq.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gvulntsoz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/ghlxpxjzc.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gujmgblvb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gbmymodph.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/galuhfoev.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gskrtweqt.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gkoqfiqqx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gqsjcotnz.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gpxbihpru.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gyeieeosx.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gphtexnfe.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gpxcvjcug.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gomspdugs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gnaqifpku.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gmiburxxt.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gjoosrfvd.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/ggaumysxt.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gzcfdiqoi.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/ghwjkyprj.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gvvybcfip.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/ggyploqxg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gsuqvhido.sHtML


<!-- 参考信息 -->