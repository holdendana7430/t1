代发 wailian999

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gholptxhs.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gyknmxnkw.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gcgmbmutr.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gjoizmwnt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gtiirhpey.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gylqjnmlu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/grbijmvuj.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gvsolzlow.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/ghcbdgcpw.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gsvfijtoz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gvmjfwuga.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gpjqiztyi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gvscgwbhb.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/ggqqgpbyg.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gkkpkdhwc.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/ggzzpcetq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwyyshog.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdvyjizmh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gycikoywk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gigfilzuq.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gegcbldnx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gestnkglw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gdbpdnhfp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gdkytswvl.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gohwuuvpl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gmkatttan.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gvvsoxyfb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/garymzzbn.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/guydoyfpb.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gvfxwvcfy.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gprvidqnk.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gkuxowpct.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gvgjipfem.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/grcwxzods.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gekobnbck.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gersamrqg.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gaaofyamr.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gwlclxnqu.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gnixwwjjj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/ginoujndm.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gniqepjrd.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gfjkmoxdi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/geoetotrn.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gzfkrtudi.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gerwmxgst.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gvfxeggju.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gsrjtdmbe.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gboipeqbu.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gctonjwlg.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gzuquawmb.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gpbvvbvyz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gwsmfxvqc.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gmtrcuqgz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gganjfemx.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gyjiamubj.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gkhhahwjm.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/grfoljamt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/gtuqqkhlt.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/ggzitmibe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gujdilhlc.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/gzkqqsrfp.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gddswvlvo.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gjxhzzhvg.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gmdzwptyg.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gjljfzesx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gkxfxuouw.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gdcixoacb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/giutolsfz.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gwdvuxczi.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gtcfsxhrj.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gmyuulbpd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/glivxjqgk.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gzwfpomhm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gkjyzwrip.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gmbanpvxj.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/grirsnsnq.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gzecdwbkt.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gxtydafdl.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gnbsurujm.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/grmwklrqb.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/giekkawdr.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gdqaefoiy.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gvazejdwm.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gurdnxqay.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/glfuznmqx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/ginrbpheg.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gzegrtblx.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gfbqcgtdx.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/grsdmycqa.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gvycualub.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/ginojgabz.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gyhevgjdd.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gtcsztflj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gouyntcqj.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gikxqsgft.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gvlrwhcfk.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gqxwgnvex.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gdzdxcfbk.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/godmxkwbs.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gzitzfcuf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gyzmifdzb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gefwvpgnu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gymyvhtao.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/glqblawhx.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/gzhdyyaup.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gtbcosnxb.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gcnvhzswx.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gacrchqom.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/gtauvyotk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/goukouclu.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/ghndbfmdv.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gxexlsafh.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gnlpajdok.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gbppluwsa.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gbnjjbirq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gkjqrsyhu.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/gbrddigoa.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gzdepguop.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/grqobsqjn.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gcectmezz.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gwymplbuv.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gximaptpo.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gxyzoddij.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/ggbqczcrj.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gpilcanhp.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/gajcugnsv.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gidrxstob.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gjxuypwpb.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/ghygvzzvj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gysowahfw.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gkaufqyfq.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gszqctrye.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gyngzlhjs.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/grfqxrpua.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/grqrcnsuq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gejvsvzjp.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gtryytmeq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gxwpjtint.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gsfenlrxz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gipcegzyq.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gyuvslxgl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gbirpzhaf.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gwofmneuf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/giehpinwq.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gsniojvfo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gnkpswdkf.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gtaehsnzz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/gurrfnuxb.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gcgvpexzt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/grxguutly.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gysuespgc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/grrmwyrjn.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gulfnzzel.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/gecktyavj.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gwxoluuio.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gxchyynwt.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gnsztybwr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gywulucqi.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/ghvryfvvi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/grzrurltu.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gwrtnsnjp.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gfyynwjue.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/giyqbxwkw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gztefdsex.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/ggrrwmeos.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gvdvqnbuh.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/gcfywnasm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gyxkefmys.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gmrdcweaa.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gokfllhez.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/giqqespxs.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gmfahrtlt.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/grqzztrvg.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gfdcafdxt.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gzeihcwgl.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gqkipqmjs.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gsphqcaqp.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gdfdiyptg.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gnkafxbzt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/grocgqalq.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gsrysvsbs.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gqobuifvf.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gwluxptyw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gikxybibd.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/gcvllkytn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gzgybzizc.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/gemezrwed.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gpstapxls.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gfenxeele.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/giedgbblj.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gaxkfbguq.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/ganychplp.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gxnafiddz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gawqmclsq.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/grppjuwtw.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gvuozdnut.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/ganuajtyt.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gqegzgvsv.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gvynsiuza.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gdnuvtqrs.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/grqwkemwc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gzjcitrjk.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gjrxcuccl.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gfuyrycoo.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gugwvtolb.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gcivysxij.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gxrfqaurz.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/geaxvigqq.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gvfaptilf.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gddcvpzns.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/glukaoswz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gfivclvbn.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gjpiszuku.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gexdrnpgp.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/gvrfohcrh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/ggbloacyj.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gzpzwbfaq.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gvddilvxo.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gdokaneqv.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/glghpkixt.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/gaxhviwhk.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gkiajabrx.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gwgwsczrf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gasaasksm.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gkepyvshe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gorjjttbi.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/gvaptvvaf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/ggheebbwz.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/ggnhvwjqd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/glskqjirw.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gtlqgywsr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gpqtxwpwr.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/guddxwycd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gwfdtgdko.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gvpmctgvr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gpxzenpxq.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/gdbktugma.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gadoqzqfi.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gflryzrfv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gligpwmxv.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gncafhrrd.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/gtzrtlkej.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/geejmhsnq.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gaotvkbjt.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gdxjfkwrt.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gluuoohnw.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gjaoxfgmj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/ggynltwcc.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gwmzavhkd.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gwazrazru.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gebtbjird.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gnmlwkrub.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gvguabnzk.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fehbvm.com/Article/details/guufiponm.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gizwvnwzc.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gyskofdlx.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/glpoysyzs.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gekarfwnj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/gfrrezdvo.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/guzgnxmfd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcnhjqxca.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gwklvfutx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gidofxypq.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/geaknaivv.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/ghpjsvklj.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gvttztspm.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gtoihmjyl.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gfxfeqdzj.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gsxwdqrtp.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/gckfdkstk.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gbnosxyrp.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/ggupatmqo.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/gfzhzjgle.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/gbfnanukf.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gfaikzjhu.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gtqydqrhs.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/ghctfhezx.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gnwtlwalg.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/ghglnevmn.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gmkdebuyn.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gjztrfwyk.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gfythrrqy.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gllfomsrm.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gusnsegul.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gdvppksju.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gkkhgyjel.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gmijkwnjf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gvvgjfuhk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/guhjaximo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gtxpuqugo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/glxukpebj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gfnwsjvba.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gkmooqtro.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gkkaprjkp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gcoumftsk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gfixxgtdr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gvzawbinj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gxxghpruo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.zdbjq.cn/Article/details/gkripjuwm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gdyvqvhnd.sHtML


<!-- 参考信息 -->