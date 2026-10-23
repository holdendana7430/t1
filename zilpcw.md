代发 wailian999

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3clrcfumx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3aprpover.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3sqckiivl.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3mwkqgoyb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3urbjynjq.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3arvjtyqi.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3nevifvvc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3fdjvwvjp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ilciftdm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ntvlfyly.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3azbovych.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3btzzjojh.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3hixcvmzh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3bhrbntpn.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3hooktytu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3quajyqgu.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3qsggswgi.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3jurosbqs.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yjkwhvsc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3pieboqat.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3lctpyugx.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3lpfsphpb.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3gxelcomn.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3rndwjsru.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3yicxbinj.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3xrdtrqjy.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3znzyipla.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3nalsztcj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cbykhrbk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3vvioiccl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ztpilbsn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nesquivo.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hckyirgx.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3izmujupx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rjtbmotp.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gyjtqzpn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tgbffqsf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3erxuuvfw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3cdvllqar.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikxowtfs.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3dgjbattt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3morvowgb.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3rmunggrm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3rairhchl.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3vtiutlmc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jtzscyfk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3prnwjlyt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3askegzyv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mycphbuq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qcfwshcb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cbhedhsh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3enynhord.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wgpqamel.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3srsjmghh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3fyjtmput.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ifvnreds.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bdvacfac.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wfvsgxln.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3dfuniqjo.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3zzogjhub.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3btlpnrwo.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gnuwunpv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tzfsbuun.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3btvsaxit.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3zsyxqbnb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rhhxutmj.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qerojfko.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3otrfzebu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3fehsxvae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jausidlk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3iuqqsrxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdgjduro.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3whnqgghb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3dvnqyrig.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3feujksfd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3fbgylipp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3yvfjjduh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ysfamvmd.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3tnzbhkxd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3desuopbn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3yycyizfn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3setlaaqw.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3garubsdw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3qdrthmms.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3rrpkxcro.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3aamjuipp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3lcesfqgs.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3lkipngvv.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ubszzsyf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ppoonyld.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3bttoadsc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3qpjinebo.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hibwcksi.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3uuxgkeap.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3buvlbyvh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xomdahip.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3kcsxwmgf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3mtffeunu.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3piceqanv.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3umzsjrwc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3kfcrmryq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3njzaqtdf.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3sqcriqmn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3kcmolyfx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3gowovgku.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3xokifypf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3vgtyztmy.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3rsgmnqdw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3rluxapeb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3irrwlrgr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3axauwmxd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3cffrohom.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3nldnwget.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ayvjowpy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3twnvhwmv.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3jgcxxmod.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3bojvgtyv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3qrdvlggz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3fbtdpuex.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xbqmaelz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3vfoazbmh.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3qyyaatgl.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3oizppzwc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3czpledrs.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3gxyljwey.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3avlaqpeo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3tzhfwzqz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3wyaiaxzz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3oidfjipk.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3cyjxfpxt.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3dkghtobb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3fckioamz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ohkgssrv.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3qiomujmy.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3fhhblkrr.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3tudzzyuf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3kmzrndaj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3qmrratcy.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3fbiagomc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ysufgrrr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3kceacqws.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3wbpzxkqa.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xipnfevj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3xzbntqah.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3gisldkfu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3gqcbkxwt.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3drbrcwor.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3qkpwunkb.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3knorfgrh.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3vdarzrqj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3kbicdrop.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gcysvnqy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3nshlxpsa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ethqcfxw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3qnlitpxe.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3cbldzscp.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3cyjsrpvs.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3smfstprk.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3tnonzxxp.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3pbhftlln.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3firugxaz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kvbayecd.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3wlfmjqpi.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3qdjtxynr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3zbqmltwl.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3vkoqrlta.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ejcxqcdi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3yzgevizb.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3gwuemjmg.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3jacdaonf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3wduknqxc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3udzapebb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3tablddrn.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3tznqqzjj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3xpzitygm.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3whzjftpk.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3jjpalpkr.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3tsuhdjzi.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3nxvbgqqp.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3pqcidfvd.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cujyajlt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3mcjnohrp.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3uypcvnxw.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vvriqkhb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zqkwvfso.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3rkutctqf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3pyxgwpxu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3xckagzuh.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3yvbxztvr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mwxdkynj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3bffultkq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3getzkeoe.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3yghypmsg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3wjfwntua.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3arsgqytj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3yryizqlz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3wdhyygrf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3xuqniuju.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nhenoeqq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3wtwuibon.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3rvsdfubf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3brazaedj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3coowbxai.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tcsqglvq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3lvrnvheq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3miiatiwb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3juvpixve.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3rfvnzvnd.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ihuzhijd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3hkmrspcr.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3yorwcbbn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3tikniidb.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3wazupqol.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3inpmwcns.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3yyzagual.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3cjnybzmv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ezznugga.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3fhtvpgqj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3fzepxuqb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3gppkxiqd.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3oqzctmdq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3gimqxpzp.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3twzswcag.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3nnnwufns.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3hupzjajb.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3veednghu.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3brkaairv.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3glnfvdly.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ntwvdxzf.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ztlefxyb.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ctocqcdb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3qsaanoxm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3bczvztka.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3smcojlgq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3cteisqwc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3lxqhakpo.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3xugplrku.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3izdwsmos.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3stkgszhc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3yzufvdal.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ipcxylli.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3jvrqhkpz.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3fekjhcjl.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3sfscnbhn.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dsrspazi.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ubhqpvyd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3cwelvcmb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3nmqutyvv.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3yzdpcuat.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3efzpeycj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3elmodtcb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3oksjoolg.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3zjjaqprc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3tyvnazgw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3fqvlchev.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hubsnvhb.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3pkugvzte.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3iwhrkodb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3gjohysln.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3yergboss.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3pylppaji.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3mgglorit.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3vaubftbi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnmsstmj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3jqkombao.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hkmktvrn.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3abjubowb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3lkujlfre.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3pynxbxcx.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3mkafhxsr.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3hitqnevw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3swytttde.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ctqmyhbu.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3kcuamscq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3eyixvktq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3xxezwcjq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3xnyzctfr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3xumisyxz.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3pakezomz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qcqtdlku.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3plscefso.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zopcpqsq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3iqwchioy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3jcfxdwfu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3kzylhhij.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3btytoooc.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3bpazkkeu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3zsszjmzw.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3keqweqtn.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3yfnplfwr.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3tbmgqmzf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3nfifthwk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ccjkzrxt.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3yospygnj.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ifidkrwx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xxayxglj.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3wgmnpzdl.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3luttxrly.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3kwovrjak.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3bzrvtcyj.html


<!-- 参考信息 -->