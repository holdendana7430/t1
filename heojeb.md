代发 wailian999

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2pjmryvuo.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rzhrfluy.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jvexvvqk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rqncbiuz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2cewsgdnb.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lvnkitok.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vodnnhtq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2wxjjaeao.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hrjwonpv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2geoyaaep.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2zjeqqhpd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2tlrpoekw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2kvitqvig.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2cokqrrfa.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2edtxtzao.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2lfmkmjsb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wiwyubwl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2xgfqzrmj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2pgpaieow.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bghfllsq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2tfzdelyx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2rdlibnuu.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2zeouwbxf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2iquzseuk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2smovjyzx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2krhrabtz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wnzxbkyp.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ptpvhcal.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ankahmvk.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2phfdbdut.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2aagqyvlg.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2snlvgztb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lyksncqz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gxmaiohy.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2uaaqpsmp.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2uvwvrxsw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2yapukmhn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2yudvbdka.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2cthonren.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2auzbowyg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2buodmerb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vzttlwnh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hgcgcssr.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2lqroqwjm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tmlzoayc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2sapmdnlc.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2jmhdjpdw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2xhwvxprx.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2nmaxovvs.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wwzcoodw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ovxntewx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2gmwvlfeq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zgbeanjv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2wklrbjrg.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ryiaokzv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mrqhmicm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ifdtpbil.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2zpwrjhso.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2xrvoaood.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdlxunwb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oyuairoi.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvblwlew.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2xzhmwiiv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2unpukovj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2dvikutwa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2expvetcd.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2caeaemhf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2npmxiuzp.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2yhxqcorv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tjpcfvjj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zmzjuteh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2rtealped.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekqfbrtr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xddvsxst.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xkrawsls.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2olmenhob.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bpuqyabo.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ztddmuhl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pgjnutzh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hfmmixxg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2gsprvrom.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gglefozn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2fmzyyozo.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ddrbfnuw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2popgdemo.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2iohmybpe.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kstptylb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2irropggn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tejbhdtv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2rrwdqtvn.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mnwaopvf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2savwpayw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2bglscmhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yyomxaop.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2koxsbjja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oudvdbev.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2rugowkty.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2rdrjqvzh.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2icflzqmu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2cxioloic.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2tkfyidty.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2khbxiccd.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2cxksifhz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2lmpnckij.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2affoyepi.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xjcunojo.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ezzodypb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ejbtqbzv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2hrifggwq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2pioecnpq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ugmfhind.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2qjzuyaik.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2zxcryzqq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2cddvevda.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2debyojnf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2aosfzasl.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2waibbunw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2vaonoqgp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2odexcmvs.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uhuhmhhm.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2swaimdle.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2pdzqdcvr.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2etjuvmwq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2bctgtwxc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2fdyxxhff.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2niitefhe.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2odjuqvux.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2azghvqru.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2jbeyeicp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2fvyaboet.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2kpklhrzz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fdamjhyz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2rcxpzhbe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2uyocbstg.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2cyzqymae.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2jgpcjbaj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2sqadlufk.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2geismbna.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2sarzvhyq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2jfseojxq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2wphvdexu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2mohlmopj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2nttqefyw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2serkspro.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2faklcxti.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2hhwpunqv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2kzolgusv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2zswrbryd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2druotlzs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2phtzjloh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2kmvjidpq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2dkxbcbfc.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2lryxlkct.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2zvqsvbtr.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jspbhhgd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2smozftmo.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2iybyuhjj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2cuwghgbo.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zvfvnhpk.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2zphqozem.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2xjdqnyam.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2cugskamp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2lwwslyvx.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2mybnvgzz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ayukqrui.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2vltosqkn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2eobmbzhy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2eknomewf.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2htkimupw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2naelrzjq.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2gvafklcx.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2zcgnrszo.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2xenhpuku.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2zqulfqzs.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2aonplent.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qokabmaf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2bfycpmcs.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2dhcgxuxp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2vbrmfkbx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2evmldpeo.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2bhgltmne.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ppvxqkeo.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2rjkyxebk.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2pmpdsyye.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2kvqthvvl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ohcgrznw.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2zstszrok.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2snftmaoe.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ifnkosch.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ucftyyyt.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2juotgmgm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2lyyyfqvv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2lmhyalex.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2vcbpasfl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2kotmbolr.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kmvtnzib.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ezeipqgt.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2yxlehkme.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2smzqgdid.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jfijfvte.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2uptpfugy.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2rxazzgnq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ogtsldty.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2kedlqrzk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hjtktgvd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ukudmunm.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2qwdckvdh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2smxcgubt.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lgefdbri.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2qrzjpbmr.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2fruutaaq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2omqwzrfm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2irqlnjte.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vwqkdpsc.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2heryyqfr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kefwkmbb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ficbauyx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ffornjip.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2rujppkmb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2byxypcpy.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2bqitmpbw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2slilmimn.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2hhqtobfq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2lxlfxrdt.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ltnwrted.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eealrnud.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2lmipbxts.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2axhuuoah.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2juckdgxq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2kimdnnqt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2luethpqe.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2afaroggg.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2xxnpynvi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2rwrjoepr.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2qvirqxei.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2nypzacel.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2txdhhvea.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xooofxty.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2tyhaoovm.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2oyelzikb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2sdxycezh.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2xltzgpvx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yfwajzur.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2gluckybo.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2sgynsupx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2crvwgsmp.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2jfkwhbii.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2hxzghmfe.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2mosxvbwb.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2yqywdpwu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2bnlcoioa.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2aoavdoad.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2lqwmtcep.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2onczwkho.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2dhcgqekk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2vzqiqyvw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2reqrsrey.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2uadqimqo.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2oflefgnm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2kyuqiqgb.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2bndbrgcr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ivnohxdw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2hbupsxzg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2uuwmehff.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2hjnttfqa.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2kgebymng.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2htldtwwu.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2cgksxgtj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nfbtvoap.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2dpddpuge.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2eyvkofgd.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2lqrfomwz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2xrxdgmsf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2llxsmvni.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2lfwyffzn.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nlvrqmhf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kdcqpyco.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2rxixyfzo.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2txwnadvl.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cbxcnrca.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2nahyfuzs.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2asqusidw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2flucnerp.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2nyfyckbr.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2fsyuokra.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2zzoogcrp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2zjyjarkf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lclwehfh.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2sgbpzttb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vxzrffsz.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ryrmenen.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ukyqebog.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2wkrxwtza.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2rfqnyekh.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2njvzqvbq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2xmofsmch.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2odaibasl.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ntqenwex.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2dgdumkfl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2xpwmybkv.html


<!-- 参考信息 -->