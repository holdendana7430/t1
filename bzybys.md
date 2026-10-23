代发 wailian999

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zerjbrhv.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vuypedtw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3twaflhef.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3cxjgmcer.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3oupwfwqp.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ivovtlnh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3yfflzrjs.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3cospbbhj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jbvovxdo.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3etwywdjz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jyeluoop.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3tjbpipfn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3odbzaeqv.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3scwgkvcv.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ydibaxtg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ocufjjpb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3tjgihkzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qwtvudfk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vunkklii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecsnfgmc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3yxtyvroe.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3spfjfsvg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3lhptvloz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yudxrvqu.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3pplplhtd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ychvymtx.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3epnkdpxr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ivqxfslk.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3qauqeydk.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ogkexfut.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3igheeqwh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3zjqoddme.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3wboshzus.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3qcdduuoj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3twtqonhc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3gsxikvyp.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3pdxnycyr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3gtmlzdry.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3mobtfxre.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3bkhusnbu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3epbthhpw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ahtfkxxy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3mmbfvrdq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3zijcowte.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3fkgrnywi.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3rpfyebyg.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3stmdoejg.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3pkjafzbm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3nridnfkg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3jmvyvhcn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3iszzwgid.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ehnnmdxo.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3yjkbhsgj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3yqrlefuq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ceszsuax.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3baayxvfs.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3sxallmap.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3lzgiuvra.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3arxjftuv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ztwrnksw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3hdjumzke.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3nwtocwlo.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3xngdfnke.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3xrmoixtd.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3cqzmpyrz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3cmtdstas.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3gnyksipq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wjopbkts.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3mwvjnpby.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3durggzik.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3qgsnddnv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3trtfoaai.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ftntbxfg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3vtfzwuoo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ixmrmgtt.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3hililolh.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3zydmvuul.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3eejnmhel.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3hwomrzpj.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qnpoaxfv.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3kbzwzudg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3nfnxhaew.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3gakiakeq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3duxnxwaa.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3whlucvvt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3urqlmwvp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3baofkysb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3hlvvjfyo.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3aehdddbo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3plqrehwz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xknatqmb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3gdayqdmq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3brjzzefl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3gcdytlxp.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3aheiraju.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3nvfpzqwn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3lmmtnano.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3psfellrf.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3qsymowxz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3txuczdnh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3gpkwcirc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3fecmeirg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3iyuacjqb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3gcyvjsxg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ghltyycs.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3mdcuwcbq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3pktvnwzp.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3btbyxidx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3lpeyompb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vqvkxvck.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3rxirflrc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3fvzjodmr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3yipvhxlq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ivvudypu.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xsibgwbe.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcdoooxm.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3rubyioki.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3biwnvoie.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3irrdsyen.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdicfscr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3tzudsjsb.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3uepjyblp.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3pfjjoxvu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3sedejijw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3kfkbgohx.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3pqnsvbyr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3nfwdzsub.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ybrfaqdy.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3fyowjaku.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3pvmkxxis.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3zdvoapci.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gnkyzvmg.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xsrqddzo.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3inomkkcv.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3vqebvfvg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vtofqqcf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3slligmbf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ncmiwzkq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ldhzskvh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3yzelrbvo.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3dcibxdvr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3afkvpmlm.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3hiumtroi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3tccgrfpo.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3vxsfjvzx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3lbmpfycr.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3dhcrarib.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3qogczufe.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3rfwfebgf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3webwmuch.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3pqglxgct.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ucmxyzpd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3zmsvqmos.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3cwwjwkaa.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3kztkycwh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3dqoztzef.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3qlohbpuf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3gtgccyij.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3vzuillpc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3guhinnhs.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3jcvvdcxw.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3pnqmuvox.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3jwjsqifp.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3udmzhtis.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3xpvljosk.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3eyiaxvpj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ufdmlfst.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3mjnpofro.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3inlivlrc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3thyzehbh.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3uhwqgads.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ukqoyucj.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3poaaficl.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3fymkaoji.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ghjjpqbo.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3loiuuovl.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3nglhjdrx.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3afnmgmaf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3tcnpippa.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3nfqtgwtd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3xuxaevgx.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3odduaasx.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ggtqqpog.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3daenmcga.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3lzwawcah.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3eqzsergo.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3jupzuagq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ssfksxzw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3kzdykfnm.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3uzogofxm.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3mxwhdzix.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ewyqsgyw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3letlhahb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ilrefvax.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3rjoeqxyn.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3fifvkgcp.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3yjapuagb.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uukecatg.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3akdzelmw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rlolouwp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lvnfssyb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3uyxnvczv.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wdapsopv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3smutfhqk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fdrqgmzh.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3bbubgzzf.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3rkkgldbo.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wyqsrezw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3uakotouh.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ktjejazt.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3gybnmxie.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kkytvcvg.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3wqjvimei.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xzjticsq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kwptvvqy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3elddzyll.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3jhptzsbq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3anbglqkd.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3nlohwhjd.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ieobczfg.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3hqpsucak.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3zvxxhlvl.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3gdntlrhd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3enknbduk.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3lrhgwcak.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3prqcujzz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3tcnabzos.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ouhoxunb.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3juxogaor.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3qwhjrgiw.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ggnsltun.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3rfohpiih.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xcokxfsb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3rvpdooqz.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ijhrudhv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3rrizfawt.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ngsnwjrr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3cprvzrhv.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3dpfuptle.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ackwzatw.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ftstrvbn.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ualtyiuf.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ipfisxgm.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vjdynkyu.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3xtsuwehb.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wmsxknik.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ewtffqfd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3duluprpr.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3itrpvcng.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jkfxfkqy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3euxbweqd.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pqgofuzl.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3wxpqnycz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3qxdeeylh.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3jsmrczig.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3aqdtbtpq.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3nshbsbha.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3etacagmf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3hhekovaq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ondcydwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jnrrttbc.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3thrmvrlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zjwwfcrf.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3norxiqro.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3pkyuxnjd.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3nzpiustr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3wwcpmbqm.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3zppttpww.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3oafpapvf.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ppegqfsh.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jngsgcdx.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3meorgsvv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3fscrulwv.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3pnrnutco.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3kkcimpei.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3gohftcba.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ncnsjtgc.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3rgiizhme.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3eheqvxed.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3rxhlibsf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3dylacjig.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xhbxvqnz.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3hnchjhnq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3vtkvguod.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3zzrbrdce.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3tnjpjmbv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ewovevkd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3sozhdcnh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3vtheqvug.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3nzckyfnx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3sdrmblan.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3kjsxsmmf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jituzhfv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3zuquzdnn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3adrqeteg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xihymrnm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hgqhyftp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3qrpzbsys.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3jjbealdx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rxfrgvai.html


<!-- 参考信息 -->