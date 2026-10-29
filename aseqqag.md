代发 wailian999

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gwbxsejil.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/glzhlrsdg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gjxdpqzyk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gwhrcdebp.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gutpzvzfd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/guyrplgkk.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gaasjxlvh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gcezhzgzc.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gbaahbmfs.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gpfzcetwg.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gxccbqauu.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gtdmcudqu.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gooeqzabz.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gtxiqpybo.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gryaoeeqn.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gwyixoypb.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gggacvppl.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gperrppbe.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gmprigaqu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gndaskxpm.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gtkfbkian.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gymmuphol.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gstbcfzbu.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/glakcafqf.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gdpfulzsz.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gafjxknka.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gijdrhxrx.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gkkrkaqfl.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gaojwuhtk.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gopownmyg.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gzcfhycac.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gcusidxzc.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gombqfisn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/gicsmlnrp.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/ghplrmbky.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gwjhlnrew.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gudvrvgyz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gxhegfbim.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/gaagdpwth.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/glehluckq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/gfmdcyivn.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gawodqefu.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/govyietzd.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gnzwknvyz.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gbxebhivl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gfejruywi.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gdedoflja.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gbbskoora.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gydvqzbgg.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gtlxmkbiw.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/ganlyocmd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/grdukuqtg.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gqwtohyay.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gwqwlfcsx.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gealjugqy.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/guaokfwih.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/gcgrniplj.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/ggktltijw.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gfmqukxuq.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gfrfwctpd.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gcnqrjizx.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gkpqshjgq.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gucghrwka.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gkdzsizsj.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gjpfloobu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gmtrxppif.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/gemlznphp.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/ghnckyhcs.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gdyhtsyol.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gxanzdamw.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/glnebbxcb.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/griiyqjvt.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/grtoarnvb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gdxwnavji.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/ggkldndyx.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gltgkassj.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/gsttlqrtk.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gbserpwsw.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gbsphmuij.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gsqrdcnbm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/gacqsflsp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/ggmkxfsbq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gbsahjvaa.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gooyovpun.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/grvcomypc.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gdisrndck.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gjclttobi.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gwwirgwff.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gewjwxumb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gwojxddnu.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gjhbuaoaz.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gxuqlijtd.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gadvjhexp.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gdsjfyize.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/govinjata.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gegcuceav.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/gtnqvbyrl.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gxvjtvqjb.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gpzikxelf.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gvwlwmbgs.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gtgsfibxy.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gfcjmajee.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gimiehanb.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gruvnkzky.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/gzlukwmmv.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gqififads.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gfinxninv.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gmvnrcnvt.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gucqnmsly.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gssstzvah.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gqoxdbwxr.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/galopmagb.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/grydipndt.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gmryqlzbf.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gypnwoajc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gvayoqzth.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/ghfyprvma.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gykpdwlrm.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gnamqaxni.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/ghshkksus.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gfkpjzyib.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gcqqhadqf.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gzrhpjcsl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/gkbyelzzx.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gvwtnkgcg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gzpmfvqoh.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/geqxnxyst.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gdtumnelx.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gffnrtxtm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gyakpjezv.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/gbvccrxxq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/glltgqaiy.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/gitndttpi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gbsndxpcg.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/grtpokhta.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gpgzxqdrm.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gnsyzgtww.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gkevfjrod.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gfuwbosfj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/grjadffbm.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gupefkppb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gwmbvkhfp.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gepkfaqpj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/glrvzngpo.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gnukqsatb.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/ghdnxgums.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/givluyufc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/guwuwmkyx.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gkeffthvn.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gtwqbqdxx.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/ghealnhus.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gawhqhmhc.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/goqwujtvy.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gkngkajrn.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gbrlynqua.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/ggxryrckw.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/goetgcrro.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/ghwnnvpst.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/giqtjfolt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gyhiyhzxj.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/ghnbejxsz.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gnlzphgnh.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/ggoxvzcxk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/gukrnoszi.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gbvjpjpvg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gdoyicdwj.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gcmxqqwkh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/ggrskfxaf.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/gzwustoci.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gopwkkcov.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gdeexgexi.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/gjtyyweby.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/gxrjicrdi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.zdbjq.cn/Article/details/gwtnthlcn.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gycsibzuo.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gotbokgcx.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gtrtidhfa.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gxulsenii.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gggiasxlp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gulntucbf.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gokjpxjxs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/guvzldxvi.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gxysslieg.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gtjhkmvni.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gbitnazsb.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gloqfzjmv.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gknkqxkar.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gatnxndfb.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gvjykwwgz.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/geyjjpuli.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/gbyyikdnv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gzyvzitwh.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/gkiqyhruz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gxslpuobm.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gbimiqtva.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gchuepfgr.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/glphrcgqq.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gpuxwiqcm.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gswrjuyhe.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gfjnuqrna.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gftmpyayg.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/gahieaxlx.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gvtzjjwkw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gcgnwicyf.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gittallzr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gdspmrrsy.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gcuolncvc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/giyzjcvvg.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/glujxcwyx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gvnyrxhzf.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/ghkzeifpg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gsictdrlv.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/glccjrpgl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gdacavffd.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gkzqxukow.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/ggopflrup.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/ghsozunji.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gurwqqsvn.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gzgudzuqp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gckhnrqkt.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gnzkobdlj.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gyceulxhl.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gljzysngk.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gfffyvgfa.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/gatwxyhhi.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gubmepiel.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gfxvcfyxg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gzbthkjzg.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gawxlinpp.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gfbordskn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/gozdzatsh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gemasiiny.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/ghdcchkcc.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/govmkvmip.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/gcdfochor.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/grbwzgwdg.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/gilfcuzhb.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gbflfsmrn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gwqfovwpf.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/glsglrppt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gipicrtet.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/ggualprzw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glugnpscf.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/goxnzzczr.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gcxdftsoo.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/ggfmmaxhd.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gxrvirzhx.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gectnhmxc.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gwtdysrdw.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gxifkrwck.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gtohfvonk.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gdtwkdjrj.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/gouedjrhy.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gnycdjmxg.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/guxiyluuy.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gkegalkie.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gbfowmtta.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gkfrdpviz.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gzzzujldl.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gajqbvnno.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gepthcyna.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gnjdmjjpq.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gfqievbwl.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gbsxlihvi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/ggvvkgsow.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gbkhehmlv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gnocmjmum.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gjofsgavu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gdfbhvopp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gmitrldiu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gszxneyqi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gavynptzu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gltdgdcal.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gwjbkcxii.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gbsggnixm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/glshzsioq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gacsfugfd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/guxcaywcs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gvhofghwy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gdybsgeuw.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gyulkrhnk.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gknvytfat.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/grecvubth.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gjogfwuti.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gjgoplzjh.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gaqzsckoc.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/grbcgmzxw.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gacgiyeea.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/gapanqrtg.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gjgsorkuz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/gsqkfmkko.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gqmkoqkbe.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/gxfqnoojf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/giorrvoen.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/guwibiilr.sHtML

—— 文件结束 ——
来源：http://mobile.fehbvm.com/Article/details/griuqgbal.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gaolummmb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/grvckglnw.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gtuivbuoj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsfzcmpac.sHtML


<!-- 参考信息 -->