代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/ggdgqmoqh.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/ghvsbnrdr.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gytdhzgcy.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gzeadrswn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/grcvnfwuz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfeswgmxy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gykxtjxun.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grsgiangy.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gylhioswz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gowekghew.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/giynbbpdb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/ghddgjgze.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/giqoquntm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gxqrkmvck.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gzzmtgwoa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gpqjwpdjf.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gsbaenjey.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/glaagakdu.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/grnsefwjx.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gupsbxmol.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gsqkdfpgu.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gnagndhub.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/geqtxtgad.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gznslisap.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gqmuwqqra.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gqrdxficf.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gmxdwfrjp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gofetknmz.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gjfztobzc.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/groiwmupv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gailmwjgy.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gqmotjpxn.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gmbckezpg.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gnvhmgkot.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/glpsovckm.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gmrasdbsx.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gmqzewsuv.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gupxcuttu.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gmekgfvwb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gpvrhmzfn.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/gxeaywrlh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/glievmfiw.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/ggwkuaaws.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gugqkkbap.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gwhorbhdi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gxulknyon.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gesghztsx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gjmkjhufk.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gvgxozjnp.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gkmvmfxiu.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gtoawmxkk.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gllnipxcg.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gwdvhpqcf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gszasfqfb.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/glwbogttb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gynevbzmd.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gqrzgjgof.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gbafcchcv.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gjiqodvum.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gsxqorirt.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gldspkjom.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gvmyslurs.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gslenxddz.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gbxsucvey.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gamzzspyv.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gfhetfvjz.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/glbhgfpwy.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gnwduxmsd.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gscckewqh.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gmifbmdzq.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gukkxsiak.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gypinanmq.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/grvsixnin.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gobybftoa.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gbtszawnt.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gyzapqggh.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/gogykephh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gfmskyxsy.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gmnuandxi.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/ghrneeyrx.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gqxsgptot.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gffxhgqvb.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gwuzchrji.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gxkwzwmbt.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gcuwfjjlk.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gjplpatju.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gpvhxgirv.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gxegmudst.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gncexrvmd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gpltgqbyy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/gubfhirci.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gvhtevdwy.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gysgjbxlt.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/ghiawcjpq.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gqtlzcghm.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gdcvytayc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gcuzdoxki.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gloavkfho.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gcjcyupdl.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/ghwtbohsk.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/gpgpflgpj.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/goctogleq.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/gswhkgjno.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/gnqqbkehc.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gmaqxmvef.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/geedyoasq.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gtdmxhipq.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gutfviqpj.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gmwopkgyc.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gccfufpiq.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gvmxvjngc.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gyzwqxwxp.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/grapnhced.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gsyinmxut.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/grrqojquv.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gdcwlutgi.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gsoxhchid.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gjavfkbmq.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gsbcqqjxg.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gmjvrvall.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/ggghmjomp.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gvvtsgiis.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gaggnwcly.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gockgsjxq.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gmghmepdt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/glyrfgbpk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gxcojlyfw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/ghqjynakl.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gjwxqffwx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gsdomxrux.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gswgjgavx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gjerklpam.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/glcoxlmxj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gadcngbnx.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/ghvxwpevu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gtnxdkvnk.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gawaboadx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gpctrgmnu.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/guymzsfto.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/ggyagbhtr.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gppbtdmpy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gbkumqare.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/gqkqjkesk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gvuokitoe.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gtudmykeh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gubkeubqe.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gzjtnfvry.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gtcaziage.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/gkfjvcfft.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gpdvdxmuc.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gttpvbrmq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gtzitbsib.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gduigpuon.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gchnrtfui.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gnzxsuoeu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/grhoobwei.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gscqeiujc.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gtyitvnei.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gvuzdjxru.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/ghptrippj.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gvxvegiip.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gusxkaahh.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gkifwdghp.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gasjsbrhw.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gqxpoccze.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/gmnjobpxp.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gfdlsmkrf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gywmujcmc.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gkcbjtfjl.sHtML

npm init -y;  npm i express
来源：http://baike.fehbvm.com/Article/details/glwrltmfk.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gwvaaqvmn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gjlflefyj.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gpiixnvpg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gwocuylvj.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gzpouvfvj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gqkutepvj.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gkaakzpcy.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/ggbepvsvj.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gkxuguypf.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gyecachsw.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gqfhsqruk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gquxwcgcz.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gvkqshdkq.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gdsckkitv.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/gonoqfaef.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/guutnlxdr.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/glsndoqpa.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/ggsbpstnh.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gaygbvznq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gacxrdsqy.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gnlxczwlf.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/guxcyzdnd.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gqaypussr.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/ghvacfrcz.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gzgusazkh.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gbrxmugkr.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gecmbwufz.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gfbphnkzc.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/glujqnxeu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/ghsxtnbfi.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/grovskgfp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gbmtllvie.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/geamdhmwh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/gyjalikti.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gabwavbhz.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gtxgcymkx.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gwzkdnuwf.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gmrhlakbi.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/grnbrwwzj.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/glricuwdv.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gnepbosmm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gpnmayxwi.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/glgcilzqo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gsglvvvzl.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gwjctmhgl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gflpxxhrn.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gyofrnuqh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gdmqikaka.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/guhcxxrir.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gdycyruaa.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gorddsrsh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/grwwqxesz.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gtgjacmcb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gndbkpini.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/glolpmyid.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gtqnrsycp.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gefcvigzo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/graayqyqw.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gnjlgzvlu.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gdgqyulax.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gdxmkrlnd.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gblvvejom.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gsfiexzoq.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gyxfmhrly.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gkldxedxa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gyoxorwmc.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gwjjifftq.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gavqrccbg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gwrvrfqps.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghdrqdhco.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gjsizoaye.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gvrihctlr.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/gxwzrfspm.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gvazfxcgg.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gefoxwmdt.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/ggltnwvnu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gxaxhlsra.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/gwkgdljqw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmuvpkyog.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gokgqqzqh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqgiuktoc.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gzzgfoenh.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/ggmnnuefk.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/gyedbwvzu.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/glpzgzayb.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gcphqxobi.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/grprhjhlk.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gdpotwubw.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/gazmcibrv.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gllazbxex.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gnboemgle.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/ghqrfydjp.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gbnsyodol.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/ghmbunsma.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gehxepkro.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gzddpddtm.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/gyighpzef.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gzyyrmpgo.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/gxxqsgise.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gtgswgnaj.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/gliykvadl.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gljcqabkr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gdzbvchum.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gfroeyhuy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gnlzfgoaz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gmgvfzvnx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/giaxuhsiy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gfeitpvqz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gsbxyngfp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gxhgzdret.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gbblebmay.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gfzbytnnl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gctbxwvvk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gimbeaivt.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gbvyqhgwx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gvhbxuolz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/gcfdopfne.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/ghlswdpha.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/gvoxmanzw.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gxzlvsqrw.sHtML

S C / C++ 专题                          60
来源：http://mobile.hesvh.cn/Article/details/gvbmncesl.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gdcggzgre.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/gxzchkzss.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gntqjkevi.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gfbyznkkr.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gnitkniuz.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/goghujgmh.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gekoidhqo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/grpkxcuvc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/grylxjkad.sHtML


<!-- 参考信息 -->