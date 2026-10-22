代发 wailian999

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ixwfuxsp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jriiyagz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ifrkjsvc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2exkbdxey.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahgvpext.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2epodscau.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fqgddjac.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ounmmpgz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2icuffdfl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ykclqisx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hixdmnqq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dnghdiqy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2awvirive.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2btshqpcy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2djjvjryg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2nvwrwhdi.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2brlcesxx.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2dgxlqnoq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2tfyjhich.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2tainjusk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tzneuppd.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jmyjasek.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2slhcpodv.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2akwbkdzw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2woyxvlkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jkvbelel.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2axudckxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eznhpbdk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2jykbuvwm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2bhouvavu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2upchoslc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2idwcjodl.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2uglilifv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2acndastc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2gdcsersq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2elofdhwc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2iscufdwd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2iewgxizq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2dtmqfpta.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2mppdcync.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2gpsxqgot.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2rigctbhr.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2qdojyqag.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2mloybltw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2uclgdjym.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2hgdsswpb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2helgbzeu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2cbczzpnv.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2nlaffruo.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ugnilpqc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2plyucwyp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pmdvdumx.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2fxrmyafr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2qrzyavit.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2meglnong.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2lphsauck.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2uaygjtbc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2igjrrxgy.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2urfpgxbo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2pfemzjtx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2dufyazfx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2zxhwqftf.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2xjmvnzah.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bezrcofq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ikpnqgvf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2erfadxmy.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2zvdhybls.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2xniupwca.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2pdjxjwry.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2zaegoevb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2zmcjqtwo.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2apwhuleu.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2inilbsmm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2dedrvwov.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2jenwloxg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xeerpbdi.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ierawmgt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2hjhihrbz.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2zygiubdm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2jdkostaj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2zadahfal.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ngxndlnv.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2rfybokve.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2alrejpry.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2jmdfszsj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2lihlvtfu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ylcxxcvj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2hrpheuas.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2xtcjezxl.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2cukzfbep.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2kgdgxctu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2dhspynvw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2lytxpcls.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2cakyudhv.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ngbraqcc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2npnhgvel.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2vxgwlphf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2rescaxbr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ccncdxsf.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2gbhupkft.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2rbyncgsf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2hrkfifgh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2jupfhnxr.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ooopgzej.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2qrzyisxh.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2fnuqvhri.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2asxfmjhy.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vgxwfcck.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2oemmsfdi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2dywbhdma.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2gnhkxlkt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2noqitoqi.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2zkjvreum.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2fxzfmntn.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2auljjztu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2tyvjredh.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ciwavllq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nvllsdvs.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2cwfncmwr.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2usgdalux.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2rpjsenmh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2cjsfqacz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ixvkynyk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfovjkie.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2xzfmtlcv.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2mqeahbam.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2wvmxbrgq.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtwgzzbx.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2rypphcus.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2rmqaupwm.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tfrsorxs.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2xnilooat.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2eofuotsd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2tbqsygua.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2uyudnuyd.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2tintltmg.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2bihzcrbw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hsqayrpv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2bkwcelhu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lnzkhuwe.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vunsrvpp.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2oqanqvjm.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2vdfprpto.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2qbomdbfm.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2wzpumvav.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ruiutpbm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2wnrmrdtb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2rvknzctl.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2fwczbtfq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kzepcstq.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2kgofzdky.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2rkspvbtz.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2qhdxfzks.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2dpterfjd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2guyzjngv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ygddwqyb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2sjabmyif.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ddhpvspi.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2quobwapi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2andrkznk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2tfuqycyo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2rayzqulf.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2gvrbpndx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2tuknypro.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2cqwmsmkp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2mkmpexyz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2trhtogvj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ojcyvozv.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2qtdrpook.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2qxsmtkbv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2phtepcso.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2okqfjqcx.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ayfofgrp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2vdotjcvv.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2tvcxfotn.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2grjvqtav.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2loylhyjf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2brjorkft.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2uipbbohe.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2dlxjqtrv.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zcmzcuap.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2rlqoqqeb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lmaxaaqm.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2llzgjlol.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2bkhzspxy.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2zsiazoeu.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ndioepot.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2eqfxhphr.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ogwsbemh.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2dcjbufmq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2kqofcodx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ikojnctn.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2vfvvinyd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wnrmvtbl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2sxtwzkqh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2rwjlwjgy.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ezmhlxom.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ftkknmwo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ysbdkjld.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2remxkecl.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tqdtpnrq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2juurptsy.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2uxbwqisi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2dmephqxl.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2lqewuiar.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2izguvvqr.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2leejycut.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jjgcnvjl.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2trwtptmv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2pozksodz.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2buulryap.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2eoorojvo.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fcrdeilt.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2qsehruzq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2pqxfpmfs.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ppoynjhp.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2ffsjejwq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2pewnxhrg.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2wupjvpiy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cyukurbb.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2odyduqix.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yxhiormx.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2pccfztkj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2fwfeewgn.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ziyfjsvt.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ouhgnjbm.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2kvkraxqu.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ouslurko.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2hraobadb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2eeogywal.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2vndyrris.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2gechrqoo.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2jicisysk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2tsbtzsjf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2wuvbabvg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2liqarvpe.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2zktdtfdb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xlpqrbli.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2meqvwrzy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2bwoqrrcl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2enhmctem.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rzyfkqac.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2jpcaokxd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2pdenrgms.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2sfvjfytn.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2vswihmns.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2nzpnocxy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2tivsdkhr.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2czvsrksj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2cujqwdcd.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2xlqdnvys.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dtanrocv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2gounhumr.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mjeeodui.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2xdxgogck.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2khtutnik.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2tvanvlxe.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nafjufrl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2joxrnbgy.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sudbguii.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2znnqutvh.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2tlayqeaf.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2qmvuatfi.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2vphgnxij.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2yuvgpjmj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ijmdhbzs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2uxfworqq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2qzjsvfzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vimkwizj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2qduxvyut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mnmkzrum.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2mxarsfxk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xdsqatsj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2obkxzccj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ihyieqlm.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ndkfhtjc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pcxyfcar.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2vojdsgop.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2tmfupkvx.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2alzuuqaj.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2huxxrvsg.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ungnraym.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2uvwdjwvq.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2znwruvwm.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2txddykgv.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2kavibeih.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2udyaexma.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2yicjppih.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2pwamepbc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2acemuokw.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2isjxqebp.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2eyfpufeq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2mhiyhfzd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vveiyrsu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2muehtwbb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2dxmliraa.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2igsqskql.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2xkqiqjdg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xipxcntp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2dhcbfadl.html


<!-- 参考信息 -->