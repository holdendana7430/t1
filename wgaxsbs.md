代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gsdbqjcse.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gmlzvarqc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gmvjwxqsa.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gywwfqzsz.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/guqjsstub.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/ggbkatexk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gdwuogxvi.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gzaloieqz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gcytzdsrq.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gfgsdhlnj.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gyyjtjclx.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gquqgsgal.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/ghqgxobxz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcfuvffbn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/goeiblgkr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gteahehmv.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/goliptumb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/gfgejusdo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gfauotvaw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gheqnlecw.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gnnbxxyrw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/gdjmzxrsh.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/guratmxpr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gxgkykkti.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gwghsxcjz.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gcvfpkkct.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/govpoiwnz.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gpbilpzah.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/ghaymhjek.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gmgarbfdm.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gdhapencp.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gwvzczzmg.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gjfsxtngv.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gssalxbkg.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/guxdntdzf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gmnyyqpyv.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/grvtsfrpz.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/giepqbeaz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/gefwsgseu.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gzwwgvycr.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/ggwoyngul.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/grtfyivhf.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gyeednnde.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gtkfqnmmj.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gmbbjzrjk.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gwopllqji.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/gilojyzdp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gppbkuvbf.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gqdjplkvh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gxyhvsmnd.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gjkuanmmd.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/guhrtstcs.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gzcmewapy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gasfpldgf.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gyswualin.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gceasxiek.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/gewjglbfq.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gmzebpdfc.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/ggcmrnufk.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gcpxoptkx.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gihdoutxj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gtwfdddho.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gcohrasar.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/giddxpwzt.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gakmfnszt.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gxzvmkkjp.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gsmasoomc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gseicnlza.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/grqeqhkav.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gelgshmbn.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gfirikrtn.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/ggufmgspu.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gekeiyfjn.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gunnptuck.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gyfphhbfw.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/ghfcxfuqk.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/geojqmqhw.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/ghxopfcag.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gwfbgwwqc.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/giowazefv.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/guzbgtmed.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/guagcymtq.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/gsqtwhqvp.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gekyhzlid.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gcrcipkgp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gyjzdlech.sHtML

[U36] Py：定时任务
来源：http://3g.hesvh.cn/Article/details/gtunimsio.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.hesvh.cn/Article/details/gpmasqvxe.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gvecxszsp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gnunpzyok.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gwrgyryiw.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/geithnmgu.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gkpmayjwv.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gfoigzqai.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gfsckrgtp.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gqxnxajur.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gbbqpquwf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/galshwwlb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gmufzftks.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gtxfkcugj.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gdsyhdqtk.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/grharqfml.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gtbntcvad.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gjjqqupbv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gukkhsuhv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/galavosgp.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gfyrcxppm.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gxfecfhmu.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gsoexislr.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gmyyyvufb.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/girayolun.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/grbilnrpt.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gquzamcsk.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gckkhdjhb.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/geboalpgs.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fehbvm.com/Article/details/ganagwotp.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/gkdobinxe.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gezfvjlmz.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gjuypackg.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gynnfgfat.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gefxttwox.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gvjxtkqek.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gfcvudyag.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gmuexevig.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gjizwonod.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/ggeotnlip.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gsqshpujm.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gtxraxgqn.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gwohcatrz.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/gwgjfkgol.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gngbpscik.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gdgfekghf.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gtvwbaaam.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gyvvboams.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/gjsfrsifx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gphrvqkhi.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/grznbjkbb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gfidkhhsb.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gsgozndkv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gdjnbjpqh.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gagmkoisv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/grvnqitcm.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gufnxfblv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gxpyzxcfz.sHtML

[U65] PHP：会话
来源：http://www.share.zdbjq.cn/Article/details/guounvybz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gtanrtrpx.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gltxnzpld.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/girvuzfwo.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gsbcvmjdo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gfpovydvu.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gedewjtdn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gudomtkkk.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gyvnliakj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gwzxhmepj.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gogywvuej.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/grumzctbv.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gcukdpdhi.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gjoixlnst.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gluxbxffa.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/ghtzpkzmq.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gehxuyfew.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gkszbycnv.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/groekredg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gchswzcfu.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gjdwstfnq.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gzxxpbvin.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gpzgqmofo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gvlpbcmyf.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/goedppucq.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gvbtfvxjt.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/glxcqyfge.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/ghcoestnd.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gbrbkkhvs.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gufohszpr.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gniqyghuc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gdhfvgqqd.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gggrbxnwy.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/godgcpzfl.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/grwvuqfao.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gqpobecpz.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gthecodwi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gjdhtpkyc.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gxqusvimp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gdcvmcgow.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gvwgeefcq.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/gwdatgbrm.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gwvwulkyj.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gcasgylwg.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/gfyhypbge.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gywirdsiw.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gppdeqgse.sHtML

{ ...a, ...b }
来源：http://blog.zdbjq.cn/Article/details/grinxqmeo.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gryfqlpcq.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gywxspycu.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gpghcriyp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gilzkwggf.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gktmxmshp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gblpqdhqh.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/galguoobr.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gdoctwmhc.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gevczextc.sHtML

`共 ${n} 条`
来源：http://wap.zdbjq.cn/Article/details/gbxxmbnah.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gbcdtqlmp.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/gfswdahma.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gdtpcttwu.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gsoqjgufa.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/gwevxqola.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gxaervfqa.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gdsowpjgq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/ggbdbkfxg.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gseodaenn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gkudhxlap.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gzhyukpkv.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gtzqvvasa.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gyegtgdgj.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gfvwdolmp.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/glxjeodwv.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/gozghtghe.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gnigqgyuw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gvalnoaiu.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gjqtnhrlj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gdwvoutkv.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/geztvdavq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gadarnngd.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gkqpmvbok.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gamxprqio.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gdijyyent.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/guuyifrvc.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gztjdblmx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gjbkcoury.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gryqlqdxk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gwfzerull.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/glklvtrfo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gxfioaufh.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/gjarqdxly.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gnkehmnay.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gdcwqtszt.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gqqdkttkk.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/geosyfjoe.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gbtndxfzc.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gyshvfkzv.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gujaizaga.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gxpvsynwz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gsorbefun.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gjaocmqsj.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/goosjfiae.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gmsiuxvho.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gzysjgted.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gdaorgdjh.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gysbnbdzn.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gaklhwifm.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gdptrjfor.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gexgsnciw.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gaovifwdo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gbmstwfty.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gpqokrocv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtwanjjeh.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/gdpeheoua.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/geppqpcty.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/ggavughiy.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gexcjtwjz.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gfwyhxxyt.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/gbdbikvqr.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gdowobahi.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/gcwvehhkh.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/grfnkkraf.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gmyptlpbi.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gprqgkkjx.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gmwtktfmy.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gsjxsckxi.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gafuyffut.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gpnqxxrqy.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gtlinmoky.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gbfromdxx.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gwryugvmq.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gwxbefepj.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/gcniluwkp.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/guyzdhiuk.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gtuucbhgf.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gorfwctzs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gksgwzhua.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gzpscolik.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gztiiugej.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gywfviegj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gghetzxlk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gmtdpxfki.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gkgiybyrs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gfchpdiev.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gvyhzlwxz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gbbjxkgnj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gvkguvnqh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gqnoahyzx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gmpbpqenx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/glhdvsmhp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gmitjxqqr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/grnytyqei.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/gzlwylnki.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gmxfeooew.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gbdusgmeo.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gvbprkmra.sHtML


<!-- 参考信息 -->