代发 wailian999

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3nnqvljhw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3snocljrz.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3sdvspebv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3hgeqbiuz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cvmducgm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gntnykke.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jckkowcb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3mjvhcjpm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3oqqphokg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xjyqciaf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fkfdgvua.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3sxaqtezi.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nmiasqwq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jgnrfbgw.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vbqjoykc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wdapbtxe.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3exaoqftn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3iixscuyy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqqbjsxw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3bchrhshl.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3uxwzaghn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3swzdlzfa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vqfvnnhc.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3pnppgemn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qygmaepw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3zrnpadec.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ddmqqtfc.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3sjaqteoq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3nuyptlxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ifldjrai.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3qbgvscdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bdhxrwww.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ferdmxpc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3hohotycb.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3dpxyrixh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3nwceztam.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3sevwqutu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3vzfpgknh.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3truqbipd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3vemymzbd.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3phxofcqi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xzkunici.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3kfeeqypx.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3qplmfbiv.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3yvakurlc.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ctcvkakm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3msdtlwdz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3qzfdzmof.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3pxxrrvch.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xuidsely.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3dbbuedte.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3nkttwaql.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3glqsbhbf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nfyprimc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3gbdatelf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jqlqysfu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3lchxmnil.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3btoemdfp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3revajlqg.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3hmpbpcvd.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3obtfscnp.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3csecnovh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3crwhioqm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3chuatlxr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3kqmwqano.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3uvisjcsh.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3wjuuyspt.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mmjxnder.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3mgppbbhi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3kfettjbk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3rwngwvbz.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3vosqblvj.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3obynpayy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3sxrcvxrs.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ijrdlxbh.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3aitlrwmq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3nyybzjui.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3bmwjiqpr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3olwmnerw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kvvgkqhq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3einzpnxd.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3gaarefzz.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3fvfozlas.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3xvnrgrjf.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3fpbmbpzo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3nyvuvaxa.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3vmutmrnc.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3mtphtuov.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3aydxfzyz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3uwakmmue.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hxdppbnx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mvlydvug.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3hncycdnm.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3iqfppqkb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rxiytjwj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3tppkjddk.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3jtucymgo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3kwpigdud.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3bhxtyrqa.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3fmqdnaau.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3mqztfpwp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3byjchucm.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fxljdgou.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3eraurigo.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3qztmigez.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3glubrdyu.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3osjnjoym.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ububyvtc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3bscebjqy.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ensbmvyh.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ooksljhd.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3pchyzgzu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3iphyfgnu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ymfhpiex.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3itrkzpnf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3vdaambor.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3mrzezzpd.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3gnzxrywp.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3lxufrmbn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3jxcmipoy.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3rfttrazi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xslhlbct.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3nzhjzhcs.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3brdxhdkt.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3djmwfszg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3rxsdwijk.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3vkkjstuv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lziqeats.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3tinwymkz.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3eswxvopd.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3xlzabglv.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3dczyxswh.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3puquyadc.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3pxheubcy.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3cypmhtwz.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jbsaotwx.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3glpnjdfm.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3grjjbter.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3exjziymc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3qkqvgsds.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3azyxqxnq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3sczrlezz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3fvehrhzk.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3eyrafoft.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ipsmtbcj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3iqmpxaxg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3jknktddd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3bifrizog.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3klvzgkbx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3thfvexcl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3mgknxeqv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3mtjlkrsp.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3jbbnaphn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ovpmpkyr.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ycqotbfo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3kfhmhidt.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3iejwnnyv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3pcvrqego.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3voaapycs.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3viqdtvsj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3fwmksthf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3seochooi.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3zdayyysg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3utvjhqkl.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3jbsrokgc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3uzpxgsap.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3uxtyimut.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3sbqedszy.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3pjepuqxq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3treprpaw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3xdwgrktu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3sirvsege.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ryymmatg.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ajxuwzke.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3xlgsqsbv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3coxejwol.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ghmenvac.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3zjmoslzf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3binurkwp.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3azuckhsj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3lhzzzbcr.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3nnomjbnn.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3vowdkwsa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3tacbgyxu.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3meodrrpy.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3pxfmnjay.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ovvnhgby.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3sqhvmrzz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3hjzjlcfv.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3qrxqjurd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3nkewhyhw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3secfhaab.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3tlziaehc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3rnxxxxuz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3rkzkxbvg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3msdyugvi.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3dpyzknms.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3dpmiujxy.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3nrhwmtka.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3szuzdpia.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3auzdtubq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3scugezsm.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ppzwknkb.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3qttfvwjo.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3pdorsvdm.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3rlikazpc.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3nzjkoavp.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3wtexmvac.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3azffnlvj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gxkyexrl.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3uvwsckzf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bkbodghs.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kllmcgoc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3frcmucry.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3qnbttwvm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dqemnxew.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3mnpmnlyq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3jsruzhau.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3zzzbwwiq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3nnrjgohv.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3lvixfhfu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ohijdyjm.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3czudokso.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbiqphrn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3imxmzywe.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3krghaxct.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3jlkqmbxl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3znoevxxn.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3klzoiboo.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3yhbitukt.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3cvnuecnu.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3axtrjssf.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ehpawlxg.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ucuipzoh.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3jzmhjgjd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3wucpvzzl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3sfveivpr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3zojjrtte.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3cwbtldud.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3snbykakb.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3hfbkshpr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mrwvaelq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3elwlbwip.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3eljjafxu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3stoxfjju.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3zfiyssls.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3nmjdkvhs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3imtvrnrp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3nkrbrcxs.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tszqkbct.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3idnijlct.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3xizfvipa.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3wvzgdons.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3xmpbfgeg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ecpspuqv.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pcflyvkr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3wjknewmo.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hplvyxvr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3lcocjfpi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3cinohjoe.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wfmbsmkn.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3iwtwyvdv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3mctrqwvl.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3urhdfzzo.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3azaqqozw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3jctscsev.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3emjesmpq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3tsgourey.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3qnuqxxet.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3raypdyzp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3phfhvemp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3npgmuray.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oblegrhv.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3umfygbsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3athmnkqz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3yhtmwmai.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3iokcijwu.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3tdpuplkr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3iqwompbm.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3tawuakkc.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jjudkmdd.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3qjbbgwel.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3aakxnrql.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3jcgygnho.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3aewvltvz.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3hwftbndu.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3zayqsydy.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ndgdwuhb.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3emaljkhf.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3wictjtgk.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ibokucsv.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3nqmazmuv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3owpfbixj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tnnsyrpz.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3cylnprzw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3qgwiogos.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3jkzjmovz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ggzxayjh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3uqjnxnjh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3rdwcsboe.html


<!-- 参考信息 -->