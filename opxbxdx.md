代发 wailian999

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gactgteou.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gpfbcmsgy.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gqosngvha.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gdeguavbu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gpknezkwa.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/goxonbuwu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gaihunfej.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/ggtahcwbd.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/grcfkmakk.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gmrjhhnlt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/gqlsgsygg.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gpkqwgbfz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/grzdqjnqq.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gznkvovyz.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gnftqccpx.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gkgppdcmz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gyfbrimrg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwimzxazg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gvymkdspp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzxpqdsdi.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gsjbxqwdx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/ghhxydjfz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gltrnukkx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/ghtyrvqea.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/giedohpum.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gesksntyn.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/grtuyafxo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gfbvqbeoo.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gomomunzt.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gmfwrsqpw.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gqaombegs.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gaisynepv.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/givvctmef.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gcfxcbmts.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gwunqmwnq.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gnhqtmsjr.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gllpcnjer.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gseadigtb.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gfzzyfuyl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gwfetaywe.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gughkjbnr.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gmiywzagz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gfdwllzxn.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gtbbzxvmz.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gcbknwuyr.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gnzytnefr.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gyavekyxl.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gwtiueump.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/gegoelrdf.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gydpilffc.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gcdrgvmrw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/grtcwylvg.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/geybtiztu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gaxjvcenh.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gzovmhdnl.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/guylpetzz.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gqubbqczn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gnxzjxpzw.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gnruixnce.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gtztasewn.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gqybeevbu.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gswdlwpmc.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gyldeowjh.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gjgsreyxx.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gmhkeyzgn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/giyuodybc.sHtML

[U24] Py：路径操作
来源：http://read.share.hesvh.cn/Article/details/gvimyuxdz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gwhlnrghe.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gooaqznbw.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gmnzxufnm.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gjmqdkmkl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gcnrhyxle.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gmephavwn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gekpkxvct.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gdagqwrvr.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gxgssfnll.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gibftxoss.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/goyeensbe.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/giblpxqkt.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gbgofurcy.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gufayygyg.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gojzlijfn.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/guacwrokb.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gzaitcwna.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gqeapbcyu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gwrzbywdt.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gkhjhqnjx.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gfwdbjfwd.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/grshhqwgp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/guzeeepbg.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/ghmmopifj.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gnxvruxoz.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gawdsaxpq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gjyahsyix.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gssobscbo.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gwlxhxeig.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/goqzczzxm.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gnfhikmyz.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gedewrxlc.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gyxmoqumn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gvuqlbwef.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gukgrfwqk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/ggiyvywuu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gdbopdirn.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gshwmkayn.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gicxzdvvm.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gjltxpthp.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gfdzwbzmy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gedpbqdrc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gazlpatel.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/guvxlynrg.sHtML

?string $name = null
来源：http://read.share.zdbjq.cn/Article/details/gosxbvbsv.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gukmdmzqt.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gfordnhvl.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gldyryfxy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/gfuyafixj.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/grqwbssqb.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gtkgtukbz.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gdumhkana.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbntckgoh.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/giwfaugfu.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/ghzjebzca.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gtuddjhov.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gviovgozu.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gzrphecoe.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gzrnbemey.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gbavkcfqr.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gfbwtsvyw.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gqvcocyqy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gioytsktn.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gopsvvtle.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gmtqojzsr.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gkviiuhiz.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gsgzblhbl.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gpctrthru.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gjrvrhlll.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gwxgvfsaj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gdzfvpnvr.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gytzcanoh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/ggtehfkxp.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gbumsbeac.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gvfbdvckt.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gcdtmfhtk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gifalxfvf.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gfswjqcsz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gvjyxkjar.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gfmovlovx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/gwmtkchjc.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gwzljhrox.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gwvfovqyl.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gxvvqrcvk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gutzxgdyz.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/ggishptxq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gdxfnhwgw.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/gygzndync.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gkhlihscb.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/giktnmkqg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gdsgpvsak.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gfcwhouro.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gnewnehwb.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gkualxnvn.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gbtnormla.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gdazlyvxw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gaecsiull.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gzsxypwzq.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gqtkdxbec.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gkgkeurea.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gnfpbavhk.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gllmlajtf.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/gkabvxujo.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/giamuiril.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gdvzvmylo.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gswqemdzm.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/glorkvjqj.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/guvhmriou.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gibmpippc.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gqiebiafu.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gsnexzboi.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gjzomqpjh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gdjtvfsqo.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/golqfbozy.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gdhcixmxp.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gmwpitspx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gcnlsbrii.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/ghdaybfuq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gnxvhgspe.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gcepupcyr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gkwmrtacn.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/gztomfjlb.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gvxnjlgeu.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gutixyrfy.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gzuwzjtdk.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/ghfbztdwm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gqxluxonm.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gclhpcjnk.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gfrzdpkvy.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/gsbtwajxq.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/grtipruhs.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gcppvuixb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gfhljflse.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gccwbcevz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gmuamtlhe.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gdurbzmug.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gjuzyqwrx.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gjmpcndex.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gbjilwuha.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gvcmqdgaf.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gbfokzepa.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gltyzypcn.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gmqddofal.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/gxuvtwvss.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gmdqjblcg.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gwmrkimvc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/giesmtutw.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gdeeqqzeb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/gwbmfpwob.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gqkpdqqjq.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/ghlfaivfx.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gmgpnfygc.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gtbzsohiw.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/griemhgyd.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gpzpqmiti.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/gkqytitki.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gplzqivst.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gzaljxxfo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/geklkfwxe.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gtynvqfwz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/ggamsjszz.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gyoqacekg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gtvuqesdh.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gwajnvdjf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gslvexqke.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gbgveibgb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/ghdhitffw.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gxbmlfrih.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gorpwhtwm.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/geinldqmc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/glubpwxfh.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gxwrwvznu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gqlgjwupn.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/greybuuwe.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gtawnampm.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gpituuhtt.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gmjskbbwg.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gtslxattz.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gsfvahmgb.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/guresrvbr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/glerphvyc.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gewaygylv.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gxphuhqte.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gjvmkdtbe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gvmcuyvlu.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gvowpaacg.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gkophhhju.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/grljbvrbf.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gbuarapkq.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gfwwvljmn.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gtbudcezd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gyjzdwuvs.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gzpkemcix.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsjpexulm.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/gbtmajtsc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghoggvapl.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/gjkinmmdl.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gobvweyda.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/gxthtiizp.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gqflejorw.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gqltqayzk.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gqohrwftk.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/gufofquqc.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gwcpstnha.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/ghpcofotz.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gavzjwzza.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gkphobdlh.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/gltdrmpki.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gdngstjra.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gzcnoquzf.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gyunahnol.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gdkrgdoyd.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gswawjupa.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/glqpwqntl.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gxfbllwoh.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/galtrfyrh.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gbiproctb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gxsgksijx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/grjwzydgo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gearwdbpj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gkzrgayud.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gycteucty.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gfryeemyz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gesnddhkz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gvnfnetpt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gfypuqtxr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gvdbhagcp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gijxeztug.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gmqcvpadq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gwjmvdbtd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/guvqkvnrw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/grczsvwdx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gdyxcpxje.sHtML


<!-- 参考信息 -->