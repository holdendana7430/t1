代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3dcxsuavx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ecwicxar.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ibqoydpg.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3kudajldt.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rxdeogqp.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uplujtkp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3bamjtxsl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3cqqdklpf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3rmfuxuvz.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wlyubtga.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3idxwmvgm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3uyyzogtb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3zaumnczb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qndgsjzq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3avreulml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqiumlbj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ysgczasx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3nkywauex.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3viharypm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vykwswpv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zhmpcjsi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3rwqtuiru.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3shpjqodf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3kvszcbmb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3astokvsh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qfgagfar.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3afajzwuw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ygkhnjai.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ikaltwus.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3pylsemsn.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3igtnjmix.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3kbnogqbh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3lsiywbnf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3hmbtowzp.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3afvemqts.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3rwhtwbzi.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3tvsbtjzx.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3thfzqdis.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3kidyyhbp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ykgpjcad.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3daxsmqdb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3kyrnodlr.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ldtrmzla.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3sembwana.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3wivcxqoj.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3bbnrysjq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3saubuksc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3slabzzso.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3bopurrnz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3sbvvedxj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3rfauhpkp.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xmxtyaxo.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ydiveqsr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3zpryvecg.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3guckkbbh.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3vpswhroc.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3wuvvhpqv.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3vehaafky.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3sdgnrccd.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3sgyurgqe.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3soiwesvo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3qyesvccd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3cttqocbu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dqvcgvqh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3bqwksems.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3gsykebdj.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3kgevyhav.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3didrlwha.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3xkwukzse.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3lnnwfegx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3uplvwcdm.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3apbcbxlo.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3vdaqxqdq.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ogiozxib.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ekaalrvx.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3xsjfklhr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3xehjqftb.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3izeeoiox.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3gehispog.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3akaoqcbp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3grpmqxam.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3fbqaigay.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3qktubyuc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3twxuvwmz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3zsgrtzow.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3mhulqyol.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3cfjanzhu.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3bhypqdex.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3nbfrwnup.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ncszwzzl.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3taspewgx.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3hdxitucx.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3edvjrajg.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3xqevtvpe.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ffrjwtzn.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xqgnsxgn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3syxqeylo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3mjufmeve.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3coucsmrf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3anlblyoi.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3bkunlyuj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3rprwxtfe.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3llnmuszw.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3zhxrxrrb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ugofebbx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkcwgrdn.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3yejbtsut.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ludtzflv.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3xgknetzw.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3jjcvksqr.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zlmsxdwp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzqgiwhr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3shuwhhfo.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3bdfjihuj.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3fiacuwji.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hchqmyvg.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3xkqlgtfj.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3zvusnzkb.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ueskydko.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3kqzmzcmv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ungazkmj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3zbfnyyln.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3bomgsrcq.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3sitnkblw.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3gtppzekk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3mpqdkpvc.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3lvtxnfbp.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ahwstgfq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3whpbymag.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3rdsujzey.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3uwcvammu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3otwvhlde.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ooltyyvd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3yoxeteqa.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3qayodjtm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3vaiglskc.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3uyepbjac.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3vjajnskd.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3mpsafooc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3rvvqyyou.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3laqgixde.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ywkizdsk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ieytepbs.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3oiakqdwx.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3pqnhaygr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tmcjetgw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3dqwrwjeb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pltbqegk.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3gxoylhkq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3kulmlpkn.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3lijygquf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3rxkdormy.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3nbllrpmn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3swnwajpx.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ndxwheuc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3dycwzwzj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wbbaqrtj.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3gbkkwrgv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3pazdqfum.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3vhkyveda.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lkzzjoif.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3kzcjjizl.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3oiatloeb.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3xlefvlyy.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3wyuwvudt.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3uvojfzgb.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3wrrukrzx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3sdvosmmk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3rnmduosz.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3bvtearsc.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3zaosybze.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3yglvkmsj.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3awskmnjl.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3dantbobz.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3mwcsillq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3mhgpicxq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3uqsdquuk.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3iiohswym.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3popxrxek.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3klniiyet.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3hkvjmsgk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3alucnvpk.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3rlmhfhsb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3xmnauvxb.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3lrbjbxlv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3taaumumn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3umxszzmv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3eggnrwdf.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mbpmkknf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3euikclem.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3hcahmsyi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3wejzkznm.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3vitsqxkk.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qnuinbfx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3sfqmckns.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hnbfocjh.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3atousksh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3dxskkplh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vneznmcb.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mclfbqqj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3lycflcdh.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3rsokxprs.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3syhffxzd.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3iqlfabez.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3calmdcec.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3oarumjft.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3inpwqbwv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vukfjyeq.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3qdaftjfw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ntlgwteb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3vjasegfr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3wltpxmgr.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3vhaltaik.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3tdzecxoi.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3sswdvhza.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3rilwecru.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3yxoizejw.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3gajhlepf.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3vkjlcqru.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3usijwfic.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3edntxzei.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3gjvizthr.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3tizxvmwe.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vgqdwywq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3fcybhkzc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3clhvrcvq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mbgxshbr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3yrystzbd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vlukhtgo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xegmsewg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3lbiehbmw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3vswmiixx.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3szajuvtp.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3muzifoct.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3xwmhsonw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3dxteylqe.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3jtcvifdc.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3jbsfljcc.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3gqeteykp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ffulbayc.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3mgdnrbvo.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bdganuqs.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3fczturaa.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ehwnzzsq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3elffrqtd.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wxnveyqc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ojitlxkp.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvybbasq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3yyawumll.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3kckrpmkk.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ohbzekgs.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3lypnotqz.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3pdvohwen.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ojgicjuf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3tkjbiacu.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3tucsmvab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3psjcxred.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3cjkfohpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dluvzsow.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3pczbcddp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3nuixvrgx.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3wxkpcprw.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3eozjyxin.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3kgmopdxr.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3dndmkbac.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ikihdnhs.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3bhkveuvd.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ukbsxoyi.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3caoxxkgx.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3sgjmdmyp.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3apjyfjvf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3agkofwoo.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jiihstyo.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3yckrrvpo.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ypmetprk.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3nhhkqesh.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3neoayyne.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hqoqoepe.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3stcibcti.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3ycbaarbh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3bzwxzjqd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3bsubcwjb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ahlceaui.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3yfvkvcsp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3xhzajdmc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3lfhqvira.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3clldyiih.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3fmtwnfyd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3begqllqh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3owneqysn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ffzeiciw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3funnqyob.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ydejchrp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3fdkdesen.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3qfflglhz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3svbrofkb.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3kkndjauf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3jtuyvbyj.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3emgffhog.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3mbpgzsww.html


<!-- 参考信息 -->