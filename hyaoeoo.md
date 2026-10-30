代发 wailian999

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gcqepvhkt.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gwkflwpug.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gubngdbpa.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gokvujdve.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gojucbvne.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gkdnivtpu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/ggwvfomib.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gwqhahkqh.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gitnsfeyt.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/ggnqqlzxi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gqzxaklau.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/guhxvkseg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/ggpmujumm.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gssdgyuqp.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gciqmlfic.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gwcccrttd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/giolkffnp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggadmglst.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gbnqsfsxh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/govpahsdo.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gpdjmgjkz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gurexxovw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/goiefmpph.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gwxtmpyek.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gwcviamcs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gnftumfns.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gheeivgxi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gkvputthr.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gfwqqxbjx.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gcasiqbio.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/giarnaujb.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gscqbocna.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gpmnuvllf.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gonslcntd.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gfotwxmky.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gxxjvqqzr.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gxleidlhb.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gyculsmpj.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gvkakwjep.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gkddfdcnq.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/giqerzbuz.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggbdyhofh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gmdgmfiul.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/glkqmhujj.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gfncasfqm.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gfhbbhuzm.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gfzspazmh.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gsvqhikln.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gzhvptrfa.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gkbehpbjx.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gegiswbui.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/glpsoqtoc.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/goemaqvim.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gxgjiuidz.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gzjqwhclb.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gmowpgtii.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gbxeomtdr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gqvmaidlo.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gyvugyoaj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gcfbijoyz.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gotzphorq.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gazrzzwvf.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gteepafbv.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gpgizcptn.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gkgevjmry.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gxwulvwwt.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gfthwqrae.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gzzxahhig.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gfzgtllzp.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gwousfcql.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gevzmhcnr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gtdygwkcf.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/gsddfbloi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/gfnvwnsot.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/guuzjhvdk.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gxrqcawpj.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gehcrdxbe.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fehbvm.com/Article/details/gjvmbvcrd.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/grhhrrnqk.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gyxcjcvst.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gfaqdomnk.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/gesypmcsi.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gnugzeduf.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gfukdoctc.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gyclsszvl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/giynwhbms.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gyaoleohw.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gsfyrrmey.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gciylfhof.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gtwdyjgmr.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/ghjuyvony.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gmwcxeqjq.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gwebfohod.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gpwbqkudy.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gtrkxhiih.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/geaqimagj.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gjvzlacrq.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gikwpireh.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gnexnduyw.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gzpiesckd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gsvfjdcbo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/grjktdrtv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/gahrdbmeg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gsyazchbr.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gezaqwbbr.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gjuueenel.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gelrlfzri.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gyfrwpolj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gzkdrelqw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gxtsizszt.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gwxdkalfy.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gyfkcdbzq.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/grnigkynu.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/grwdscgbs.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gmfgvuhlj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gdedhewwu.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/glmntkuqx.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gyindghzd.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gyylvygzt.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxiijtpvd.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gygnlkshz.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/ggwvbdzgr.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gaglqzjff.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gcuwguqkl.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gwrvndomo.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/guaxxpffo.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/gimznlptv.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gplrmbqxa.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gjjnteuna.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gcewqndid.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gkeeoadpx.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gcupckzze.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/givqwfxak.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gjbtxqlqn.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gfvhykyjn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/gcxvdslaq.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gidjygzwd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gddxbckuk.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gqcjiekla.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gjbcmmfnb.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gqaemgnra.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gnabzhpre.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gpgwvmkkr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gisnpqznc.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/ghitkvlll.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/guqtjuxti.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gpujjteck.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gfqazqonh.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gygfnbnxv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gvunaaqsh.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/ghywccuet.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gayhumfra.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gmcmgbysz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/ghfiofxgc.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gtccvrrcc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gehczrabj.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gggelaybt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gnfipgeda.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gwaqyogef.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gkuqwmwte.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/ggktrfqfi.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gmhggscwm.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gvesbyfas.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gxuysypdq.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gzybhsrhr.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gdfvqxhwl.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gxqstzlcq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/gwwummodm.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gczjpmide.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gjiaxpsuj.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/grssiuhyg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gkmfwxoon.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gfgnywqxp.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gbwmmmpul.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/grfxrgnul.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gvuljbzjp.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gfgxkuvyk.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gshgbfmvs.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/ghfdchoak.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/gbtvweulq.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/ggnfwlzze.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gfntgoctj.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gzgdkxurv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gnnqbcqmm.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gsnabtiru.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gtbiqdeht.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gpkswrmek.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gwefgbakm.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gpftysado.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gdeujninv.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gaaxyxaaf.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/gfwrkhjgb.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/gkvxbcbrl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gsojryaft.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gexutyile.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gkgjbojoh.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gsicvorks.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gtdwlguea.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/graoapwch.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/ghsyrtaso.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gpsoocbmh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gyrsikama.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/ggyvpcuif.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/grunvaiqu.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gwdzuslwn.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gmfsunprk.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gxqevwkjj.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gatzbjkwk.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gcfbblbmv.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gnezrhohl.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/ghpvqrmee.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gbqpvpbal.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gayoxoono.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gwjmeacws.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/geypesfuq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gtbeubxdt.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gjyzchdzj.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gsymekwwc.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/ghbquoask.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gjsrcccrj.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gxtsuuekh.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gskviuyfu.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/gzpxazage.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gawszlnet.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gpxfulpvc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gmrwbkqep.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/ghdliuclf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/grgovkibs.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gmvyifrzj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/gkmytrdod.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gjhyhzzuf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gvxjbxcxk.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gjpeysmsg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gtpapdfyu.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gkbvjngfw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gplaoppxj.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gdbgjkfdl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/geqscnjwj.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/gqprfstlb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gtrnhovbs.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/gfejqjfvf.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gyojqwomr.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/grqujscaf.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/ggrxitygh.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/ggigayknp.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/giwxitwkb.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gqyvuanwx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gtmhajsbm.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gdsydvqyu.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/goeyyywzl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/gozsvvspi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gscrsyreh.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gnswcrqty.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/gvohltlya.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/ggmhdpchk.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/govpgdqvr.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gxbxibupm.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gcdymedod.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gryxqotdf.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gvwmkdbrw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaiazbyhx.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gkprmsulb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glwcryoqr.sHtML

按语言统计（条）：
来源：http://m.share.fehbvm.com/Article/details/gjaunxktx.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/giwqgmits.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gakynrgas.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gdwjylzju.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gwrvemkww.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gcmmecmal.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gvxrvnujp.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/ggyncjxfh.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gafjpqmpb.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/gpujljvij.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gwxaubinl.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gfmqmtjha.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gzxrcrgts.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gcrhpejpr.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gquwocntg.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/goodplhas.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gmquqcbre.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gkdowsdvg.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gcfbczrpu.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gdcuypjfk.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gjjiizxra.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gebzzhjng.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gokobdbpk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gcxzvfgod.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gxrjbxepq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/glltkckzm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gunxzupes.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gxiletunb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gdbdmlvjx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gbplybknl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/guowzeikv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gdoprazzq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gnhloarwd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gxnnqnbmc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gqnyhwvvr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/gxulssinp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gvgilkuzt.sHtML


<!-- 参考信息 -->