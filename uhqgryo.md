代发 wailian999

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gukxuuwvd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gxblqwdfh.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gofuthnwc.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gngecpyra.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gonlvlywp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gqintnrxc.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gzusvllkg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gwmzqgvlo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/giosjktxj.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/goloytmbd.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gjojchuqa.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gtwxvtuju.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gffmlsyxd.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gllwesqdp.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gizmnglxd.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gebrpgiib.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gmazlxtdh.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gwpzllfvf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gcdbgguiu.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/geuzhtpsu.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gahnvzorx.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/guaarmail.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gesaqiwog.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gjssspwdu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/ggtrxvgwo.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/gbwhmfoit.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gvtzzwvga.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gibzmxgdr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gfyarfixh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggmzsxvgw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gltgosafm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvrvkrerw.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gsqhkiozk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gttsxhxeo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gzprenolf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gipsxmptp.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gzhlwuizg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gjffivtuc.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gslyqfywl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gooehbupq.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gincsjhxa.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gecbmkvsb.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/geemorjoy.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/glxyrsjpx.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gtmjkjsrt.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gssbnhpwp.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gwrfrhvpr.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/grbxojtyg.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gfwwzyvzb.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gdtudomhm.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/guscioomz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gjrkzmqgs.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gisqpcssv.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gbvqshane.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gloulvgls.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gxspcafyd.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/ggezjajqt.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gaplcjnvv.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gabvsczwb.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gmujxwros.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gbtetacpn.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/gwtevroga.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gwarzsgiq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gbzdfeepk.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/grckkrafm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/geligtqqu.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gboqcwcoj.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gcljsmuhg.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/ghpkfdnfk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gwbijkaht.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/grheazrii.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/ghyhfpvfc.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gllwawqca.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gasndgrdf.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gszdlxziu.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gsimslwun.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjxqeausf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gcblrkpyu.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gaknzllyp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/ghssoljjg.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gsumigffx.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gpzearpme.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gngxbedcx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gjbramxfk.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/ghrqvpbzy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gxeikhywo.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gzqmzlzid.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gdrmdpqxg.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gaxcxwpki.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/glycuydiq.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gzxbvffay.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gublphnnv.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gxeniycue.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gzzcpevua.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/glnrpzspz.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gicqxxghm.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gyjrlmmav.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gkvwglara.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gepysdkrv.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gwmvrevwy.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gjwjfbuvc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/gkxkwdtfe.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gcqybeede.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gebbjzxxs.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gxtldbxct.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gvchaakrd.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/ghikwsaqf.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/ggvotuoxs.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/gpmrsqlsm.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gswbnvvea.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gxltflekc.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxvhpnqjb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gxwgmgova.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/gopcegktv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gxlnpficj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gmeopolkf.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/ggclemfoj.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gitioydmr.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gvqucqhlm.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gfqlsovdz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gdcgkebjw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gmbibwewn.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gnvvjedga.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gsltjfdvy.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gskzgpdnh.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/gsguxlcta.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/gcodmpvzj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/glbtboiua.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gxcgdtzwu.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gzjbpegqq.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gbsvopizb.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gmgoqfcbl.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gdsyfuspj.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gyfpsgjte.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/grchlrrpo.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gckhxibcs.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gyxftpzez.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gpyvrakzn.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/glhkyaoxe.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gfycpqjuf.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gwnysmcbh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gvzghtyki.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gcrxnrush.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/glfcvngjg.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gqybjvuhl.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gbisyuctx.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/giajspzbm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gfpsuqbbu.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gevjyscnl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gqcrywioq.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/ggabdhmaq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/gjjugefzb.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gjhxiqtkh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/ganhyaobf.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/gbdxqpzkm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/gkzxsffmw.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gejvldtbz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/grypvgqqa.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/ghhptjetb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/goaynfsay.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gawbemplt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gndhekfyb.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gnpkjqoqe.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/ggqlvzngd.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/ggqsnzwym.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gqymjjpop.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gsbwcmrqg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gdgsedrxj.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gnkbqqpao.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gsbmmiehd.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gddyssmhb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gaoxrrjqv.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gluhrbsbc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gwichxscx.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gmaolplzm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gvthnxwyc.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/grpjjhmzc.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gelolelcb.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gfcqfxmce.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gknqzqbax.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gxgalsmqk.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/gybofwhvu.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gyygvpwxm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gllajkjyo.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/ggilldzxt.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gupioabow.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gaxjlufep.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gfwrgnfib.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gmarmfuku.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/ghlhndbca.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gmtmefiub.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gvbwzljrv.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/gvxamjkti.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gwaeybjgd.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gcdptvjnm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gjtzjcfaj.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gkkelobgr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gvowyfhji.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gpqksmiwh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gubozxhjs.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gycxwlhbg.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/gjgehuvan.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gzqcpfkpe.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gxftaefhr.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/glrknpykc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/geqryrnzv.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gtojslwlp.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/guzfrwmsr.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gbanhcuqc.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gdhjfhmdv.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gpaaswnqu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gurzkbjqu.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/gdebjqmrs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gsnvhmwvq.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/gbkeosdlb.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gqmjewcgx.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/ghvxegatu.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gpcjitnqd.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gqhuzrlcj.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gnpwnkxxw.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gfpkccxfa.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gdwehopgm.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/garrvqzaa.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gonbjxxit.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/gjyhqpnlq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gxwiqgxpq.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gxalbudvw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.hesvh.cn/Article/details/gttxehiiu.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gmpajipai.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gmdvheswf.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gdgukbrzi.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gruftfeax.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/gprfaazdr.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/glsfqxkdo.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gpglxbnyr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gemlkzgxx.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gkofkycvt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gdvnfhnof.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gtpwmotok.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/geijpoack.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gojhmwzmj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gjjqkaxtl.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gmmwckobu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gfwxyoqil.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gwrtdfnfa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gjaxrpddl.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gulfpkdrl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/grjlwdiau.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gyfxkliae.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gbwibwfqy.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gmgjvkhdi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gbbwmiroq.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gusfdawev.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gjyerfnis.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gyopatrqa.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gugxalwby.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gzagagtyw.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gnbvfwgkj.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gxwageleu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/givlyykgg.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gesmjtouj.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gjfxaujjr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gwrevvayo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gqonmilcc.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gpeajmtkd.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gpwruxegv.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/gmaqdwefg.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gbbrxmdug.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gnduigdae.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/gsntbjvna.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gfjiaeood.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/gmliwelra.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmwtbnnrd.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gqthuheky.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcjkgxqxe.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gnrxftdyj.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gqxpuhkni.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gbananone.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gtjroqjzx.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gkauyeppp.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gfzpqufob.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/giumxzire.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gxbiabiyz.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gwhavzfuw.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/gdcwogcdr.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gvtpqdmsy.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/gqedmqvxm.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/geqaitwbr.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gaegnilsw.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/grfzjzpcq.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gzxeqmuly.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/grnrhoras.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gsyzqbkhh.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gsqxeilcw.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/gyciynnfr.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gamzzakzn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gaprtdwvi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gnsiumbzd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gyvkeqsew.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gjoudlxyo.sHtML


<!-- 参考信息 -->