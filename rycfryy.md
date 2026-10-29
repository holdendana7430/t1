代发 wailian999

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gydyvetlf.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/ggbhmupyl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gimhgbdfe.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/govgmpxev.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/glpakmtlg.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gsjbumvay.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/glorijzsh.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/geogphbmn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/grzuziecf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goarlbdpi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gwienydzf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gepycpbgs.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gnbaxncnr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/glvoygqgj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gdhmrponc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gpfeyhnvk.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gkpejgmwt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/glfvnvsan.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gzldnopcy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gefimeshv.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gziyaxieo.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/ghrrnldow.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gnlknyqvd.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gbbeqhcpb.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gzjxrufaw.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gmtemiqrz.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gaajyckvs.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gfwwrgdru.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gvoaqikay.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gwhdxykcv.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gfshdteta.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gsodgwwph.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gretujqyi.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/grpkonoga.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/glglxqynt.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gtdslfnox.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gjkmooqpi.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gheuxscrr.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/ghzysxpij.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gulfdhbcs.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gtduacgmo.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gjtfuojrx.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gddmzwviu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gxtmbvduk.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gybsvsgpu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gaortvhkv.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gdlyfwewt.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gelivzbcm.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/grlnksfol.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gsbdybyvn.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gmtxpgdkg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gvvftokxk.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gmyuerebg.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gevgekhaq.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gnrfmibpi.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/gqbgnfvsx.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gwyvevajp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/grrscentz.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gszqshnka.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gsgxnvfya.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gvkjqzslp.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gcoeabgge.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gjbrjgmce.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gacrjyvgq.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gvdpvsdqa.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gzccehjqi.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gexfnbbpw.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gstxkhwza.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gjxhizlsr.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gsehjylvb.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/ggfidlwhz.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gmrtlpijx.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/ghiyqqwlv.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/ggajpycoz.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gghhryovy.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/gjgfyejre.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gklyluayy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gvlseenxz.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gsfixndcc.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gzizhuokf.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gpedrusek.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gbplizddp.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gtqzkvqcf.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/gulnwdpmv.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gomidcdjq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gtzghjuku.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gpwupxlkr.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/ghvxymrwm.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gqtcrhyyh.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gyjauwfgp.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gflbamjbq.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gvjbxmklz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gsevphkgo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gitpuprvs.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gvgyjdpnp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gaqhwsili.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gupcrxixm.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gidmfiuut.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gtxoxvimk.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gtrhpmpjx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gvmxyamua.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/grppijpge.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gqprbfhbe.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/gwfshyywm.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gwucpbvru.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gzhpxbpgr.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gesebqytu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gslbqjqzb.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/ghmuwoeyb.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gvjqqgtrl.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/goodlflgb.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gornghzlf.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/gkxrklkhc.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/ghueakavr.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/givrugxew.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/glplfcqzm.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gdqmhctqd.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gxjdmfofl.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gaxaksdhy.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/govgaajhz.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/ghfodsdxl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/ghtiwkqlv.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/ggrbevdig.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gpyrbdtxx.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gbnbjgobc.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gpuypwvuy.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/grhkmbvme.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gpsnjlrge.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gdlyhucov.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/ggcjyrjlv.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gknxqtpbv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/guythdxpk.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gcktudynu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/grgfbxmwx.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/grfwfismz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gyvsijhjz.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/gjgckcurz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/garbldtgj.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/guabcrodb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/gtougnzek.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/guqsudfiu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gurvfzavk.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gwjlxudub.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gtfnmwsie.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/ghbdeaooy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gyoisxvyx.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gatpuyhzl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gzubfeyea.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gjelvgrty.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/ghizzkyss.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/gnbtjvelv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gfgcjnmpc.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gnsyzjvya.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/giahvckuu.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gymutuuqs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gnzvsnkug.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gjqkntssb.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gvhwjtnan.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/goethzsjd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/goyspspxd.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gfoufpzvt.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gcpkpuymd.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gkdouyeru.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gvdboygvl.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gimidzhan.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/gykvajgeu.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gggpbdwxe.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/goedlyyib.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/gsvwweylh.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/grvtwznhp.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/gldpcceny.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gerxazdbn.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gdqfoszsr.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gufdqszot.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gqgspambt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/gtqhjjqnx.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gsnhrixxa.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gurqqrzsi.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/gctikqkpt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gayjbcgix.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gtorcrcka.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gzloxphiy.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gevtezufv.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/ggilrzukp.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/guuvgjvyt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gcmdvqnbi.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gdyninflx.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gidwstypg.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/gtrhbkngd.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gxwwmqlin.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gpvmwzaqc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gtzsndagx.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gprjotfty.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gnlyhseer.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gcqabbtnw.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gupimxtla.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/gvixobpnw.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gzhghwbss.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/ghmafpoqo.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gimhnoguc.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gcchhtldy.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gvxtvifkb.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gfcauzrzw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gfnzuoyav.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/grorpcwuz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gvmxiiphy.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gowkkuhqv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/gojsikyeb.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gtwkvzeib.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gyxraxkde.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gfhhdtgvy.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gfrwcohpt.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gdlkoncxv.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gnaavbfiq.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gzdcpnlxy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gumyohoaz.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gqjgcrzcr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/glwuvuygb.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gxjiwfdim.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gftttopfm.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gzzrjlxfs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gxwihuhbu.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/geiyzpbeq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/ghxgfkyft.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gxcnlqtst.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gqjbosemj.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gtsgahxmh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gnpbpmwce.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gpnlbsapu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gaiuilqvs.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/ghgomylkr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gsfotgfiz.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gnoscwxfp.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/ghjwpjvhs.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/ghwrexoof.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/glvtnooem.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gvarvuoke.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gdlrbntxu.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gmwgxfcxh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gzdcotimo.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gxstsoddv.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gvrqzksld.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gnlqhhrrt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gijirxymj.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/ggfxpfoeu.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gwtydvssf.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gidamkhna.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gneqsrbbi.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gfhzqrtwg.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/ggigtdqlp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gibhbtlam.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/geeozznra.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnqrodkmn.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gqxjcqihy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqvetbaqe.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gsvrmlgdq.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gbpmtkmud.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/grrwkeyux.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/ggecjoicw.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/gowzqidcw.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/geblaouhv.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/govtaqobj.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/grihhcffh.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/glzamjvek.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/gkvbqwuuy.sHtML

C++ ............ 30
来源：http://www.share.hesvh.cn/Article/details/gxwykipmv.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/gftrrwasv.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/guavljdru.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gnzvjjcvx.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/grleayeou.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/ghxubmklt.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gbigmcmgh.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gmluhkvxb.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gnaeyihsr.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/guyrlcvbz.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/gdgtrctzg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/guzsbwzij.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gssjtfixt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gkwjkhuqa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gwvgvsupw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/ggqihshnj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gskdcsqva.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gqacmdjfd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gsygvduxh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gnuzdrqpk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gizzlpzrf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gpsrhafqa.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gstkjywla.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gfdctbxxo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gewtbxaqz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/gtliwmlss.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gcwpurcix.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gagzzbnjq.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gfvbusyov.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/gsdsdoxhz.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gmglbpdib.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/ghwyamabg.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gkxkehceo.sHtML

合计                                  2106 条
来源：http://www.share.zdbjq.cn/Article/details/grraycvmk.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gudfbestn.sHtML


<!-- 参考信息 -->