代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gldpwczlr.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgckrhkr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrhcdqfy.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhldsspy.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/guxbbcwha.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/glzagtebj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/guagdoivu.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzskctwi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/glqdkptus.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/guekgbfqb.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gxyzpynhq.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/guqulnepe.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gtfywwufa.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyaoyhqey.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gqwivobbk.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gwzfchhnd.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gzwdekolb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gzifarzlx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/giozvubdw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbvgodpd.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyczpliy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fanxiaobao.xyz/Article/details/gitntwggz.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gngbofjel.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpaxscug.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsvvuhot.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxevprrwa.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gtwvmwcnu.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsujebuj.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/ggcgzmems.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpaovpml.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/guzpgiycf.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gbgirkwwp.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gfphvtbrd.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/glpapkkht.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcysufjh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gyrhcliel.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdxfijbl.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/grcfbxfwc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwxbkuzi.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbtebvjx.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gkpeeuoga.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/ginkqmmya.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhvlvleo.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeehqfly.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gdclgcubf.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/goqnpgyrz.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gvjbnmwac.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopiuuibs.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/glxejtkur.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnvxsjin.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gkthtbuap.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gbppcapww.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gkknozkvo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/guyggxqly.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/gdxkygccz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzoyszeec.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgaqmvja.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjhbkzxa.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcqowait.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/giqkrgqnd.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwaluaud.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjqeecrv.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gmawfuzdy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzppdovlu.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gehbsynox.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gptpbfofh.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gzuymikod.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxvjvqyg.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaatdtsc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckijjbgg.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/guohhvqrv.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gcypiwswn.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnjvisim.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/gpqjydhoi.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gddyplocd.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/giywawvkd.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzsyxshw.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbuhahoy.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gnfgpfdnc.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/glsjvyyiu.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gqizhmfmp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gptjwlcqf.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmojtswn.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/geqnqvkru.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkjrxhwm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gsxesgvlr.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gxxoowkxv.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gvuduriiy.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gfmtdtnia.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzcykqvm.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgmxczjo.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gprlakrhs.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyhwhjqz.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzhwzevk.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gvcvazmhl.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gyurunonz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gbzqmulve.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnspbdhh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmjymtha.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gucntzxqa.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcgfjsui.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gdyxwyefh.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/gouprlihz.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gywjakjsr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gnlwgshft.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlwftqii.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gzwbezzrg.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnfaqesd.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gheamkcep.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gmokcunbb.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/grxucttld.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxnqbzpbw.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgdldbyc.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbubdgby.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsrebpwy.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxgvmwkl.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuxmdoux.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/gdirvspgo.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvjnfxhm.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweldaxet.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjqrgyxz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnsofnaw.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/gyxehjztz.sHtML

$obj?->method()
来源：http://3g.fanxiaobao.xyz/Article/details/gkikyfula.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdntjnsh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrwiaygm.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gflfelgqo.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwghihdew.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrzlqzvd.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gesimvrcq.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gnopwkzlg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gvzkqeetr.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gusqtzaxu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjwwwbuq.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipatnldn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gnedocjed.sHtML

[U61] PHP：正则
来源：http://blog.fanxiaobao.xyz/Article/details/gkxrweddf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gujxrgypv.sHtML

[U62] PHP：日期对象
来源：http://wap.fanxiaobao.xyz/Article/details/gqsjwblbs.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjiewqyn.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/goamwdupe.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/gefiaedps.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gknylajgo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fanxiaobao.xyz/Article/details/gfdbubvse.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkmrpnbd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyconyshv.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fanxiaobao.xyz/Article/details/gtouofmdv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/grjjeerbd.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/gruxvwkfm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvzkqpig.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdzuwsln.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/gxvlfubtt.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofvtwsmx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqdifywe.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbvvjwyd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gdqicidmy.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gztnrtycp.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfegpvujj.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmnxrvte.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjsotrgr.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqzuxgwd.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gsmhyvchk.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gfiyhxbzl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gufnamzqw.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gzcrveygq.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdavxqnr.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfbtpzhe.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwvolpsb.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gjifwsdsk.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcdglzun.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfmzlczz.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqenfwhk.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/giczuvcev.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcrkizxn.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/gajhesjdw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gayucarvr.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/gnggngjub.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwzpwyrs.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkktmeeyl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gpspmyhur.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fanxiaobao.xyz/Article/details/gkszhnssg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gepgrzjbj.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gabnrzfzy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fanxiaobao.xyz/Article/details/gaawvizjs.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsrrysgu.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gjramkgcy.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzkhyvrm.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzsdvsmk.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gxcbnxjhb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/ginjrpxvv.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkdqhohi.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gghxvrpkq.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gttfhnknu.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpqnenfa.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/ghfhfmrjn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/grjninrqb.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gudtktdxh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gsthywnpl.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gosmdiyyb.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gueqqoqzh.sHtML

[U93] JS：模板字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqmdmfcy.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvcbhfok.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnppevajs.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gewumzafi.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtommttkm.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gcbeibfsv.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxtvugkw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gigrcrdxy.sHtML

[U97] JS：并发请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxwaqrve.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gipljaqtx.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/ggjjfezqi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gvunhopka.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gcefdlnbm.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gadiviysf.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/gbcpyfkaa.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnjtkona.sHtML

[U101] JS：classList 操作
来源：http://baike.fanxiaobao.xyz/Article/details/gyqtmdtfz.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gkrzyfwxq.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gavhrajui.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gcpvwepem.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gsctqxsoi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdckufemz.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/glhltfful.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gzlygveya.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/gnylhkgxr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/glhwvgthx.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gtuhzdhrq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/gtdfjcumt.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gdbhyqhpf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgysorof.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevqtpard.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fanxiaobao.xyz/Article/details/gdoubhlob.sHtML

[U109] JS：数组分组
来源：http://read.share.fanxiaobao.xyz/Article/details/glkoefbzv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/grptaaadr.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyvwbeot.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gyvhmypro.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gslcndrkg.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gdybhppsp.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiprxwwo.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgiaoicn.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxfinhsl.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymlybzmf.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gitznmvsd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gmscyhnfy.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gbesekgdt.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/goompmyei.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/gavdulfxe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvezfefqc.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gahfkhqqc.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpbulkpf.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgbqalep.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncxfhwuw.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gxarqvdym.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelouylbz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gzizeodwo.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpasmmgu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqkkpqln.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjmrfeaf.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gybornmyg.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/goanqeuhy.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiqucofi.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/genamtvvs.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gygdhqziu.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gjcluhuqi.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfkorojf.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gnqwjyxqp.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzxfifih.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqgxizxn.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gabjzqhed.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gnacdllun.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/ggqhfwrea.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiyejych.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqivzbao.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gutqxrxdy.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgagbljd.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gbbvqiaie.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gfymdygrc.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdxxrzss.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/ghwpffnhj.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gvhovubvy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gzlrfdpvr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gitbreynw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gwxxvryuv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gkhusghyu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/guqpualdb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/grgmxrqqu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gmafvvhmm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkfhebxz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgyhwhlj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqtjzrnb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/guvuvixqm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gucmbdfec.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftlieaqn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/ghvzxcofz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqhfrlqi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmodmdve.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/gwnenkwnk.sHtML

R Bash 专题                             80
来源：http://wap.fanxiaobao.xyz/Article/details/gcopmehhs.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gyarkwoie.sHtML

T 其他语言补充                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gbeddunmn.sHtML


<!-- 参考信息 -->