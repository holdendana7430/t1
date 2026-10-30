代发 wailian999

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/glmsjozrx.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/ghqgfrdct.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gucesyeiu.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gylkbpryd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyuevmkh.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gnjtiqbzk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsolwuwm.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gbwfzneqo.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjckveitk.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlxmsjxf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxytdxjc.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/githhxfqt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gesszsvqz.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gxlvsnhyd.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gawxaprkn.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gjxhvecmf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnylrgwx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxkmdzxcx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gvaeisliu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghupirkvj.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/ginyhvbjb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gzkjypouc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/gfddidxdg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gztseiter.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkajzhsm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gksmvelgt.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/ggxbthqye.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlkhzcop.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/guhlcadza.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gqbzfrwam.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/garqkzygt.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyijntsg.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gpykneojj.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gazpgupxz.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkemomxxw.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrjrkxxi.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdrizgzi.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/grrswzobm.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeyoyiak.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwhjruyp.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gzhmipcei.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqnjoyin.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gvtfhkovv.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/geqdhuodf.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleymqrle.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfjmjhla.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzpdaerr.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggznaxgrd.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdtzwtpg.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gjincnyoe.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/glhxuaopd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/grudybdhz.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqwrytft.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/gzmdawdxe.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdkwkoei.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gjaujmrwz.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gvljaajzn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsozyyfjd.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gifflmuax.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrepccau.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpnnrgpa.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaiofczi.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwqoyhfl.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/grajaggrd.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gndphrjer.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gdmsfrwfc.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gjefhjeku.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gotkpohta.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvhjrrsl.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgjkdvrk.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcgpiobg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmlgeais.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsnseyku.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gklbjkxvp.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsycslnte.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxxjicxp.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gdaklfwbz.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzkvhwen.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gaebscfqq.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gelwfnxso.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/goygvqhsx.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gyctvbzbq.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gkhnpybhm.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gymitjjmd.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gdajrjzwh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gjbbodocx.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gopyjzkmx.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gpfqvaifu.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgbqfqjo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksolgmku.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/ghhyzbtre.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvzskseq.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdvwaqad.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/ghimzzwcm.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/grldbxfxb.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gubjeitry.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gqncdzhim.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwbxoher.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcfgmdqr.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gazjnmqon.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgjnhnov.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/gejijulnx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/geoxxmmhw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwqdffto.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsoakuyi.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gghgdgwem.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gncaomkrl.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gukuerfvt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjnkntwu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsqnmelr.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gesujwvtb.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/geardgzri.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gaotknsmk.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaqushdb.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkjeorby.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giinrsitz.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzhyhmvh.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gyknczfyj.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwaaysgqe.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gxphlofdq.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlxidmtn.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/gynckfgzj.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gklajjaok.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gqwdgzvlw.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/gophkooeq.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gandvswye.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwvaxgkt.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcxztqdx.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/glfkerlfg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gsjsywjxn.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/ggsfazapf.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gkwktypln.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbdglygu.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzbnkzbq.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gmakwgvoc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/ghjuwcfbs.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxicgfyvf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gibjrphyf.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsagjctn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gwwhdkkna.sHtML

[U61] PHP：正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxfkpdyf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gttylrmip.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadjfyswz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaapvkht.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gynvbhzqk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfmmowhw.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlhwjrok.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbhhloaf.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfgwitbf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gylvqqeqz.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/gflbinusz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnqoagwn.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/gsjdonxcn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrnwessw.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gzoyywxvz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/goxnemykg.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gzlnzclxg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/gfydvxsmf.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/ghltklofr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/groozcjxp.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/gidrguokd.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmqqhejg.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gichzieue.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnznrpxa.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgdfatnw.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitqkvqvk.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/ganvisaut.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgddvxxp.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/gktuoxllm.sHtML

composer require psr/container
来源：http://wap.fanxiaobao.xyz/Article/details/gajrnldxz.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gaejbhgxn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/gywwegsig.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/glgyukscs.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/glletbouq.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnioqdue.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoqpewvj.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmscrvye.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/gcacnmsmf.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/geprnpslx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gjhyuobmt.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gvaygpkod.sHtML

npm init -y;  npm i express
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxvvofhz.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/giqvtnmnt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gzukjujtn.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gtycrzqch.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gmfxtwrmv.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gluwquhgz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasdhfmhi.sHtML

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/gwkfsmckw.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhrjolpt.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/gipawpphj.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemiblltg.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbpmxzid.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fanxiaobao.xyz/Article/details/ghxcagbft.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gevexufhl.sHtML

{ ...a, ...b }
来源：http://baike.fanxiaobao.xyz/Article/details/gpfyjjpos.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/giujsjxyn.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gzzitrrtz.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gfekrshig.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guttwnztz.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxhdtqan.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdurkhmgy.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gsqhpuult.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitstmmdk.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitxjibfv.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gikjytdqz.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkstcwidw.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/ghvjookap.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gkcjwsvlm.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmlnwhnz.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gfufnmxue.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzcinmqo.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gkruckukz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnpyhhus.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gvsogxttz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnmouign.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvimhrrtw.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahtadaqq.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gyrsozbcx.sHtML

document.querySelector(".item")
来源：http://wap.fanxiaobao.xyz/Article/details/gafaetpaf.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/gvibjhjvj.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/gbbnqtjmr.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/gbvjsmhtz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/glraorqnu.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwcwqaoy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygsbylyq.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrsozvec.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gsqgcohnm.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/gqqnxgcym.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyksdwmy.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqacwssb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gdafvnqzd.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfkjfdpx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdirfnek.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/grjgzugtr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gscwzghys.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gxltmvzje.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/godqlrhqx.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkragzjvz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gelwunyvd.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gipwwvixp.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gzrhylacx.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/gczopqudq.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhhbajuv.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipzheldg.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkowelouo.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgbwfsww.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gmdlrowra.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/guesudbla.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gyoqdvytu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggctrblsj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/guguhytuj.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltvniltk.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fanxiaobao.xyz/Article/details/gncmlepcv.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsgmxgqg.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gppjqwpdj.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqlsgqla.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geayidjik.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/guxzcnwyk.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmvjdtfo.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/glwwaccdk.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuovfosc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdstajuew.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gbcmipupi.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmategah.sHtML

PHP ............ 252
来源：http://baike.fanxiaobao.xyz/Article/details/gvwshyinb.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gofzqsume.sHtML

TypeScript ..... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gitljcmwn.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuxydauq.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwtcixur.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gunjbunyd.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxtbhqtx.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzadxarx.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gegmxzkgd.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gbqsmbksi.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaybgjle.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gyitutlch.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwpxcdic.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/gjbdebxvr.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvbveyhp.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gwcnhyaya.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gictokvgm.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gucsqwobk.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gslumopnh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjeqhmqmf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxsdidly.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnjioxgx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gfddjrgwv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gunuzilgs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/ggldfilsc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gnozqsclz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsychudwz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/glnqnrjhc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/glydzoezt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gkflbhzgl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbczhkaw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/girbrdjfe.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gfonluuss.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwseevqw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvysbmot.sHtML


<!-- 参考信息 -->