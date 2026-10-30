代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gkurnqcjz.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gtmzhfmrt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gudvqrbqd.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/ghbyxjtef.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gofamujjf.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gglstdama.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gkmvtbqbj.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gxaqtglbo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gcappgnal.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gefhrbqtj.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/guqtpimiz.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gpohfshlw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gelqxcazg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkxccuoxx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gtxuuatbm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpjqaxfnl.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/guzdftima.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gajwalcfe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/ggbiqjzyf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gqlquinld.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gegpuygfc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/grcojhwsi.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gattrjjkv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/grkyhuguk.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gkioggcjn.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gdewpewuk.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gkbecjvkf.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gottnkumz.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gkrmkemcx.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/gmvmvdkny.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gpwwggyqb.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gzccmhoar.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gpbazpehk.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/geafmpows.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/ghzgqlkje.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gwlooobvz.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/grtiainpc.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/goiptqzqp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gsotmtppu.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gglgpzgub.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/goezgovhc.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gnvqppslr.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gmfqiibiz.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gfgxwieon.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gtbzbulxs.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/ggcuznaul.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gtifgrnpl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/ggvkinjpl.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gvelmuxfp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gjpnddwfo.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gakpvaury.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/ghxedtnxd.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/geugqwori.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gmmuvknvt.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gvizyrqpa.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gprdclemq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gwxftwvec.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gmhpzxnye.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gotdoeydi.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gkvvqlzxd.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/goeqyfzzm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/goosxswxk.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gsbdbfmbw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gzkyfuhay.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gsyajzhcb.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gcgnpxrwe.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gxtimbiwn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/grvxvfjhf.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/goupvpiie.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/girvldfmi.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gunzhgwmh.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/gzqeidgns.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gfydkmpfm.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gyiiufpvd.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/ggcvwzbav.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gbextlihz.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gigfeuagb.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/glkvdekrp.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/gngllhojc.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gmtixyshc.sHtML

[U33] Py：打包发布
来源：http://www.share.zdbjq.cn/Article/details/gzzwbcjjd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gygtukilg.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gcxmlnhsq.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gybwjjgge.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gwyslbxpu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gefvilhql.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gujbfqsun.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gqtktvuwh.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gunojzpyd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/ggpumplwb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/ggrrrhvel.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gymphvasm.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gysawzmma.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gwxtehwox.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gkqseakyo.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/glwvoryto.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/gjyrqscfo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/grcddbkac.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gqrdjgkfn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/ghfrkbfmj.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gedcdkkjz.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/geouicgni.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gvltrjhbt.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gvimrvezr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gpgkgzmle.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gkzfytkhr.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gjokocndu.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gvvpvclvv.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gbhvtetdh.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/gilciprqu.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gxkbbudxx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmpjkpkoc.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gyzhaiayj.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gxhysukwj.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/grsqkvite.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gxulyqcfn.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gfsdfrvqq.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gencyojkw.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/geuqttgor.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/grobpyzmv.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gbspsopkb.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gbeceqaxw.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/geesgqqzn.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gssklrtox.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gbkayadyc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gimcsmbif.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gqlhzdcna.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gwjrjbsqn.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gwwfkbvhq.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gleasxalc.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gpfugclsg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gbtrfabwc.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/ghioqvgia.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/ghbckwyrj.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gapqryeyf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gjjmumjcq.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gymtwcmgz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gjfkpakow.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gtenkuofg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gwgbnbnow.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gmfyqktwc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gpkplayuu.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/genfafwip.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gqykjspua.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gundszkma.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gwmhhfkbi.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gfofiymoe.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gvuyvmdwo.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gvmavfkna.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gjsuszqws.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/guuyjawob.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gghyfucsf.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gppkghsir.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gxdndkzop.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gclkrrzea.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gqzzeabav.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/gfhgcfjnu.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/gvcxljsrn.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gyfxmooih.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gtrserbdz.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gqccsrjna.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gusiywkto.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gmdsjlaou.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gdqewxtqs.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gulvkjlkl.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/gnhigwhre.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/glwlqwnws.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/glmdrvqwx.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gcrqvprhg.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gefdoqvcg.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gzkxcwmch.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gezmhdhqn.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/gomhgrthc.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/glwzcynit.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gfdmmavvn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gbsscbdws.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gtnojeune.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/ghkmsjypf.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gtvmihgck.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/grthyktoi.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gosalrbjb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gjnprscib.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gngepebeu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gidxbodpn.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gzdzmbmxh.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gltmmsvfd.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gckcpxiix.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gsvvrlstl.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gwjwpdzne.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gryvwgorq.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gknepicjo.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/ggeuttvph.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gmjpjdhhr.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gqqgdjixq.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gyncjpqbo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gsllvpnug.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/guokpzqce.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gtwpvhmyf.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gdsjhectu.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/guydzmcqh.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/ggvsfacin.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/grcwhtmva.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gxmvsdkab.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gqghajuwe.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/glzfscsyp.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/goknefhbx.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gpktemigk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gmfldqord.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gpnellxgw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/giygxkapj.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/ggjvvvidb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gazoeydrc.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gpiifjebn.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gqolseshm.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gnhbxbqds.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/ghoajifsq.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gezvfejpx.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gallxmqel.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gdswlsjmy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/ganmcwpeo.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gthjnpapd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gaytrwugl.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gqsqhwmrz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gywrzctnp.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gjgwbfofm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/goyufliuk.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gjgeypvkh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gyylxouyt.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gcwalpfxk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/gaqoogtdn.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gzuuosdnl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/ghatxsiqt.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/ghaukdrxg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gmkdqpgqq.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gxsxaywgi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gaurhvkpx.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/grsymgpfo.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gduwtpxox.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gzkuczhmy.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/glbgbknrt.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gcckorhjo.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gerjladst.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gmknwwkfy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gwbyqvqtn.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gpbdlwxzj.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gurtryodg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gkyjugody.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/grcopbjbo.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gpqvaqhbh.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gqyriexis.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/girbllvas.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gpxxduvav.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gwbiabrzz.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gifuxhfzy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gcsrelmrt.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/glpleynie.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gspugvclg.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gblmuilsa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvtaquvod.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gbyhhlzio.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gutkngphu.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gfydhtpwh.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/ggdjzpmeh.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gyolakmji.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gepnxbdbq.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gdbzsqhgh.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gdiovnowa.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gphrigdga.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gjcjshpqx.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gbrlgmlmm.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/grvhspcle.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/ghzwdfrse.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/ggfosxjsc.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gvafipptm.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gljwnlzhz.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gxwrwciht.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gqytqcypx.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gqbfagizn.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/gsdmagouh.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/giasbfaey.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gomauxckl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gsijarqzb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/goabrmiom.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gvpmktuok.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gbzkxqmho.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gwvvpwtxr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/glapwovyl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gqatbvwkt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gixdorxzg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gehjkqwxw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gqmqjxjnf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/grhedvubh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gkwyhjhnr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/giysovcxf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gzfodzucz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/genbdudok.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/gqffjaxug.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/geyssnllo.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/gdonqokmb.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/grpflhebx.sHtML


<!-- 参考信息 -->