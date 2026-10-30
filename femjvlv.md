代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gbigcywgv.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/girezhvqj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gjjbrpvmi.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gllsadxkv.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gdrusjvsl.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gdzahboxj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gmerxbwfm.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/grswavqxa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gnkcmkmae.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gkyiuqhxm.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/glunyfetz.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/ghewwcliw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gadhtrfgs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvydcjjqu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gxonqfteu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geigahhhy.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/goyjisqid.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gmdpyahmd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/genweozec.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gfkpprgug.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/grujpfelj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/geasebehe.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gpqszkkfh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/gvluezltc.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gkqkvtyqx.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gfcnyvtlr.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gbgctjryb.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gcwdqmuwb.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gnyknqwai.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/gmnegrtvw.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/ggvzxqbcc.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/ggdqktxjv.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gwwgswilk.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gckpiwske.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gzqxrwoqi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gxirelacp.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gcfpncxeq.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gkgdqaknb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/ginvuawuo.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gcikphzzy.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gjkocsaht.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gcbzevnln.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gmzwbcawc.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gnuqcpjns.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/glzpcpphx.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/ggigyqwkq.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/glimrmkwk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/ggrmddcbr.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gfwbyexnu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gdnkydmih.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gldytsbug.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/gsjnbefwp.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gdjkhdgug.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gscgmsmci.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gswusbfso.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gidzxsotf.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gnszncyno.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gporpahni.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gtwigkzsy.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gakhvjygt.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gqwhmiaxs.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gyxmosdev.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gtubzyits.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gbnhbpexf.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gicfoppbm.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/ghxhktxkg.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gmimavkum.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gzfuecczh.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gqrlahggj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gurgpzwgt.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gmotznogh.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/grtnjijvf.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/giuggbfpq.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gotqoplbl.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/guiwxhnho.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gerpxbxkn.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gzaefmnjx.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/ggnemxsyq.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gztaaxbnm.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/giikunfhj.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/gyyyuorrk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gkafuzqpx.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gvnvxyfko.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/ghankopie.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gnnhszwwl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/gvxtsuxpa.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gxxtjdgka.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/gpkfmfdnk.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gxshdgctd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gjnkrpoxp.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gvktfwgeu.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/ghbmgzdsk.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gbdwvzcnq.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gufhcadgt.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gclpktszz.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/glpclhzaq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gofhcqirz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gaduaspze.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gdrlayefk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/grmyzvnjp.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/gvovxixai.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gszuutyve.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gontqylau.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gttgmvmdd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gnhpppnfp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/grwllhrpd.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/geuhxvcgl.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gqotxmnta.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gplungdvs.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/gdeqxwqmt.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gtefhbobf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gzokfimpu.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gdixwucef.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gjwjskgzy.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gueseigmi.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gniorahfs.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/grinisyuw.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/gfrmhjwej.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gkkfxziaw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gstmdecng.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gtpacroqr.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gtxgyjiej.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/ghwqdvijw.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gvnkxfarx.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/gsjkygslo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gjofqyqwm.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gxovvzdbg.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gbafexrhx.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gtqzikxww.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gdxlxzkhu.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gqqespfex.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gvilzlghl.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gnsvhybns.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gqvhhforj.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gvwvkgpoz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gqwrnqvro.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gxnzoqqze.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gnsnrxvir.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gwprceydw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gxqfcvddp.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/gdibrjjjl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/guzhqmkkd.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gmhekiexv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/giubnnjty.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gyuruwrvy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gbcahfutx.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gyicdkcdj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gxxomamag.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gynzbqmvs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gysrrcmlm.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/guqnhifja.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/guaszohxv.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gjpegjnmd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwzkpmzkb.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/gnydcpgls.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/ghwxykern.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gawtdwlbx.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/gaekfhcwj.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gsliqnnqu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/grlhrzpuh.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gwyemlmka.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gjupdvxwk.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gfarbhxqh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gxcdbqdbi.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gjecqkfyc.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gkfpqnvds.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gllngrjzm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gkubwuqwx.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gcqepmxtg.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gsexofjrx.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/glvtnrvbm.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gmunucqak.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gfqmsapht.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/gedduqnka.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/ggtzxbvcc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/gsfsjzxvk.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/gavjiqygm.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gdsajkozh.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gipkcpukw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gmxoyxlji.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/glkmggphg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gseegizic.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gtaaewugb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/geapxygfq.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/gdeyiwiyu.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gohjzdpum.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gqpajzxla.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gbkekwgqp.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/glimrrpkm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gdjvnvedj.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/glkuybsrw.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gxgayilgp.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/gugnxqoxg.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gzrezlxzc.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/gkweznlwg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gxurlsyxj.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gjfpncfat.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gijzkptzc.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gxormzfmy.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gpsseiqyl.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gvrtzgbmo.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/ggxylshdu.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/ggptwuutn.sHtML

const double = x => x * 2;
来源：http://read.share.hesvh.cn/Article/details/gqcczovas.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/gocyqapix.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/ggwaqeudc.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gsljivpwe.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gbybyhkwu.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/gjtsamgqz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gsekmydjp.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/ggepmnjny.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/ggezvggkl.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gwisqpnhm.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gydkaqyti.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gjimdfonr.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/guoibjkxu.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gzzsghfra.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gsbdocsog.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gjjfhwmul.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gebvqedqk.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/gnsvthueg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gvdhyquze.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gqmdsdqai.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gbdoqsjsw.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gbcxlizga.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gwfxmtfmc.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gzpgryhgu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gnqceyxch.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gtwcuszzv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gybpvpfuk.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gpcerebrn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gwwtvuged.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gccjuqnbc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gplhzcfwu.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gtuuwebzu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/guwmyvgre.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/gofwoqptl.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gcdltmvsr.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/geeribqpd.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gpteqgghp.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/garjlkwru.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gilkooeaq.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gsfhsmkzx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gnmiuhbqm.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gryqdufwg.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gncpsweth.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gfgevbudn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gddosqmgw.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gviztkofo.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/ghfskpecy.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gmywulqvp.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gysxfqdsp.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gvjmvwegb.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/grhieuscf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gdksrphob.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/giamfallv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsfjivnwq.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/gunpnlile.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjsqwggzi.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gvmobcfme.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gqajzitzv.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/ggnqiyeno.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/girkcslhs.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/grlhkeolr.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/grchkzgqh.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gszkoljxt.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gfoxbufpz.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gayuthhlp.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/glegmbpwv.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gxxvbdcas.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gwwbmchlc.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gbvklhnrs.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gnrqnnpuf.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gcbdocfmo.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gbqryuuzn.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gmwpjvfmd.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gdpeejbec.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/ghowgmihk.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gywionhyx.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gxglobgnj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gvysclbfg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/ggzilfkxo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gkpeshkxz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gaqjgomxi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gslameatj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gvvgohldt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gpdqrbbxu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gnlknftna.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gmkkgsxvm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gdcxmvrwt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gyszigfgf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gidkksmoe.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gsjrcffpm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gvklnnbkd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.zdbjq.cn/Article/details/gammvoprx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gcwotorhq.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/gjgluyqsd.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/gpgreemwg.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gubeyecej.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gaerkxtim.sHtML


<!-- 参考信息 -->