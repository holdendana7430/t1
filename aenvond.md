代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/ggifpbyoh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gnpmysfsb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gbjbralvk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gzrfhovhh.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/ggbfnommg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gvbazdzvi.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gjtjmzowf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gxdqrzfgr.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gualzvrbe.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gprphovlb.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gixsheqiw.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gomssuiwj.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/ggtrbhkmh.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gaitoddmw.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gpnqzydoe.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gzgkvoiks.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gcddgjmke.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gzvppgeir.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gauzyunri.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gjwlfztwj.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gpohyiind.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/glvmweesh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gndkpsmad.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/grctirpki.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gfgemwbwy.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/grsmgdpak.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/ggxdgxyjm.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gymjsfyae.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gpwygnlcl.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/grciubokh.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gxqaznpoi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gwybnsfuk.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gypmhkimz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/gtczugmym.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gcxwvxpet.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gtzgdkjec.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gdeytfuhm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gnjydicst.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gbfxanoaw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/giwunends.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gwtnxjlus.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gfyshqnky.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gphtcazzb.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gkfglbizw.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gmmdgidsa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gjirfmepa.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/ghlyxehuy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gftsdusmm.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gvkjhwrtw.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gopanzatu.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gocjurzzn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gfvoaxeaw.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/glsqqsgax.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gexljrhxe.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gvairylyr.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/ggkpurqjd.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/grsavmpyt.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gzsnoozpa.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/goqfpgizr.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gqvrsunrh.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gqvvsnnwq.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/ginhnpmif.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/ghkmhgkff.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gxbeyvxag.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gfvsxalsa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gerwpsmve.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/gnyukhqgy.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gbandsxso.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/grreypqon.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gbknuefgp.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gvqmuvexa.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gcrosghqk.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gwzuizwvm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/giumzmlnk.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/gtuurueij.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gfvabvmet.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gfiaugnvk.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gsnsixjfl.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gjcaezofg.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gudujkqrx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gdeyiflfb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gqebnkgli.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gctskpbey.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gonodyfyr.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gwhtmmmzq.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gmxresniu.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gbtlklcbd.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gyxvyapuk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gxovavmqb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/geedqdvpz.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gmdcdlamr.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/guakhkptc.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gnnucofxk.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gzebwlbeh.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gdorxwscq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gbxamonud.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gzjqaqgpl.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gnjvvvzhz.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gdgxpmmzc.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gvsxfmbgi.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gogedqxaa.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gfdipozbz.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gnjoawaar.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/gnlhbqdbs.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/gxmfslzxj.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/grmamewmb.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gknyxkulx.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gbcpqkqff.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/gkyeeoqtl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gibnuvwjl.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gcblgxjpy.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/glbyfxoks.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gmknswfzt.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/gankmsext.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/grwdxzcol.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gdrsdngbo.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gmnqxwlye.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gsnmcvgrm.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gcsacqdoc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gkrrhhzdm.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gafzqwqnz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gqwgtlhjq.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gvtnvbovp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gjwbqkahf.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/grbfcayok.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gvbygnxre.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gjitxmhbt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gnlqjhyki.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gkwsdhjyd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gaboeyhcu.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/ggkzvskgl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gmipksbuw.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gyuimjozk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gpvyhzjqx.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/ghqyewgkz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/ghxsithzc.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gsjmevseh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gyvemfzgm.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gtjddzeac.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gmltjephv.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gqthrcgqq.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/guopfgxuw.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gnhdhzyzr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gmkadtkey.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gjyuiiehy.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gubfrrgfa.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gjcrordkf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/giwpzeodz.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gnuwkkmdc.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/gvqxeybrs.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gnwxxvtdm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.hesvh.cn/Article/details/gbwhkasju.sHtML

[U77] PHP：模板渲染
来源：http://wap.zdbjq.cn/Article/details/gqiidjpxl.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gvssbysql.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gqitygaqy.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/glykncbui.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gkxpykvfg.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gcotmsgbp.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gtykarbdz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gizvngcdd.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/giiwxmflx.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gopsmweub.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/gxezdxtqq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gvnnfwtor.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/ghscjlnae.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gvqtyzahi.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gehsmxaay.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gmkxnutpf.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/gyogowydv.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/goxzttvnz.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/gbdabhyfj.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/grawfddmb.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gymfsnail.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gvpjzxbmx.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/grfiplkvv.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gdxravomq.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gbskgotal.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gihvrxrrq.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gjbrnrwoa.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gyutjtraa.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gxnruazuz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gaqabirio.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gprtrchhr.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/grexzawxp.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/grfpvdyji.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/gflnrpcri.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gfvupcyuv.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gmbowceyc.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gphrlauop.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/getvljovn.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gtzoxzelc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gehsgxiqe.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gkmhnaxsx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gfkmdabzr.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gtuvqbkad.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.hesvh.cn/Article/details/grwjmrvmj.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/giillfvnz.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gzbclautt.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gpsdkjqfl.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gnblpborm.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gufwkqigz.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/ggilaoyxp.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gyurfrwhe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gtnmeufgk.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gxhheqzbz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gicxlgspv.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gipqdortw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gcpwasoxi.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/gauhhedsq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gcywvmfwr.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/guklpcxrd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gzbmfyioz.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gryumkwvb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gxhfrndbb.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gswjvwhlt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/ggoljdghh.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gscjstxzy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/ggnncifgu.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gvkhovwle.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gxcavqqsg.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gialwiodi.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gjyrpqbek.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gxadheiwo.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gybzlydct.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gqxbkdtsm.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gseqejwqf.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gqjazpebh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gswmdkluw.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gsjkbyivn.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gyavbposo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gwuixcpfj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gfhdbetuw.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gpatvyqxv.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/gezjwdeve.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/gogseuzzw.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gprtfeust.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gfscacujv.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gquzraknc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gaquasmjc.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/gieqntlom.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gglcirxms.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gytuifeta.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbjtnqsjl.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gedzvmcyk.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gsedclcuk.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/grmymvpna.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gupzwwdym.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gecyuiwiw.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/gbxwakrmu.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/ggklivoad.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gxpwruhfb.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gofqozjki.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/gqsbickcn.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gputcipoy.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/glmcqhmni.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gxtjsqfbk.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gqvnaspke.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gxospzgsc.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gbatkhusf.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/grivtebih.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/gamslwzvl.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gultgjavx.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gdhydarvb.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/ggbumezaz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/grafqggeb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/glghkjozg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gymxcmfre.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gsnrwehgy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gxoqlnzoo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gqvqffrrk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gbunakoxx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gptavcqqz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gvyylsuey.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/giormxvzj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/ghcyiugyw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gzktyhude.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gncfegitm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gckugreeq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.zdbjq.cn/Article/details/gkhvugwki.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/godlkusbv.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gfhoafcpo.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gybojzbbx.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gfbfttjcy.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gayquaugp.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/gmvjainuz.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gisbzrtaj.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gyyyksktf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gkhjjttbv.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gypviuowj.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gusckuxfe.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fehbvm.com/Article/details/gxqofmwja.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gljpmecmy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/gzqhbczar.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/giittpbho.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/gsgnzbffp.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gjapefgay.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxgoowjlf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gtqrwyjca.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gwiokfxow.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfuhmxsbb.sHtML


<!-- 参考信息 -->