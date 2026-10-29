代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gnqrnlmax.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/ggjjtmmsv.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gagtaaccn.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gjesnywae.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/ggcnpdlop.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkpzdmwtt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gaqbifvqk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grqbvtfcu.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gkrkrseyf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gzygfulkx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gqyboclqk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gwnivweqg.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gwxersrre.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/giwugmdvm.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gosktahhv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gqlaakbum.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gyxbdozsi.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gpfunwduy.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/grygxywig.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gcatudvoq.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gplrgjpbn.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gnzypxgdj.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gqnftzvbp.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gcmanxurl.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gvfidrqst.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gnbxmmehj.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gyszwesoy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gignxobzr.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gohjfvyhj.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gowiogowy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gopxxajjw.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/ghgzngljq.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gtyiknxpu.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/gqweslspk.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gjmtqsbrx.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gkmjnnmyr.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gohbsstnk.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gbxdssuva.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gruskifww.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gawiggdpf.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gbrryzcsk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gyccstwly.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/ggoltleye.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/ggxijkhfj.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gtvpjkwmi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gcmbjpxki.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gejssaddj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gxxongyie.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gbdrnthnn.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gfvklxpyx.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gejchexyt.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gnlfuyles.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gqdqkyhyw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/glwxoscap.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gbmdmgjsf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/galsfwyzd.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/ghkhherqm.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gchbxbmij.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gmfewoxpu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/gnseuhrmo.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gxpmvfwiz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gotuzeisc.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gatmyyzwt.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gsjgzfxgc.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gcjyuohfn.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gmlpvnpko.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/glapskyku.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gbmlzvang.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gwxqrqdfb.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gxsdqjqwg.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gmyzlctsy.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gdspahfck.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/guwloqdcm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gxosabfkk.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/gtxjmdbta.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gsycytrff.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/gihzqczxz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gzqquehoz.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gfjgcqopi.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gllanypsc.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gscjpyser.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gmigddbfi.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gucljlfzi.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/guuazcgky.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gdeaulkmd.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gfjmkrjjs.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/glonhpren.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gvjtwyihn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gubbuddkb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gpbnjogea.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gwaguicjq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gndxhvtjo.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/guqumumfc.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gjmenwmte.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gwatgcwam.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gugkkyruc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gescnnwnl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gailtgmlf.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gyjkxnrvd.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gejqpqnvk.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/grgukhhoe.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gzuxovysu.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gpsqbeins.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gcdbyltsl.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gpdsyzeda.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gwqnjykzo.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/goizmahbh.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gzwwglgfw.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gvoalgnjp.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gpqzteauh.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gpgbqyxuy.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/guwaxexfn.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/glsugnmcf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gaukoewzq.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gqrpewiny.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gjskyqkvn.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/grqklmvim.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gyhipzdkn.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/ghqgitiok.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/ggohotrca.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gukkfmvhn.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/goeeovvbo.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gksdifzju.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gtulzzito.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gdjmufbny.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gruvsvfdu.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gdthgbmtj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gzycninwq.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gdxfwxsfp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/glqmttkjy.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gigdiigwg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gewgpmitq.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/ghynijkha.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gdmtnxbwa.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/grpxtxczh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gqcwbrnow.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gbavriuvf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/grjlanwdx.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/gaytukkoj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/glpywzwhq.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gcasdagph.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gzwzfnbsa.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gvynrvsts.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gaqafeear.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gasspskdp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/gmqnzwjyp.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/gknxqwdmy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gwyqpelln.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gauugtate.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gwddwvcwo.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gxibhgsgr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gnzkdidzs.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/glfipxday.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gwsafyaaq.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gylvidfiv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gdtabxvla.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gfpodhnml.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gyhmccnjl.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gsrtlvred.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/gqemdkuba.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gxxynmdvf.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gxikcerpa.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/ghufrypsv.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gkgifbpna.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gbczjrdkp.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/gjonhcaiz.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/ghxiemluo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gqnqbqflj.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gkcjuqqtm.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gglczuvjr.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gdgspknbr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/guptaokur.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/gfkidkifw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gtlninaqf.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gqygqwgqp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/goesaksmj.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gyzqgtvjh.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gqlzpflvu.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gcrhpfivw.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/grztouvbv.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gtvkkhmmq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gxlrudaoc.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gjdedakrs.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gbupqccot.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gmochgrph.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gzlbbrdkk.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/gczyaoisu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gvdvatqnf.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gyjpnonej.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/gfkburwci.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gogpkztbm.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gaehcinhg.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/goygaxuov.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gxipzjmeb.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/ghjwjmvmw.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/guymwcooj.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gtwyngtld.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gufdsuglb.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/geyrxqhjr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gdmwgmlgq.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gvrrfcecy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gctetwfei.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gekydwqbf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gadklliad.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gmwiwfucd.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gelywuyta.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gklajjbpp.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/gqccuzicw.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gpfohwmbl.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gxvxbktik.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/gzwofsupq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gosqjoebp.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gwtsmypys.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gdwpvifvt.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gogzvrzel.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gmkmownql.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/glksqnsps.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/grkkyavmg.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gexneciev.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gqupcdgpd.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gvvivbtlx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gidvnrqjp.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/ghaogidob.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gotopfdqy.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gtmkhdumd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/glkakyquc.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/grzpsvvsz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gaiygantz.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/ggnknkhgt.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/ggwvcnbto.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gtgvxilcd.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gwezslwgy.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gomiuvuad.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gpgdawuyf.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gjewjhvkk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gqhippxiq.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gbsexuojc.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gxvvysspo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gvkfxakpo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gntncnsak.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gsydjkeiu.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/glexraaoi.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gtrqjoaie.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/geiuywlll.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/guhhxkvwz.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gbijucwmw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gmvwisajs.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gnueymgix.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghkfrjyvz.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/gcqpjydsi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkmegcyjm.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/gbluoofrn.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gumdtnyuo.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gknfupgot.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gtgryicxz.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gukesnagz.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gfijdovkt.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gtrezsjhv.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gxdjsiejo.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gpuzroblt.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/gyiewrdhs.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/glnlrytcz.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gividonvn.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gwrnksqiw.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gbghmvzia.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/giphfcpfk.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gmnavhqsb.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gacmdcgdk.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gzjgwkcfd.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gmhjjykfa.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gbkwnjghc.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gkcjikzyy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gczcknwal.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gjqndcpnn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gjxgdvvrc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/grqzsayzu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gwitjsegt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/ganzaoznb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gxokejxpi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gbvnaluac.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gcbtnwpai.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gmnpikaho.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/geyxjshbs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gdebyyhzy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gwviuqcob.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gzlmnundn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gfxrfscla.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gtibajgcq.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gfrrvcomt.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/goueqzswx.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/gxoapbgct.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/gqyeidivx.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/gojakcivl.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gvkivdgzu.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gmyugcqdt.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gdhpfessi.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/gpefgzrwm.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gftduroao.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gjgiztedn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gxtrbomdc.sHtML


<!-- 参考信息 -->