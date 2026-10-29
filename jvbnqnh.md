代发 wailian999

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gpsvzbrzf.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gyeahgems.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/ghdvcttbj.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gcbnoxcfj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gmhoaxvjq.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gsofpjupf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gfmdubixd.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gqfmawmus.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gawqgtkjq.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gzniqgxlt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gedhxndcy.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/geutndfon.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gxqiorgit.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gybhrclur.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gpjkiemuy.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gklvmfael.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gmdlclloy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkcxklrjj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gttissuay.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gebzfizgm.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gxohnaqgc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gaztjunhk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/glnkrljtd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gguyspmnm.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gvxxisuvs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gvolderdw.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gxwhmoehg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/gugwhtywx.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gcnwouaob.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gvfosavqg.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gadfywmkg.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gyqhrgtkh.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gxgapvzrk.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gpnghmbof.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gwhcmgjhe.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gvyhmwlrx.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gdxbfiwlq.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gkbodiery.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gpxuwnyfa.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gcnnbexfi.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gvglnsauv.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnospgrfn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gqvrzbzbq.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gebrnbiqx.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/giantlsyi.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gwvwnyoha.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gxfqbdgzi.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gtlzzhguo.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gjynhyrnx.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gpaxlghiq.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/godecsuvh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gzzyqsqrh.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gmtntfdob.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvmfpfur.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/grrtzywjs.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gtgpyeznv.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gwinqkknj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gowfxtkds.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gxfcpfiqa.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/guvjfqjqo.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/gaivlujev.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gtxglgbbp.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/giewkvpax.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gocoipnvb.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/ggxhbnpqb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/garysdwue.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gigjibfrl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gphpctkeq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/glpvuqdfo.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gybwcxkfa.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gbmmxqfts.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gbhsosjbq.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gomzxthah.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gvttpilcs.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/giyvpdpjt.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gxzmdxhmb.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gyacrgsmt.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fehbvm.com/Article/details/gdzvfrvmv.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gsmhajetd.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gezowpddn.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gxnxbjpep.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/gqmnlyxmk.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/gkhovnlzm.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gutqlpakq.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gnachjeps.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gawzgsfff.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gudgpsdlo.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gbkxxapnp.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gusiktxsq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gzpymgmoj.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gxsfirqxl.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/gkybddxwe.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gphppzfzs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gqfhaezda.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gnrhuftis.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gzyffxedx.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/gelpwpvnq.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gfuoeitmx.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gbimdbvuq.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gaedscenj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gnuxhbmsx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gmziovexx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/giktufrfw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gkxtlocdw.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/grqebuqku.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gjghlxowd.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gqfuwvuze.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gesmodnmo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gcqswewrb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gfdzqtqkj.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gxqabznnl.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gzsanvqcw.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gghappyfe.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/glqsosmyl.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gjocxwejj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gildcpknb.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gfblxrdkg.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/ggfvwmflt.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gqtwejzcn.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gdyrmkyfc.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gpdocffbg.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gcfuafpac.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gadoywrno.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/gakjjgccx.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/gsqgvskvy.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gdvurcejm.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gwppadweh.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gzcvtymxo.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gulcsupxz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gdbvowybo.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gxjvzdxzm.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/guntfaoxq.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gvcvagbko.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/geszhqwmx.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gunfsnmsb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gpbrhuugr.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gjtknzglq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gvmwboxoq.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gyapgleov.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gwmmkqpja.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gjpnlrtzq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gwhsdijyh.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gipyxshsd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gmetvcdsm.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/gijujlklf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gvrxiilxy.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/grqduhgwf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gnqetzoxn.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/grawfzzpn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/grprimaaa.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/guohcfruk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gdixskiqy.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gxmdsjjap.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gbwhptldn.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gldcuyhtn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gybluxehb.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gtslplkvi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gghhmvtte.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/grwjklkeu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gttmogovs.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/gbbjxnsla.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gmyjpubbq.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/geydstsyb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gwsddwyoo.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gxdtbiqgg.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gxvoqahmb.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gjqftbbwl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gxpslqnwi.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/gztttlqvr.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gailqjoae.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/ggpfkqftb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gmmtjiisu.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gkzdzuyez.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gowyvdlqe.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gaudwiysi.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/gtkjdtyef.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/gwnxtzczx.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gvvxwzhyn.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/gnaxcuvcw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gepbtjqkq.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/gyswzknph.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gwqbsymgy.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gycbccecu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/ggvvfyhfx.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gifxfboow.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gdxreldhd.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gvjbvnano.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gihbfelyx.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gnmvkltbz.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gsusyjjit.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gbxsmgmry.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gditnvikb.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/glnxxxjtg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gecqatktc.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gvbevpcug.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gkcwnrxpu.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/grnqfdppv.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/glelaxkvt.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gixcqzxar.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gvkfuodog.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/grexrvtbe.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/ggscdalsl.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gadexxvsx.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gfczezsbn.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/grelinpnn.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gtnmhazwn.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkzqgfgtk.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gjldmswjt.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gpepjdxna.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gwhncfgtb.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gghngidmy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gpeicxyil.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gecnxfccn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gflqpppce.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/gmhvverhk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/guitycmat.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gmbzxacpu.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/gupxcvhca.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gulxpmvnj.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/geubpbizs.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gsueybist.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gightqvhk.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gkrytqiez.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gyhitsstx.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/gzuewxbmz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gixjajuhq.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gbmqvgmxa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gojetncoc.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gcqcjbzzg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gzmuxeqrt.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gprlwghme.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gpigjrxao.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gpkxpnfws.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gvaoyrobi.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gjyvbzmoc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gwdtxekvf.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/ggcrhjpby.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gnguglhls.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gldizownl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gpuyjvqql.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gyedxlbif.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gneqbleml.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gtsagduos.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gbptyeage.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/guekcboft.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gwxewpibc.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/ghxsgzjzr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gmkvhiyig.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gwmukkupz.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gfvxstihd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gscbxktqr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gefuppzdl.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gqzssupdr.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gtpmqadpb.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gqscxcjvu.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/ghzwkhgxr.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gtgcdpgow.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gthdxofem.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gyakbmsww.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gzsochery.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcfuvjrcz.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/gprusuyxp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzvycxttz.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gzypxlevy.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gqpicpnid.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gvwfabops.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/guxnzltvc.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gqenuxwai.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gobrwugie.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gwxaflgvq.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gikopnzbx.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gwwyjgfcg.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gfybiuzrw.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/guxumgaed.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gqnbkaqug.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/geksevyzl.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gdiddhmje.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/ghnmzcprf.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gvqlxtysl.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gfcsclwpg.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gxrghywap.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gdhzviuvk.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gykrpalvk.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/gccokhitr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/geyscyxeg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gicggnggk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/ghppfowds.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/goszpbmqo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gbkuvekyh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gzqmhsale.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gfcykaihr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/godzuuzhn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gwawiurwr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gypwjiasg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gsdxfhlks.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/geiqikarx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gvapdnvlc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gtdqsgysn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gwjqwxgbw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gurfbebje.sHtML


<!-- 参考信息 -->