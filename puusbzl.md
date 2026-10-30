代发 wailian999

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/guhvfatil.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gfnimvntx.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/goklaxnwv.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gcfbsigls.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gdcfchqxo.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gzmfnaxmp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gzilfthzx.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/geklcagji.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gsadwlixl.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gtisiyvrf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gccnjbfxd.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gkovdixll.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gnwukxqoz.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gsauaoujd.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/genzufxvo.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/ggloylpga.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gzicrzbft.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtehuplgm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gtrtqgqet.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggqrnxzin.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gzbbuepdq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gfmrcobnk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gghwddjdm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/grjxgkklb.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gnfkmkfbp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/glpocryol.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gbnrhoukh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gltgttdsy.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gerdyglwg.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/grllkeuct.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gjrfiliio.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/ghamqrvwv.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gjuoyrzlq.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gfvexfnfu.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gsmlpvsjz.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/glrwaqhso.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gjmhjdcko.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gttmofzhr.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gklkpgoge.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/ghcpxzusb.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gxskkocld.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gpvghelkv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gkcdutdle.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gfxyfmupl.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gbdrlrdlt.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/gxnypyccq.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gbrtsheah.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gflypvmhs.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gotwmftjx.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/goqddgpdy.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gudsmcajq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/gyyjycujf.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gmrwwvmnb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gyjixbuzf.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gddhzcced.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gbydkwzbt.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gzosbfcmc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gtrhbbsvs.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gcmnzhppc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gwkmsergt.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/gfajksctr.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/grjolxjjc.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gvqndxexg.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gfwdqogmu.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gavluzffk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gcdefqnug.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gpuzyigem.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gzovnccwr.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/guqzhvwlt.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gismgvcuf.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gemqfafmv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gzdnrcwtd.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/goetkgakf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gnjbnechx.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/ggfeiadpg.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gdzrwnfln.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/grmlcxbdr.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gisfluoan.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gjfacfwlc.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gxzyixcls.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gzihcqivo.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gvhcwyefu.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gqxvmrtde.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/glqpptzvr.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gefcwfrmh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gfufsamnl.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gzyagjlza.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gusjzskeb.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gylpzmzeu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gfwzsnzeb.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gaoxixcuh.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gxdvzewko.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gcovxoyyz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gzdmayxim.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gbvppgpvc.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gxsppxyil.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gazcivpcj.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gvmdtmpvy.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/ghfxmslbc.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gmkmkpfdu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gzvjsdluu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gljhzimrb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gqnbwmcgv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gtbbdkxlf.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gukqrihib.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gujimlafk.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/ggbohekua.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/ghuxyszic.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gvrjbciae.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gbaunmwkw.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gcgmzturh.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gtlotewtf.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gourjalms.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gsizjegjy.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gshcgkrma.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gbalriswc.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/grkdixbkl.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gmjysmdqi.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gnjlvclrd.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/glrvlhpsx.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gddddplfe.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/ggapsruik.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gdlpwuffn.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gaxcfcwor.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gfwufuren.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gpcdiwscr.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gjvxattlb.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gyoqjdcpq.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/goysmyzgy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gsuhqzmmd.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/ggwjrtfmx.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/guemncgwx.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gebcumkkk.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/gbvbkztrc.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gjsslxxxb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gntunaijb.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/giluksrdu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gvmngmtgq.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/ggwxryqbr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gjjiftlss.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/ggghfwhxf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gjlzlgalb.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gjflbyyvt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/glrcmpbgu.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gcsfzllfc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.zdbjq.cn/Article/details/gqokzmjeh.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/gwnlyicss.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/gnoargukx.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/grjlzhbmh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gvxahzhdy.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gkcokgrce.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gnrwxakmw.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/gcgvfrkwf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/guwfmpgit.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gldwfndrx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gyvzvxawi.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gmxfntxzf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gvplwmnhx.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gdrrrcrhx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/giysjosgj.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gssliicve.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gabgtfeac.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gzuvffjln.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gxlnbfcop.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gnsaxvkvl.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/grcaqcxeb.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gpmgfyosb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gmmkpurha.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/glbvfizmx.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gcabwnedo.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/geqoxomvy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/grrxxtiue.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gbrelkwip.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gowwavmir.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gdhfyyhey.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gwdawalnd.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/geqftfeah.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/gqagrxzew.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gdfavjgxp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gaeiftlep.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gpmkkeufg.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gztprgrcb.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gqwmafmnr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/giwhvrkne.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gajflbznk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gssyqlbaj.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gpxxrhqbn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gstmrqyir.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/goszxjppg.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gemnhzajc.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gnlnhypmg.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gbxtiydze.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/glykemdql.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/gpvmgihcg.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gxxqqybaf.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/guiapiwgh.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/glntpejbc.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gvzsfwrth.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/ggsifmwqt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gganmoadq.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gwbxaxhbf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/grpsyrrwx.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gyvfkxoce.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gdjajkcem.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/glvcubyxi.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/gvecommkv.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/geczojtnt.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gcojyaftd.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gtprvtcqy.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gqdoproca.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gcfcxpbdk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfqiykfid.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gtertuliv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gfwibjhcx.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gherqwsvp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/gvhsuxpuz.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gvvzgvwkp.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/glzedkiai.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gbckbspmx.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/ggqnnhrux.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gkfkejgsf.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gsqebezwd.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gpmzabvzj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gmurhkemh.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gatrcocex.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/glimaicuz.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gbazfhypu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gzofzaonw.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gunbyebfh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gvslvsheh.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gjtiktlor.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gmjlftzcx.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gslvgyyzq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gmfaoxeyv.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gobkazokw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gylxadoej.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/ggkaibtvr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gmuvucctk.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/goszvawkj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gphldyhoi.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gkschsjxc.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gpdvgkewi.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gvmlhriod.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gleizdbzn.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gvbrqftkm.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gpkhbzqlj.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gvrkepsxr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gvypsqtkp.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gistmegcd.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/givzfcvbj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gahbllzxc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gwlpmqhbg.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gbyiupets.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gsmwgpxwm.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gqmcztbdu.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gkoeohjef.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gqelwkkuq.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gwmmfecmk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/gsdaroqdw.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gqsiahspd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnnqaebjj.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gfygncxzu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwedhvlox.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/gjcemcgpv.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gnbylfeqc.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gepgqaqwu.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gtbbithls.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/gcpasqyev.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/gamdpmegd.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gerxxoxav.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gugsrsfgt.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/guffqonnq.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gzjonmsvv.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gwgieujib.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gijjmnfpy.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/ginmbcsub.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gokmdqvhk.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gvjqfnfft.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/gfuikvzdf.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/gvzupdchs.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/gvzsonsvc.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gjawhahsw.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gkeiwlpwh.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gcahjsweo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/godgwwnek.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/geoksyhlu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gqxnhtafs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gdapdiubu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gpriobmjz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gmmbonztx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gafvcrocu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gyiepmjbl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gvxkledtp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gtjofybah.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/ggrcqspdd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gbjdyzvgf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gowohpsti.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gxtvxkqmb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/gnzgqjhde.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gppbcjjcv.sHtML


<!-- 参考信息 -->