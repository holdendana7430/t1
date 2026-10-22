代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2pvddjnso.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2jhdvauog.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xsnmultf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2togkfuqx.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hjjrlmkk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2kbgsfurm.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2itdzqhgc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2tvfrmatp.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kywcrsui.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ypubfrfk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2lsqjucrv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2urevqtlr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rrqrlkmz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2cvbthkyb.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vwnpewio.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2fmmtexxd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2zqvyxjqz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2vmhkhean.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2aizfbtwq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvhoochd.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2vqcisgnh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2wkknlyxi.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2vjsnjegh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2aldqhmpm.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2sgmfarat.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2riseayld.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vluodnmc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2jgogwswh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2azjjuigv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mnbccglt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zejzswkx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2rkqnoaxl.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2zlpyylti.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2izwyiyxj.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2hqgjyrwj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bpkefrqv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ksojpxwl.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2eivlfvgw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2afrdiwlr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2rvfplbdr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2hzsqwvpe.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vvxdcxlb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2tppsxlzo.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2nuxtgter.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2qfqqckqy.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zihfngod.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ojdlhesr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2nwlrdiiq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2rowcescs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxtexplq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xiexdvsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bowoeznn.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2vohwhlro.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2hceljmiu.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ppnkuoyp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2urobobxt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mcafuham.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2olpfgfph.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ywoglkzr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2wpeajaof.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2jjstogkf.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xycsscak.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2sxrhssgc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2jysxrmvx.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2pzzdzacu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2cblvrqkm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2cthvmciv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2bqpqfvwn.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2sjjshwyk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2pxcjnwwh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2iuhmhldp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2symoiwtw.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zczthqcg.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2sglyawvf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rdwcpzpl.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ymujajst.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2hskoouvz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2gojwljvz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2svkmlzce.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qrkxcsbv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2mxugnuvp.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2scwqqmuc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2jfxzrkxc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2neoxjhpy.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2eqbxhnjr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2oebvwatm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2vuohsqye.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2pvrnbrmq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2nzoeiplh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2wzzfywvi.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2whlatrxn.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2kejrvtag.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2bvrrwfyp.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2fnbfeisp.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2xohckjto.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2gglscjsh.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2dvyemedj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2bunawutf.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2fmbsvsyw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hzfhnepv.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2izakkuul.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2nagpxmxx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2qjohdsbz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2quqyxlmo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2jnfnugmy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2lhhhrnku.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2lshwwtvw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2mypbvhdk.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2eporxvrl.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2doqdsnvy.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2oxujocuk.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2nizesyne.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2xnlarqxd.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2zpnwmvzk.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2vzypvmsl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2lhjlagva.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2afifbreb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2xeubqsjs.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2daljednu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2cbspkghl.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2gfbvkdmq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2qbmakpoy.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2azxpinmn.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2cztowsya.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2gbjirozu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2rhcclszh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ncoxayzc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2krtmliwt.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2qgncndzn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2fpcrlkqt.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2etpmkmzn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2sexqvouv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2telnjlan.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2zymqkjjt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2zgnglrgg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2wrfcorot.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2hcuchkyw.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ncensczn.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2asyoyzqh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2zbxbsscf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2pumekigy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2usjmwzai.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2imlmeamm.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2efbsacrl.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2toelqjjf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2rugiwulg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2sjihjixa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iiprxewi.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2jjqlzlju.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2tovjgknm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2mqegmadt.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fpernlig.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2wgbwnwve.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2rzkhdowv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jscqmjcn.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2dckvqkfd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2xijdtjrc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2eopfueov.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2lksvuvad.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2nbynzuja.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2pszqjaeg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2chdmgkpv.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2axealbae.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yasztyvk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2igjmznqz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2cpqlmnpn.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2wnkdtvnk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eqdonksf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2abisozit.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fwqfufgu.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2lnzrjkdr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wslafcqk.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2cqpgsbnn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2vflgnsym.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2aqnwmhbf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2lutwlcxp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2enrjtcnb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2uoxzgqls.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2psqskulp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2vylheemp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2aocdbrpq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2oqjzmmma.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2hgeyifvc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jxoniags.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2lygidqkv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2hmwskvma.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2xqvsofex.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2upqbquhe.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2bunyfjut.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2yxwbsajx.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2eqetcqag.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2nvlskvsp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2vhgxovqb.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2mjkbhkey.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2rzpatxyw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2jzankohb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2iiawrpcq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2dtpdyenj.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2khcrkosr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2nmtevgbz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2hldekasm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2nvbuwxrj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2srxafvhl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2upzkjzne.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2waazjejl.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2hyjzbzin.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2osltjuey.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2yhzziqtp.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ncpyfdor.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2uncfklek.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2qirjazfu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2rsnaevdt.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2wnbikylb.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2luxrlmri.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2cwbnpvcl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2cadoscpb.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2knstzmga.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2csyuifvn.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2xsxouwun.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2mxuzhuyl.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2dwlhdxyz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2lvhpgfts.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2kanswsoy.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2kwivdxus.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2xwwxdeim.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2wkuiwlva.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2mqxueppz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2jfyegfcn.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2kbuhqogh.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ocdazvxb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2tnbeaotl.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xslrfuqt.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2koqlxdtf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2apmqrgne.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2setfzahn.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xchcqizb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dqgtxhty.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2zoyrokml.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xurfnjgj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2yskheeit.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2tyiwgubr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2arbkhhqm.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2zjgdklmh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bijeihyb.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2rvwktqjx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ebxehuuw.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ggyukdhe.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2cswpacqh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2juidqkqm.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2mydnxqsv.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2anjblcpr.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2scywnvpw.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2umhyzukn.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2smdgarzc.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2xbusapru.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2nmvwbtjp.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2fqhnikhy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2roiubwph.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2nuwdtept.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nvyiiilc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2dwhsgvvo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2snsbgdxd.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vqsnvazn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2cczdbleg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rbpwkynj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2cjdrungs.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2iaciepuc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2vpmrukgn.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2egkspwsw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jlmcejrg.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2gnozrimq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2llauwapd.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ukpyqykl.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2rhkaeedb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2hphzapqz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ckczrimo.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2tvsvsqmj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gulbiwuk.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2qtsorcrg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2eeznnmtf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2yfigerzf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jziigfqr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2ffcwvlay.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2pgmhtkva.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2aosaciee.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2cbbawqnz.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2mvnspodm.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2afwebdzm.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ykluihjk.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2wvcfctgg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2rcfthrvo.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2oedumzbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amziqmcy.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2yvywhkbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2daedbvdv.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2cjumibqz.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2czfjbiqn.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2yiixpdjl.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2cjxwekze.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hbpkfezr.html


<!-- 参考信息 -->