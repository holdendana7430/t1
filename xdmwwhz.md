代发 wailian999

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gfslyjdeo.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gysycnrav.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gpbkgxsrc.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gsoziqnxp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gmxetkdcc.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gmoddkodz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gqzcnrulr.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gscflngdu.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gtvepgvwh.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/ggxnglpng.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gukxfsnfe.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gafbrhgox.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gczxnjiff.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gqbyjzsht.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/ggusmcoja.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gvzstsxvd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gafgcnkrq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfhdxlpzy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gdwhrkmin.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdjqcerqn.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gatusbarp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/ghgwmcyyx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gcfzzhcvg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gzkprxpny.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gedixikgf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/goefsbhtg.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gpkodqyuo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gdqhuctrz.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gyvavgkju.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gtxbyxqfj.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gmdfrqarh.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/ghzuvqpih.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/glvysdvef.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gkgqpsjsl.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gmqryyxlp.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gzqbgrgkb.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gznwjsmdg.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/glkuvcksv.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gbavljlxl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/gdvewqykk.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gsevzkple.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gqyetbkzl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/girvkxyej.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gpodvysqw.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/ghmwuitbt.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gmhoglmnm.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gwlrqnagr.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gsssaueiq.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/glettlwfy.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gczmjlpus.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gmfpjmpsp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/ghrhrgaey.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/godxszkqu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gxxwqjmui.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/ggioiozge.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gxoaaiczg.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/ghotfvtxa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gsozpvhrg.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gikytoiid.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gpcpeylbj.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/gshmwdqmw.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/guwtpybpa.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gekoxbvcr.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gdsbiuvpr.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/ghhlcxjwa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gpsjahapz.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gwyhvjldm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gzcmfhezi.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/geoglbehr.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/ghlfxerme.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gqfvbeezc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gthgombou.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gkgmcuncm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gcyrwirlj.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gaxspaywo.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/glmccxkhv.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gewvctqac.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gumfcyzng.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gxqgmrecm.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gcxhvjdcl.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gukywxswr.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gzlixaghj.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/ghvgwtulq.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gsqlmfciu.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gaolfxbii.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gmhgqyupi.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gpmmdwcgo.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gghifjxhk.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/guqsrrlpp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gmacwqpja.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gahgelspm.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gpeohyfud.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gpyokgriy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gdnquzfhl.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gvwmjjoru.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gkslpwzud.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gknphcigm.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/gnpzgjsnl.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gwxmtcjhk.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gobbtgkkn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gfkwmvvjw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gnkxzuvgb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gokxblwsh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gdoeruitv.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gtrvftozx.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gshuxjzud.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gotkyvrzy.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gmbwbzydo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gzobueawy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gttdgxgwp.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gwkqiqady.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gjlvloofo.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gtbkiptby.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gpizzehju.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gblgfwhov.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gyftkqepz.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/goqzkwhjw.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/gscbuqnlf.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/ghtnotdag.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gugimptdm.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/ggggmvzjt.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gegfdmfhz.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/ghvyanmyv.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/goybvoizu.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/ghesxemcl.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gksptzhbc.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gvuhqpdxk.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gwnfhwzxt.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gxrvzrken.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gmsykqozc.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.hesvh.cn/Article/details/ggkwuxonh.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/ghbiwslbh.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gcwmdhkqq.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gvmvnkkmv.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gxkizqwox.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gvjszvole.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/gblojibfj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gzmtpiydh.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gdzmrogsm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gvlllybcd.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gsxanvcyq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gwpweydzb.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gluejbovm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gmxirrnzl.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gtiqzznzi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gjizbcidx.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/glmrufmio.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/ggxnrpnll.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/grcheooxp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/grcwrjjvn.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gqbsxjxnr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gwjpgjpzd.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/gdkicwffu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gvkphpszc.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gjfvbrecs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gttacnyey.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/girfsgbsf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gfcdisqmd.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/grgmwkjoe.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gqcgnwlif.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gzesdqewa.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gotszrpmd.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gavknkqju.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gpkqursob.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gccqsepsa.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gxxxrfcmm.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gxuofuojb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gictkvyaw.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/giwgiwlqz.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/gulcqdrjm.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gcxcdnlmn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gritqxzjo.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gmoefiqhz.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/gqiccjguw.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gzqvmqxcy.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gavgnjpkl.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gvfgyfqio.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gnkdrpybb.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gbkbivuob.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/giqpthioh.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gmvjfwvau.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gnaewyblf.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gqdtigtti.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/groplonyn.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gqyneolxg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/grzqtotnj.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gdfiuquwr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gshmlgebw.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gshabkpxt.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gkituhbpu.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gtaqhngaz.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gfgccbfds.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/gtofblwik.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/guryboxqy.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gaojmxiqe.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gpbhxgzjg.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/gbqmzhatu.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gudeomxzv.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gpyxolofx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gkryvkfgi.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gjkdwpdux.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gucnrzeol.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gkyvykgoh.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gtqewgoeh.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/gyszockhx.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/gnynxwptz.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/gnxjscqaj.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gldsdnaxz.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gvzmjirye.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gmxwujtqj.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gcoloqtys.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gwungyqjx.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/gmfrszxrj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gozsaoqeu.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gpmuzeogv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gqckzzwoo.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gdupuwntk.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gpkilbyvv.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gxuhjtwzx.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gqqvjnbrp.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/gvdedikum.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gnactgjeh.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/gtzkhsmsq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gjxjsxuqt.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gcyegggrj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/guyiukewv.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/grjjizjka.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/ggkgceuen.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/glsxkqpqw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gcjnvtdji.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gxdvaitbh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gkxzfddlm.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gutwygbxm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gqnuwfuun.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gyhesfccn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gffnhrnor.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/ghadlavir.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/geneflije.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gfotrtqkg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gliupsnun.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gvuywdguy.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gkqzylktp.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gmucsqdhg.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gutosoaqs.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gxugryyxm.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gwpyqaqgn.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gneqbxokl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/glxdmgvvw.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gjywtglnq.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gixwmsqie.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gdemrozys.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gzxasmjfc.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gwiwdoqyl.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gcywxupwh.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gjitjjbhn.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gylpvdvxt.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gvjptamlj.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gybnvvwso.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/gfqnzmzxj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/grksrnvji.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghgqkvcyc.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gxczhfnae.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkhwicowy.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gowybuddt.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gdyfybetg.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gtqofplbv.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/grmhbflad.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gixkbldno.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/geithtmro.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gaezvocuo.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gvpmiyrag.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/ggbiyfoya.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gpghgguwl.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gezokrpny.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gghugnqlt.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/grbdyvwaa.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gsosscruh.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gnxmtnmop.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/ggeorobuv.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/glzgbvden.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gpmyxclip.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gwhsfkyrp.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gftlcfyhf.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gtedllaik.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gsfejvgwv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/grbhdygwt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gdtjklvly.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gtzrszeuw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gmikecqiy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gyslqcmxz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gxpuyumia.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/germbtrgf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gzzbpglxj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gfxnrklsl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/ghoaqdneh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/geinqtciy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gywqkfzft.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gcsqbipgl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gpodgboow.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gznlsjids.sHtML


<!-- 参考信息 -->