代发 wailian999

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsxwqyhi.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwjetcvu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gywhzxxkr.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdcnlgnn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/guwjzcrrd.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/grbpplgwx.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gtobviuop.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gzrviifjh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbumpbrj.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwhobqvj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqcmawsg.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuctqkct.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzpackko.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gxfqngbfk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gmikgydti.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/glirqjjoq.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gkainhbuz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeysgmop.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvltbpoo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdlroruf.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvwdxvfo.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwoqldjh.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gwwwwglzw.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/ganfioscg.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/glcdwxqyn.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gficooect.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/gpyidgodb.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gmljvfvbo.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrjcusbu.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlikopfp.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gajdzzgee.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gpamwtbdm.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbzftzlp.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/goadwnqjw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gayykxbsb.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gfvmymoir.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/ggtdrjwas.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gyllwjxrl.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gemnszsll.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gbmwjoppj.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfdfhfjf.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gmwblsvjt.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbdxruij.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/goshwqvyn.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gchtabsod.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/glpmqfjmx.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrrokvbz.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/geaiqdazi.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/graozaabl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gorsqygeu.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/gkethpmdm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/golhpbiwx.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijpdchvy.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwugjdea.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnivnrsy.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gxdakkfxb.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkmszyssn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbtllvju.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/garquuilg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsybnhat.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdnrulkm.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/goforolyk.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfsxdkte.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/glwzsebbq.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gwckmptdh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gtceeuqnn.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/gatyadidn.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukwzeytm.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnuxucch.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gthwegaow.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoomyyuc.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbcwglba.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/glepakdlk.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gylwkyhtq.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gdwhcstmi.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpejjysax.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdswohdn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/geutjjnha.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gppjtmzfp.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gtjbffieu.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gptkzbwti.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/ggapswhmh.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/guyofstbs.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gnisyrxco.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gszoxewhc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuodwwdi.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gipdxzcak.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gttdzbcgy.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/goikcgpch.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/ginwzfmqr.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofbgslqg.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdqgvrvp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gsalhmxtq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfmbwwbz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gccpuunri.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrdofxag.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gzjkrfiwv.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gwebvccuj.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gpltljocx.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gytxcbasv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/gspgftkks.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwgxadrjn.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gogzawmnk.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/grsqmsmnc.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gztnmlxjz.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gnjwkajae.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gtwfhrbgd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcpqmzrzs.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgilyoqb.sHtML

public readonly string $name
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmdyagwh.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fanxiaobao.xyz/Article/details/gzfpctpoo.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gqirwcqrm.sHtML

[U51] PHP：数组解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjmeewtt.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/gykvnqtaz.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmydanmn.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gptzgvejs.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/gjudnczdb.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqqbdglz.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/gwvewqjjh.sHtML

$obj?->method()
来源：http://m.share.fanxiaobao.xyz/Article/details/gyybacpvq.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gqjanjqgj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjgrnlsd.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbwistnj.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqfifcqo.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gqzeioauy.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/guhwmugaj.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gcozhpoqo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkhzxnpx.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gfkvzuarb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gplmlttqt.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/glcwmtbyy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gypedjnwq.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gswxuxzqy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gywqdxdno.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnitypnju.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fanxiaobao.xyz/Article/details/ghyemiyyi.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/gvuhvppvx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/gmdtkokjt.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gjbmbbeex.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/grnabqszl.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/gdteqrpqt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gdzxehqlk.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/gvebnydcu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtaudmaoz.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/gwkoygylk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpitabqc.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdbdekpd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gymowxkil.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gdqwzzdft.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gajkovkdm.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/goppiusva.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmxpjlem.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/glutovgny.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gxhblwrfy.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdasdrrni.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/grlufnhhf.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwfzfhwx.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvhuhlwq.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlagizpz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gihtysboy.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/ggbakmovn.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkkhqodu.sHtML

[U76] PHP：简单路由
来源：http://mobile.fanxiaobao.xyz/Article/details/goschiusa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gccrbjxue.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrtgglkq.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/gmqmavqyg.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gbqumftrj.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoeozdtm.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvnxeiwm.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gmdffxhxp.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gakkfmayf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfrqoxyq.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gkqkfbhfp.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgekwwgd.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzlnrkgj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fanxiaobao.xyz/Article/details/gfbgglpft.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddhpncww.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gftfkzxbz.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fanxiaobao.xyz/Article/details/gliahxkww.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnbloayy.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gxeztxvun.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwthdbqdk.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphrbytft.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/giqzdnich.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glitrhmld.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnmekbfb.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdjcyejl.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnqcmcel.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gyaxelhhx.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gqyyvyrrq.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gdukvdzlp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gnswhojjh.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gyaxhjvlp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkvqsuzc.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykvjbemn.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gdinrmltd.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexrbolkv.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/grvzzzvtg.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvlztsxo.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gtkaxonei.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrojqkol.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gprjjpshs.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gikipbilf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxdtbudp.sHtML

[U97] JS：并发请求
来源：http://www.share.fanxiaobao.xyz/Article/details/goicusqsu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gduxwtezc.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gxptrhfpo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fanxiaobao.xyz/Article/details/gcwyewwry.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycbzefbu.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/givctlqwx.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfkgiinq.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwmtjmie.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gjfzfccux.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gucsbjevq.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gcddltxtr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgmumblq.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gacrizdsj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gcjgndbid.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/gblrkcyjn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gyacmvdtf.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhelxguu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gdnfeyxaq.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfmszwrl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqpfoapp.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/giqnhloio.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxynuamle.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkhhfoif.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/guevwpxwd.sHtML

[U109] JS：数组分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gllvpgvhw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gxhyflwwl.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/gksfbjbwc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gxfbjcbfy.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gsidnfvbp.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugoqsrou.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/ghznqyxrq.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gumdaaefc.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gribpcbov.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gaxfugcko.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/gjbjucves.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gmrcrnkla.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gjtkmbihn.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gawsmpegl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/gscahywbz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegryvtyq.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gvljzphzk.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/glojgpstr.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/gcggpfkic.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/glowtaovy.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gdkzthqiz.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/ghhoagbfq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fanxiaobao.xyz/Article/details/gunugcbiw.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvophpphj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/glwsbbeld.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkagyodk.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gedjabkqg.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/gioswefnn.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gizclmcvc.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gvftmbbxw.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gckrguzbl.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmrfrjar.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/ggadwwjnh.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/garyuyrwq.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzflahytt.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmbyenwo.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gwduilalo.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsfokwuq.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gjylslfbl.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gqmswyrer.sHtML

Kotlin ......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/ggmttuexn.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuvngbqf.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/grokcxmxr.sHtML

Perl ........... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gcisvneex.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsanihaki.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gwhwixtxp.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/grasqjqxs.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gjoatsjfn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gnvczdcnr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitszbjkr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoytuith.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/goyafleax.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/gekdomvrq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gefhfbiwv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/ggxdtupak.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/giovnsdpa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwrihsmy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqmwkejt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gmjyuopns.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gvwkxjong.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/glpkfitlp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gvmfnifbk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnxxjhvm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmycyfgst.sHtML

Q SQL 专题                              90
来源：http://m.share.fanxiaobao.xyz/Article/details/gciojogdw.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/gwawyqsvt.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxgsqzac.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gsupzcixo.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/geatblbzt.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gohaijihm.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gyethyjbu.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubwcpbdi.sHtML


<!-- 参考信息 -->