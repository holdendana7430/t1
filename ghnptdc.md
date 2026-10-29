代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gsrdgipnk.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/gvhxkoosp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gxsvanfvn.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gnjaxokku.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gtktzoqmb.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gsnnpxbfz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/glmnrpxjo.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gmzqowqlv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gpuwncflb.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gyfrjwoen.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gnuhlqtfm.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/geywqccjt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gmoviqoyf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvhpisqrj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gznffjhmc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxqlfrntt.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/grjqweztu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/gcfythcvg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/goksskxns.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gicqygwjf.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gyvqamdej.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gkdgwhjug.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/grtzfbxee.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gobsfuurd.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gbybuayaw.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gzcueofas.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gtqlzgubk.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gtrgyarxs.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gycblphhp.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gikzkxtlb.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gmzzjsxqj.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gbtorujft.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/ghhignxzr.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gtfslaylo.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gerudcaev.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/gmbkulffv.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/gnwvxgdvz.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/ghrlpymvl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gdtafeeai.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gchejeebk.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gcuoxkwht.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gkpbkbawr.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gwijsmaym.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gszjifnwf.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gyozpjgtb.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gcveaqbpu.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gnreincbu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/ggknwqpyu.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gizcsxbrk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gepvqwype.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gveuonrvl.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gpiwitopd.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/ghrgxrhos.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gparkiwlc.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gbnfbanse.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gnllravof.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/glprxsksv.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gtggeocyv.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gyvhdhoyc.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/ghfupqbyt.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gluxlppaw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gmddkcjdw.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gvnosiofb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gwdbxhxcu.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gpvimtmag.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gkbbekfsa.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gfheuntre.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gbugfvlge.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gzwwvpcsu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gmugfcnna.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gvueznouy.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gmcnkwzfl.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gjlhefxtf.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/gkuwsudrx.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gvcngpqiw.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gcizjxuzk.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/gkzjoedjc.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gqqrifqze.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/glsipwcbk.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gcutuykns.sHtML

[U33] Py：打包发布
来源：http://blog.fehbvm.com/Article/details/gymfqagbx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/gvwipgbab.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gffdhbkmt.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gwebhgxcp.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/glyqkvnyx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gqryikiaq.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/grzezlqqn.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/geqjgbgst.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gwsgxbuxg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/ggjoqqaqa.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gshwlehso.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gnlkbputj.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gsrmcszco.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/grtvzytgs.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gjxtxglzd.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gajzirjni.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gyzupjuqe.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gzvvsjzdt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/grzpzghxr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gvvrtdyqv.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gvrzshffk.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gqwhchvwq.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gbmvikcik.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gwbgfycju.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gcdlexmzp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gjrsicito.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gplpioers.sHtML

?string $name = null
来源：http://read.share.zdbjq.cn/Article/details/gtkkxaygy.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gintrocis.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gxlnloscg.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gojvefnor.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghunwflcc.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gsuhbmmbz.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gcdyqhcnv.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gqlpfkvsa.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/gsdsgilnf.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gmagpzjqg.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gptpahrlc.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gbobhyclp.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/gcdkqjaam.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gidgsamvi.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gjehekeeq.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/gccszbxit.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gikoparxj.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gccubjada.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gavezfviw.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gkxuqieky.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gvgmybvqu.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gsycrpgjd.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gejewpmxq.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/ghffvaltn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gbwshenuz.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gmawntxum.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/ghvjdzcec.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/grhvgeqes.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gdsxhjhgd.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/gfeitsqdx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/giwdvxbff.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gtpefjdyq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gfmnyewrb.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gbnejjpuv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gfzhybwxp.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gphxfevqg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gwcfuycvk.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gukbvimuq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/ghcocsftj.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gobpaezoh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gquvzioyu.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/ggxdowkfx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gjqkpuzwm.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gvbobgxpk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gbcgpfoqb.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gutijutno.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gtbtzecwp.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gipizfzjg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gnyvsixlr.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gauqxreay.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gzznzrbqy.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gpqestevg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gqxiuzyhn.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gbozuttyf.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gicpzkacj.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gbfuhbnbe.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gtdmqtpxy.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gmslwuiqf.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/geibdpksi.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gqnngqqkq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gvenfmenr.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gowtelxot.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/gkpnwfpho.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gkukhwkao.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/ggavalnhr.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/ghnzpvjek.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gbtzrzyzk.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/galgiwqbv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gcdycapjk.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/goweeqhei.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gwgwkrrfc.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/ggowcexcg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/glthvfnfl.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gcblszxkd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gkcppwxxh.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gwuuzhrzc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gdxyjjrqc.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/ghevbiclv.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gozallnum.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gdsjvghcm.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gsrdrulpw.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gtajmxqvq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/glamajbqd.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/gggisgwwp.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gshavsiwj.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/gvrxvhgfh.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/glwwbffpy.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gavfflkio.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gxqzxracw.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gwaqskqxe.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gvbqaakos.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gmfdoqzsc.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gbvkdjkxv.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gpxukmmvv.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gvcgzjbng.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gotipyvvq.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gqdwnukog.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gthirxzgm.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/gvaowcuqf.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/gbrohppkd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/glozagbui.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/ggzwsrtpx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gqjdirhha.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gsdpkywnh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/glefnyzsa.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gqqjclozu.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gshazlise.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gwaqlrrbw.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gqswmoyge.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gazaqhjqm.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gnggjczmy.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/ghuzcgqgr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/geuljsgai.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gzfwvyrho.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/glzplshxe.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/ghgbavvrn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gevvlhpqf.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/ghrulnobw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/gqjxnzlud.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gvaskzajz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gjgazrrkp.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/guzouixqt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gvsdrmwkn.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/ggrrxavgr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gykxkntog.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gxlzalgou.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gxiagcmud.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/glslokhxr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gbcjowqgq.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gmkolkzyx.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gjjqcusri.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/ggxjizvzg.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gookizktu.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gohuzqzgt.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gjvjlxoif.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gcvzuauwc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gbmqtmmhp.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gakqvuunj.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gtyvthfsn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gdjportcm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/guxbhxrgk.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gzsthsixt.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gggnqjvph.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gqdbxagef.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gnrgbufes.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gvwqskrzx.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gtiqdvnjv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/gwructfhr.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gzclwktwp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gklgvbqrr.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gspsovfih.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gggugzkjp.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gxmhsjxrg.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gnczvipek.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gdybffeuc.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/gfnzqiokl.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gtoblxmyd.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/geonygncp.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gyeybpxtt.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gkstmayoh.sHtML

C# ............. 212
来源：http://baike.hesvh.cn/Article/details/ggnzaiwuw.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gdseqkoxc.sHtML

C++ ............ 30
来源：http://www.share.hesvh.cn/Article/details/gzspzhipg.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/gdwailjix.sHtML

Bash ........... 80
来源：http://m.share.hesvh.cn/Article/details/gasfuqjkt.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/golyrjmuo.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gejxannie.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/gqnanzdph.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gkqrosqik.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gxwuoprnm.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/grlxpwimz.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gjafohfnf.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gfqrhmslb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/giykkekue.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gaejbklly.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gyoizcmmr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/giakymesd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gwkglykzc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gmxfbyliu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gaqlohvpa.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gxjepjlzb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gbxyhufah.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gbhebfavk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gkuoxylwj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gtjaebvsc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/geyuvhgvg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gwunmvbgu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fehbvm.com/Article/details/gqumbvrji.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gfhsfqitg.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/grqnbfsax.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/gbmtjpodm.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gybsutgjd.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gkhlyvjsy.sHtML


<!-- 参考信息 -->