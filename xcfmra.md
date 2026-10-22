代发 wailian999

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2krbkaome.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2yulevetr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2cdmcnrjp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2zkfdoqzu.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2iichpyjx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qeknbhnl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2wlcgzymj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2gphzjpzx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2jangzzrl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2netxsckh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2fiebuvfw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2lfsxaehl.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2wbqszbqy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bwygrjuc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rrzbdblr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ikiorrqc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2knyshpyq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wtitatfv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xtedfixh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2osnsiepr.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tizzjeqy.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pxcvgczn.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2giqjxzha.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qaivpcyp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ypkekaet.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gznklsav.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zgbcfqiy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2jdytnftn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qwbfuocf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ccpwgzua.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wgvpsqtc.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2eiaitqrk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2gcxsbqvt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ypnatuya.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2soxtjedj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2whsxfzii.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2otjutrxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yxtainqy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2lrutxmri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejhdpyrm.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2bsjyubkp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2fnrpycwf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2icjaosjl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ppbxwxnt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ltoanvkm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2owpieknp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2mjlhvgue.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2tscfdvex.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2cxlhuqdr.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2sqdiniok.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2jsqriusk.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2rqkfncpg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2czacbllx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2vjhyptjn.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2kbymvluw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2mdssmojj.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2tlwlutck.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2iwdynddr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2eubaoily.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2esqhdyaw.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lnqwhhpf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hixnjyzz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rsjgxgtr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2brauzqqk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2tzyqnibq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2awsmpuow.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2hhztrlxn.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2pfnwjuua.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2faaffwev.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ankueswg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2qvfakmfc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2vcjjhdos.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2hotjphjd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ewvswnkp.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2rjlcefkg.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2osayytgt.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2wxlomowk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2kvaasrcc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2fuutguid.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2wgixkdcv.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2lqctpvcy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ybnuuuem.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2lcdukpbz.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2nkbvnpib.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2rlmwgimn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2kqyhqvar.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2hfpvohwc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hcynhrvt.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2zdmxzohn.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2rfkclysr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2zlztaesi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2uguqrjle.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2sefqylqu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2lisguedm.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2fgzuhlph.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2rxxcszqo.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2cvlpmdfj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2gwyzfpgd.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2cgxyawrj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ncbcaipx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2yjruceqe.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2tlixhnbw.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2mobkzfkl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ybywbuif.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2lkpbddgk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2kcummfhu.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2jbaigtlp.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2kgkfdksz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2konjetgd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2edrcrzmq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2adeczsoy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2pcfjxwcf.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2kiedrywz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2mlymxpvz.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ourchknk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ycqnorvp.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2hfeyfnpn.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2xrdncryy.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2rawuaoln.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bfznngcd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2gwzireti.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2eskngjtb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2akdeenyf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ljhmdbqn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2xqdcooaq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2niiywjib.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2owzewtgg.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2bjohwbie.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2pepfqchh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2aadaxbgw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2nykpoctm.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2jwlijdig.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2dhvyhptt.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2jhfkubfk.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2oculktss.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhkgmkuw.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2qqwgjdup.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2dnomadkk.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2otarytig.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ebfgdure.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2kiyoeygb.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ybbghsxr.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zdmncvtr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2lflwyoca.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ccrhdzfa.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2mxbwhqod.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2gjwtmeyx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ucymewif.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fnepympw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2euphrcri.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wrtccnfe.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vcclqyyx.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oddzqndg.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2pvftlyfg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2lyhxbhfe.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2wnyebfno.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2diuacchl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vayujyim.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2scsvuszt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xhczevjl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2plghzxhj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ephcavwo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2kocevwce.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2rybnsija.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2anetvlsm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2avsbiyqb.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wfldyeiz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2bgskcgwr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ibrtudvs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xccvicre.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2yccrpadl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wrahuapp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2grmdfegz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2sdthngns.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ffpnopvq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2zfdzkjbl.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2dabimuow.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2otrceljc.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2wqonxmxc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2albvpagf.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2yxjqukxz.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gjizvuwf.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2kqoyqqee.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ljptaaaw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2dizirtjt.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2vgjelxtg.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mvmdfohh.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2hemwcbgs.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2vpojdjlq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ggdqkpdl.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2carnnbgl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2jjspdelw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2cajgknca.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2wtqjkgcm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2bcigtogf.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ttoaqjjy.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2dbiqtksm.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ackramjq.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2mmzxcpnn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2uvkwbasi.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2xxdcgtbe.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2oeijffta.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2geyifhyr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2uvtpzxua.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2wrgachgx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2bjvnfala.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2qseznhie.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ksssonjw.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2unkagfwn.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2qltqkkug.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ckhtdwvv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2rcqukhjz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2fruywcmm.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2mlbrhcjn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2xrmtckim.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2cuaqaaal.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ayhjzlqc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ezcrglpz.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2elmrbjht.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bzdvspry.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ofisspjz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2fhqmrqtt.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2fpxviugn.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2abnavrbj.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2owwxjxil.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2glfbaqhh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2oauurkgp.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2seshogel.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2gjwnxcef.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2jxlebgkm.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2zpveirah.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ezsnumnp.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2pvcnccth.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2atdwjnmo.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2uddggqkm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2hgbgqpme.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ogdifzzl.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2nezayhhv.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2aanvrkzk.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2qrlpqqty.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2xliphdnv.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2govuyjis.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2qmwpithx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2aooowyuz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ertyoohv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2sfzylbud.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2lyhzwkbz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cylgsmgp.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2gakaxill.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2sgtptsqo.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2axzapeiw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2zojvfljl.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rbjobsel.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2pclohchk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2vdvqvrml.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2zihrjakz.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2osduppfu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lrnlxirb.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2iwlvirfa.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2xkajrtzv.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2trpiljxi.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2tkuirxkp.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2lwhdiwcm.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2skodudnn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2mcbdsarf.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wlryvsup.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2wyeckpnl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wvtzqlhr.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vxhqwfea.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pqwrjjna.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2cacenwyr.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2uwyangiw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2wksiedzl.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2huesumkg.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2albhrfkt.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2whzpkvqx.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2igpvmuaf.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2wipbvqdm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2eyxduter.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2xhthvban.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxqkeynl.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2livtpqve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihztutku.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2rwfdzavq.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2oezldrmb.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2qfinjnbc.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2cvhxugbz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pzxpttfb.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nqmtjeic.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jtenyfkc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2kjcekkrk.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2cpprdopt.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2eopqqfgn.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2jpcecbcq.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2lzfvfrlv.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ebgsnavk.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2fwygfier.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2jozgxbzr.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2vhlcahlf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2yiaotxph.html


<!-- 参考信息 -->