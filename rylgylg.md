代发 wailian999

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnyfisio.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/goqykolhm.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpihdson.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/grcqhahya.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlrtgzep.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/grptkzepr.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkukvepv.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfufmmusg.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gjorvbyjy.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhzlhiax.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gsetpekis.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gsfiekpdh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gflyfmlcp.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gvjzypjrx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/glsotejxc.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseusuqzv.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeexfqxw.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/glhtrphet.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gorozzdbx.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gggwcafcu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsahpyfh.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/ghjdzxclx.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gehimmini.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfyuyfyn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrspmfja.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugurlxdo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gvjbjdygi.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyzrinbk.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogzcojrx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gvqnbuaib.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwlgpnaj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizfzivfe.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gtlpabkow.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gddbhqsnu.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gvctobdyd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gjlgqpdhr.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzvlywke.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gjxxhsbtg.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeyoqgwi.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasmykktt.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gnksztvjc.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gvzaivrop.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/goezmpvao.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppcgwewx.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gdympojsp.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gqhbiiefr.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gcugogjze.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gazmkkrbp.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gznpewgcs.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvctwikh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/guuyohacy.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gmjzzkjai.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphpoaant.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gjpakytov.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gttbrykki.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gsxyzqjfi.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/glmgaohmu.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gtdaktohf.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxcmvtzz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwkracgp.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gfumfrnyj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gvhfxohwl.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/glukhlaqp.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpswehph.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/gfkdonism.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqmvoiwg.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gesyqwzfr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/geyvrmtir.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtczdqwd.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkeylcen.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmtqfglv.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzeksqbc.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgzqndcy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxhfmkhp.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/grtyfrfbk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gknvfukus.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gyzstzkmb.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gigcbycta.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/glbwvdlvp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdoljlyw.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyxampsi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gvqljuwya.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaxtddub.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnesmbvp.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/ghbzydofj.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbsitvif.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtreopcj.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupchjbfa.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxyuaujb.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gatziwbrt.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlqtikxh.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbpbkvrw.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/glydexabk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzejpwgb.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaysyzkp.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/grreisvpb.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/grkywjvvy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxuhnvet.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjzsdlbi.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/gfxyiiebf.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwyliekq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpncgygn.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnuxvmiw.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyylokdw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfcfywvf.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuanckcu.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/gbwqbisbt.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gfpnoatzl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyzfrfiz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gdgbnvcjg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhshrpdr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gzikrekqt.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmybmykv.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgiciqpz.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gtliyhnsd.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/govfbujdf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/glmkhkqyr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcovhyajf.sHtML

[U46] PHP：可空类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmwjgnmk.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/gcrxudtqg.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/gwsramhie.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvqfqtak.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkfqhadh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmzhmjszu.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/gerkghabt.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnrvknfi.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmczgwmy.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxhymzow.sHtML

[U51] PHP：数组解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnjbipgm.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/goymtpghc.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/giwjjydxj.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpisxsju.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/glvydmvvg.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkxcjrbs.sHtML

[U54] PHP：空安全调用
来源：http://blog.fanxiaobao.xyz/Article/details/geltehqku.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnftkiyr.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gzievabor.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/ggemseugr.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnikjxyx.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbowemrqt.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gqhxzoias.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gelogsvia.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqxsixat.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/goeauomfx.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gipdsepsd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gecgeehlq.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwtztasc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/glnyqoxbw.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqteoucs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gojzetytx.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzvljbux.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/gnnfrleuq.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/gzwrhgdkg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhfehgrm.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/guqlslcug.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/gyadtuebo.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnqbpjmb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gptqivivj.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzyfnhvi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwyrbgyz.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gqrxirgug.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/geqwvtimd.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/glgesxmpu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgvcqppo.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fanxiaobao.xyz/Article/details/gxpixsnhf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnanrife.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gfhfchnqd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/gjnmywlyi.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gzziydhmo.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkyyozcj.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnefclsy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmbjyfyf.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gwwvzergr.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gfpuobjha.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/giwgtbhsr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fanxiaobao.xyz/Article/details/grudkremw.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgtckiuk.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/genarqzie.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/gtcmbgltx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggohcfmcp.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjueosjzi.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/ghrijdeuk.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/guhcyydax.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/geeafxkan.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gthmlfvcn.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/ghriggaym.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gcxdndjng.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvgmergy.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gqabtlrkd.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/gjqwvkmlo.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/grtmbzrfw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoipeujm.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmhhnnrt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/grbfgdjxl.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzryekwuo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpmnjkjz.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzdcnpqp.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gdegqddah.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabksaolz.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/gzffcpmts.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gethiqfko.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcyaftuq.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzuxlcwz.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gabycxwmi.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndahginu.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefkrtcpk.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihzpgxju.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gosfkkapq.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gpayjysus.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gobrczxes.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurlmsyso.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gcwgqmywn.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gkgodtfgc.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiwgzbgz.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/geavfnrng.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gksuknmxd.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/gyypyqcvh.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlipktpm.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqrelagl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/glgxhbtcp.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/ghekmykdw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxxzqhct.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuqcjusz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geajtbrvm.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqmfthtr.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/grxapamzs.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gnbpujllc.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gusidbszv.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxhjnmow.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpmrwlxf.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/graytndzl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/ghrdbdcxb.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gsllyyskz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkuzdjpa.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnnhuqem.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gotfauyol.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gzdfksoky.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzdxpmbb.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gsagthaqh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzlnuvmh.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkvgrjbd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gurgyyxbo.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gqztgggxa.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/gguoyxwbu.sHtML

[U109] JS：数组分组
来源：http://m.share.fanxiaobao.xyz/Article/details/grrbgmwch.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gacpesokz.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/geuzpgnpy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gvodzrnlf.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gdkjnswvx.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gbbjcfwix.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjarbnze.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftwprmny.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfltkptj.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjdvvzfy.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gyrrkdwdm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gngjelwds.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gloxrvhnm.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gfqakhyfq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdqroenp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gbswnawsq.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghurwefap.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvebptrq.sHtML

[U118] JS：开发服务器
来源：http://3g.fanxiaobao.xyz/Article/details/glsyymfsh.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gslioiuqe.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gawwqhaws.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzbklbsl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtbnmufw.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/grvyrljhj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdgyxskxe.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpznavsh.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnmkafyry.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmwjyqqh.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gijbqacfv.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbildhpw.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdacrikm.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerurqjef.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gasmrsrmn.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gbadgjqey.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gmzabwxgf.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdguurna.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/giwmsnwkn.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gvxkrzrcw.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gbtwdhkuc.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gurfrhrso.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gljrillgg.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gxthzgtmw.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/goozjnnkr.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gmnfmfbvf.sHtML

Scala .......... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gprixhwkj.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gfwmlodte.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gpmezhgoo.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gjetnpvxl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/guicuneib.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/glnrhtdzi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gkskxomik.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gammmgogm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gospqxivc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgecdrab.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/ggpjdrybp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnpjzvjx.sHtML


<!-- 参考信息 -->