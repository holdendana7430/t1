代发 wailian999

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2cfjtuotx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqqncqyp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2uarugjqh.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2yeaipeqj.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2riwjtkom.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uehpayao.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rpotklit.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2aciidulj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2hrturags.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qixzychc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2udwmwgzy.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mzrcytwn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2bkvajjmk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zydatiqt.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nzhvixbc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ybhpyrrg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2gljukovj.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pqlwvxtk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2nwtelzed.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2hgxxasgs.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2eatsebfw.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2bxctykzw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2vrspdmhs.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2dfwiekki.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2moophduu.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2rwrkiria.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ulgvcqlg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ydnyikot.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2dgokdmmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzuuxwrc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2udjdtuix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cszkzqsg.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2aaksjbyt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2kvfhdayr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2iheeiqdj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ffqgamfd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2rggmpvjv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ykxflooy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2xvxlwern.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2oenlcmnc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2tueuwfbj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gmnczbgt.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2jytjekdw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2wwfmwemp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2zlojwhwl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2vcacevjm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2mefqdzkm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2nyuizgfz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ygqijmff.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2jbrikknd.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2avvwigag.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2jmrekuxb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kgyidovv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ioqheoin.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2gqsrufec.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2itdptoqr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2rdxufylj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2vogixozl.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ygphkcnr.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2pvekwbih.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ycvxsomh.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2kiohxvnl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2krzkfwow.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2aitawtak.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2fehtscvj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2enwxqqye.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2jdyjobro.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2zqgeweoh.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2unxkrurq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2zypkwiai.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2sgviyfhj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2jwkgttwj.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2brequucj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2wpmrymor.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2iloadqkg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ylqdplwl.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2bmfqnxpb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2imlooozc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2hblvvkwy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yzajgxra.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2zftjdxap.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2hlbyecre.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2mrblumgn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2afaffjcs.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2dhnjqzpq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2achezlqt.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2zknehiqr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2vamibrfd.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2sfvmnsvz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ulqeqniu.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2dmmovyhl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tnmyyfmr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2bfiicppb.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2anrgzsoi.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2jxzbcvub.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2kgoehodx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2oarvfdpw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2djzsbnqu.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2yqrodrhj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2vpzfbdxb.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2xltmwtxc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2gswhdqde.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2whhttzyh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ogtceqgm.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2xgppsqoi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2bmbbapku.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2shlxlzgc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2jiuiwxhd.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2smrehvqz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2mhizqdvo.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2jgsxhzzp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2dlzbleif.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2cabwufbk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2hgfzdqxt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2grhnlodj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2rjbkwxmb.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2spdjidlh.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2btswomkb.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2pdtjralg.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2susheirz.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2pvlmifoh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pmshhejl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2jfyoyelh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2elmcwprf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2xkkxhwgd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2hsjvqvnj.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2cyfplhis.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2rugsenbd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2lqweofks.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ymivreqd.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2jctiuwzb.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrqvjbmc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2vuazptij.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2jqwoyxlk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2jpjhizlw.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2prqfxffg.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2esggjzto.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ffjzlaiv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2iggccbvw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2awoavqye.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ezchgvri.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2xeqsggqh.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2zhluexuy.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nlprmrqe.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ftqrwqpp.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2dmtqpddp.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2sbrjlvbj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2widetcet.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2pyjltcnl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ywovrqup.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2dzoblnqn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qwdwaiek.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2gxdgkgqm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xfpbsknc.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2rugxhoeu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2jzjiqwpa.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2lnmevakf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2emgxggun.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2cjzlwjrk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2njlzbpqr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2mjdfnbtv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yaloblpq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2xsootqqr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2amvmwkuh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2pjasudcx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ovoekmiy.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2wmuviroc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2kxwybhqg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2bepkidba.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2gojdamkk.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2gklvdlto.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2vclfrrdh.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2twebhthl.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2mwqbaudu.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2sxqtuuqs.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ybynrkdi.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2kljmibev.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2jngmjpys.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sdodxfwx.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2cvpvcror.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2rmhbnluk.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2znyyztdi.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2feiphtnz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2aqxoqdqp.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2sbiddgdm.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2hxhajnnj.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2cbfqghxs.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2qzyxnjdt.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2kztfanwk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2zycfthth.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2wvdoyszb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2jmysbmnt.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2vaqzdegy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2kwmslzdr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2wgrikony.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ijiugeyh.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2tylqhocw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vgnvpyqz.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2qipokgaf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2bjfaghmr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2mxbrmfnm.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2fbthtnqg.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ycprwhih.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2qaycqbqo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hbdhxslj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2nlmyrofs.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2yqeuiaxr.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2inkrqtrs.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2xctdakoz.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2oydbdogi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2nqmyoazp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hcbxzrzq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yivdaymf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2xvxjdwnq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jvmwpruk.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vjfzghiv.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2zeaumrbh.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2chgmrcqy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2wqwlmwfq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2eukvzdbn.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2bgsdnhbd.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2zbzcgtkn.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2iorgvjqw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vdvtrjcg.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2vhkwetey.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kwtikdnu.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2avycsrpa.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2kothcauv.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2lwjdvezf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2cqoavdrq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2bhtmnkex.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2iphctbmp.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2kpcwrtlm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2qkmosdpb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2llcoqshw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2gwhjbocx.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2etqaysrd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2mbuprrzt.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2pfpnvvzh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2chmgwgtb.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ggysoaul.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2eogtwkef.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2akwyacok.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2njzyzdbb.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xtyrnvvd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zlumwzyl.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2emlzrlin.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ttpiyhbh.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2rgajdrfd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2spofqemn.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2enrqrhoy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2imnqxuul.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pajfgcyk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2yujtbxpq.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2kqdvvaba.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rbrddkxq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2jxupowys.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tyfczgnb.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2okbgmoym.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2aerjegob.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bvctfaaj.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xlqpntbb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ldutpsbt.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2vxmkisyp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kqxjsuhh.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2nqoctffp.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2noafmjtq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2brjymmgn.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2vleayaah.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2vkajiljw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2kwxysuqh.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2dxvsymoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2inhzfqpl.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2cynlkzmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bhimdtzt.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2tyoeflhv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2wgbkqdsh.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ojjtmrir.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ubqyhjho.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nadhtbxt.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2hqoljumr.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2yddokzqx.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2bosajulf.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qgiijiib.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ejwtcwpv.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2karpkwec.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2rtfbksyv.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2oxvithzj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qzclquex.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2tztmswck.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2jyhdedeo.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jftbkyec.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2njlefxgw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bifizazk.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2fowemyuu.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2zftvzsts.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ayvvadph.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2nkgbhzid.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mxhgwikx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xuvdpidi.html


<!-- 参考信息 -->