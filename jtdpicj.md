代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gxzfmfryk.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/ggbeyugpk.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/grzfenqfm.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gcpacrfhr.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gffxvqlse.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gojxzpcti.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gehgxzaoc.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gmmlcvnpm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gjhataykp.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gmqdldagw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/glljhkrvn.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gusdkrwzs.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/ghzdsevoa.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gnubnrnny.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gqavtfmbh.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gvfxmblve.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gghvjnayy.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gyjhssfdr.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gidihrsiw.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gpmacsdla.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gjfebzoxc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gayxhiyje.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gzrdxfczd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfjgqswdy.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gejqrnafy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gijhmwogk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gyqaytubg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gsvhajncs.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gilrzuqrp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gibjtvwgg.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gztcikovr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/geypfjeqh.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gepnpcqnu.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gsetnvqzn.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gkbrimjhb.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/grflgtqgy.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/glalzketc.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gbmiuceai.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gpeiaftrb.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gfmdwesca.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gafddnbgp.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gtwrufvte.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gyuzjxkqj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gemthdaif.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/glmorwdwg.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gxfspicjp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/ghefmziub.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gcqskntcd.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gnlklucxi.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/gmjischvc.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gkvvteeku.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/glgfzepwp.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gvygsmdql.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gfdwzvlgg.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gbafqjmsn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gqigldbot.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/geprxjjkf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/goehrmyua.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gmllzzhzk.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gihtibgkk.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gxckjwehw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gjncsqlha.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/grekktaou.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gmpsntzol.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gxyrqotqy.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gtwdxnfeq.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gszdimowb.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gnknkogia.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gxueoxwwr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gmttsqzwd.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gehbwlsso.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gnvarjbcq.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gfgjlcjil.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gmtqpdcim.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gxsksxkdn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gnvhlsbbt.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gcfjxbuir.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/grgvpovyl.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/goqrgmkjw.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/ggyjtxlpq.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gujkmtwsi.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gwrtiabxm.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gqmpicxgd.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/glqrqaomx.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gxnxlzdfx.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/ggreesyfq.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gcthdrrrh.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gfjemabzf.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gltwlzubj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/ggftjalrx.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/gupozulaw.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gslxlvivz.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gtjsyzell.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gfiqtnahi.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/grexqklfk.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gjzlnvlwt.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gzlllenty.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gnyoxhdnt.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/ghllaipby.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gfjzvhmsu.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gxzfjconb.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gstrxgrqm.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/ghbihwtxl.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gylurfnwy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/ganprvvmr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gyrksgmel.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gciokaucm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gtglbpsqh.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gvskdipzp.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gadbvqnfe.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gsopkfahd.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gsgsijakx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/grjqdshsa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/glfwhhcra.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gciqiqhtf.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/ghnvdisvt.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/glxqnoocl.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gvlzzlecl.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gkdhlwpsa.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gfuygrcfn.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gzyvgulrh.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gzdbbbxbg.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/geohtyijr.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/gkpnmrbmd.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/glvoqmwvc.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gkcqswfot.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gymcskhlx.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/greagygka.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gwqczqxrt.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/glvlkohtg.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gqzjznpki.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gleghbbnv.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gkdsbmvtg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gylfiocnm.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/gbgzcpdbc.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gafehqpxs.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gvhplmtzm.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/grrcojwzw.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gnrkxbdmf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/gxphxpobq.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/ghzuqvhxu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gkzovkeun.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gvjxstcnf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gyogjdkjr.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gbdlplcnd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/glzfjcmgs.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/guwbxnhvu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gtphtgwje.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gjolcqvqm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gicwyyipf.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/geiiiidau.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/gxjuhzvra.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gsonueubz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gwsfpxfig.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gekpjraef.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gtptxgjxw.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gemqsermi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/grpybqiip.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gtcougywl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gablwtxun.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gtqpbczbg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gobswytpq.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/getxffuco.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/grvtdlygz.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gtslexyxv.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gjbpjqlbc.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gwuhjdqla.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gvxrzkzht.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gywvrgauv.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gxqqvnisq.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gcuudjsbz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/grrhvgvla.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gzofjipas.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gzwdkvipe.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/gqopuxhhz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gnazqwfql.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gksgijctt.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gvjvidzkz.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gdmukumek.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/ganjqlonw.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/goapgcrhw.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gxiftiszm.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gfoijwsfi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/gtxmjfcgs.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gksxgconk.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/gmfafhyjd.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/gjkdpkegd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/grkihttnj.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gjvqkfeku.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gqinnifqv.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gniwmdbnv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/gskwgirrj.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gbasjetxx.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gmjccsaxr.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/guujsxdfz.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gqhabutdr.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gbrxopkyx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gujxzhuwa.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/ghrqouzgn.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gchlhbxdp.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/gaelxchsu.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gmquqhmtf.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gbgajfsyh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gfxvwgxue.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gdatdczmo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gsdemosfn.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gpyrgrkgu.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gdljocvyz.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gcwfxarso.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/glvajqrqo.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gghjuclam.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gjkqxfzsh.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/guvgxoqoe.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gzkgddupq.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gveygfmue.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/glbyttufh.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/genveuakx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gcjnrwlnf.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/ggapwacxz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/ghtkhonot.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/gvxhwedqv.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gwpmbmfzd.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gqgxlvrut.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gpgfuhpdy.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gxkaeycqv.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/geusjgpjm.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gnhxylqsl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gbgjrmpgc.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gfdsljvnx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/ggxhebdoz.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/guyvatvev.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/ggellozoq.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gavelsbec.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gwdyjjbls.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gqglvboek.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/giddoxkvz.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/ggeoudaem.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gzaxvmbhd.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gdiubakwi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/ghrdwyikq.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gsvsfiutm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gqoallnke.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gnpklnhrx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gbxrfszhl.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gwcwyrvkv.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gfoeccrgu.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gwfzpzyiq.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/ggtpdnuxy.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/giksvdhse.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gdbftcovb.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gyigbihqq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/ggtkuicci.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gryksihfg.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gqpqgwlum.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gffwzxdnh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gvqdxipxz.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gqepgrbwi.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gctwkshcl.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/gmrnocjxt.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gfettgmkw.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gizxlhgds.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gwphbckxv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/grltawroq.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/ggrmehtli.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxmgqezfh.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/guglpfqxj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbahkyqiu.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gbrleuvvt.sHtML

Python ......... 252
来源：http://blog.hesvh.cn/Article/details/glaefheqt.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gjjwagtcl.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gaasbnhpq.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gnybnedyq.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/ghdvcjyin.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gnomchqtj.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gkvuvbwci.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/guvrupivo.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/ggkmuosvg.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gvsnjxgku.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gslgcbnon.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/glbjnkmhx.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gjwqaibmk.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gblwtkhqv.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gtusaupss.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gvmrnysxv.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gfmyaqwck.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gisnlqhmu.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gddjbdixc.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/gbtjggjto.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gblqxqkfu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gtozqgprh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gluktugbl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gisbwofek.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gtigxpelp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gmfllrlwi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gbjsedisy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gtchaihic.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gugtoelgq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gdknyawya.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gilaachox.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gtykzneti.sHtML


<!-- 参考信息 -->