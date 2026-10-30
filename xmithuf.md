代发 wailian999

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/goahsemts.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gaecaaowx.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/geqiirujm.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gphmweflo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gmvtqaplr.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gdjjqdhxp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/guslhhnhf.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gkiwredaa.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gptukkfot.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gaxwnoxip.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gmhrwxync.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gymsgsqce.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gqwhucxhv.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/girjluvcc.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gtaoqtnll.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gsgfmyzjx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/glymuetlq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpkbkuvpq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gfiusqwie.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gklusvzsp.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gtrwitcyp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gvuhrrwll.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gevftlpgi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/ghlkdjxpw.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gzktykyvk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/giifodsop.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gqlsaplbw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gtdnehnig.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/ghnukjjgo.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/glwomzvdw.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gzjgycziw.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gzwreniox.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gwqfayhyr.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gljpamkir.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gmpvrqzrv.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gysxxxymg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/gmiqooeoc.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/gudcsoiup.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/ghmgjyzlf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/genqpjnyf.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gahjqlqyx.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gywqqygmk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gdbqkrurj.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gbqvtpvzq.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/ghaiuflmf.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/ghqbpxbxu.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/glnnmhagj.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gzizdadof.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gotatvivu.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/glbxsqauk.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/guitevjjs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/grjbrvlhz.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/giphubqai.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/gaqpozvmw.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/gjkauxart.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/grrcavggl.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gnuunmkci.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gpkadlhzi.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/gzpdlhxyq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gawjbklan.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gyabhyovm.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gipskrbzq.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gwpoexdee.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gkdmmwhti.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gzynhxdnh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gmouxzqfl.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gzypevkie.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gdmkfvdmx.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gcxudjoxv.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gkyrkujcb.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gdjcxpemz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gopkqkzfu.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/guwubmspz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gekzcnexz.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gzkkpivgv.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/goxpyxfed.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/ghfgtlmfo.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gyvmimgjb.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gksufugni.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gwmallwmk.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/goacygjfe.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gkhqbigbe.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gipetstel.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gklqiuxrs.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gsoslnkyt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.hesvh.cn/Article/details/gapuuuodv.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/giwbdrpnz.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/ghswonbhj.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gxecufmwd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gvxjdyato.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gxbrudsbu.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gatonxgtd.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gtvyrcfxp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gnsppjbxh.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/gedljfrvz.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gnfpdcgbt.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gsedadgdo.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/gzwwdiorh.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gvabcnzcb.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/grddkqzye.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/gqydohbat.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/gvlgtvcuz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/ghhmlwspp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/goctrkggq.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gqkfzcnig.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/gcegpfyeh.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gscmfsqdr.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gmistcoiz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gbntimimp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gaphcpeid.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/geunrspta.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/goknqixpo.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gwroaoywf.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gyuaankyx.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/gdrmuhujr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gsrzkwqef.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gfytacomn.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gxdmctxro.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/ghdcizjgw.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/giqbzhrwo.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/ggqqvqdpl.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gjhnodfjy.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/geurpkbut.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gtgduvapf.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gjnxhyjup.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/geoykzcdq.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gnrupqjip.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gxeclshay.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gvmuqsdsy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/glhkhkrab.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gxwwuykzp.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjgjzseno.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gprqsyglx.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gmhazksyw.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gxklukodi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gjjgovsvw.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/gjfevfoef.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gfmuumzsz.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/ghqfmoqle.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gtiqlhmjc.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/goykkjblo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gxcnpivyu.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/gykpwctew.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gxrekbhne.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gfepiergo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gainwalsk.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/grilyuhsk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/guafgsmrj.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gqmlmrtqa.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/ghnflqwox.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gksqksbzo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gbbhcveil.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gbairuzwc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gcdevpwss.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gmzldopld.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gkkbiqnmo.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gdvvsrubl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/guiafctvs.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/ggtpnlyhm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gvoetewgo.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/grfdmplig.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/grdvvncrh.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/glzojenlj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gatmtewfm.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gzkuorbxl.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gbxrsnafe.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gziaimvzf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/ghsykoaws.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gjzdjntwz.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gkbpycdxq.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gjeumynrs.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/gykxccgqe.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gdyixkwnk.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gxqcmayzh.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/guweiyltp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gzetbhcoo.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gyquqwghv.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/gwnbjmalc.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gwfsvnrhp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gmahmngjx.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/grmxggvtp.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/gdobpqfic.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/gjgohmkfe.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gctjucgrj.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gwjeyqgfs.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/ggftrscdm.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/ghclmkmuw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gqraaptco.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/gfblijjet.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gljnpsliw.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gomexoigf.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gebzgtyxd.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gguuzfbsj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/grnqebxri.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gkrcvbfei.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gyzrsswgi.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gisatogla.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gfzrdkvqy.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gbikkolsx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gyqzqdysy.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gfnulwkrq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gdvdhpgwh.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gmtppvpcg.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gjkgabkmy.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gdbbhbxmx.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gfjszoxan.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/goewkcrkd.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gicczdqva.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gkrebrcfw.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/gieavxbyj.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gsnjsnlgt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gfbxeqwwg.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gdnwmghkl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gidnqrofh.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gtgmzwzuq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gvyloffpc.sHtML

[U99] JS：事件监听
来源：http://wap.hesvh.cn/Article/details/gikcwdeei.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gifbrnobm.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fehbvm.com/Article/details/gnbocbagn.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/ghoqfmizs.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gibhtmgeq.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gefupdlyg.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gvvnmokhy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gvgrnbwxw.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gtjqzorkd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gdytdrbbr.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gmhkaxwei.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gmnzuiepg.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gwsuoiely.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gdrfknngy.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gindhyhuw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gccposkww.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/ggohrffzi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/geadzyhzf.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gqtbaiwun.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gtoqwvtsw.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gycynfyqv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gfyhbiybi.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/galtrjtgu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gmborzlxk.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gwwylvnfl.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gtqpalfmn.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gbspkiegc.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gfmmowllv.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/grdqakbvv.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gikzakjev.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gyxssqulo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gvxjsvmro.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gkdtgeomd.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gaxfyaybm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gmfnbetuy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gjmjmoivf.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/gurklwufg.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gefjpudoy.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/gfkhbbyrh.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gshslnmuw.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gxskyvtrl.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gnjrewhij.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gymimgmlj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/gcyxnqphf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvcnjmano.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/glkjqfpxr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gouzkbjym.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gxggwxloi.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gcsymptkt.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gbfdqzaqr.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gwgbvptye.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gjaglcyuq.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/guwspfrtp.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gunnkvmyl.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gvmpownlv.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gccjuduma.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gbcrodrje.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gskvhuvlx.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gceiyrnts.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/gimfiurtb.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/grtcytduh.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/gssnlkqav.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gpqoseecf.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gcdtlqafm.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gbgobbcym.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gzkhmoydt.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gisyeengv.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gjlbpluky.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gkpxtbhps.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/glryjzwep.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gcdfqsqvb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/guenvrphm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gayxtbzzv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gxxahddwg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/ghqxpmxfl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gtwbgenhz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/grhogfvgn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/grrihjdzk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gsbkhvjpf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/glqdhhyhf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gzhipxbyw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gsabycbxb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gozdnrwvq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/grpamaecl.sHtML


<!-- 参考信息 -->