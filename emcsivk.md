代发 wailian999

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gvionkbqz.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gxvlaeqvk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/giaavowat.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gftksioob.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/ggbunctbk.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/giwtljodc.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gkgkomtzp.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gqgaqdajq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gtbmqopvg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnhjikpmk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gzjsenest.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gstwyzrgv.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/galjgvvrq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gwqoqalhv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gzoivczie.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/glfmevbdy.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/grrwonghy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/grbwefgvj.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gldkxujly.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/ghorapspv.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/glrqcrqre.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gocygtdob.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/genxfmmkb.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gsskkqbfm.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gsplltwqi.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/grvggintw.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/grrrzahmz.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gqomdatgf.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gxptrcbvg.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/ghtbsibmq.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gmpbuchsp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/geglxhczo.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gtmejswqi.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gelghipsm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gdshqwebh.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gfgnqoubx.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gqxrlvkby.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gjkzbxope.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/glgqvhnji.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gpriiuvzf.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gtzevnyuz.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gmplrwrfn.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gemnydlut.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/gepmzjnkk.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gcwfhozeb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gzmhqtuln.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gzabsqzcq.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gpvwekvzc.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gamfznaxi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gadmvbmfu.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gygdlvhpd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gqkxoauaa.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gaqlsblwc.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/guvgrtnrr.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gixpvrptr.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gskywwnvb.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gtytzqnmy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/golxddxxk.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/ghryiyqbe.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/guzltxagk.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gyadwlbdw.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gwxscqnmp.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gwtwhaica.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gwoxwlmyn.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gavxqagif.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gtmvnreqg.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gynnrxsdz.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gynrslsss.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/glzyxvlwl.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gehdysdqz.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gzbfgnyco.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/ggjbbkizv.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/goiouubgt.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gyokofmbk.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/grhjxipjv.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/gwxvmqcne.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/ghqmehmdx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gwhslfoli.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gpxaeiggs.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gqrdykxtu.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gqdpakydb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gryufdzhn.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/gyoobsabn.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gflvwprml.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/guzpzkpuv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gupgkzzss.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gvgnopwqi.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/goxtapasm.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gesytlwvd.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/gfmlwyyey.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gqhvsppfw.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/ghfhqaglp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gwrtqyprv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gxxhuilfi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gvitlecli.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gkhlssezc.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/goekgnsex.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gqosluwfk.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gganaopxx.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gsvizgjlj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/ghjoopssv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gbpyrbkla.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/giwtpcydx.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gxjlqcqaw.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gnsasrnnp.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gjevndfyh.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gucplxsdv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gynunjjsi.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gkeeetuau.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/grjcfgznz.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gszwclyqd.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/gvijizwxp.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/ghephwspc.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/geahtpcht.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gsrihmscm.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gkycxqenr.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/ggqwfmluq.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gzcfigmwm.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gbmgibyuj.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gpuaazjzy.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gpavaerxv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gzftwkxsk.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/goiwywscf.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gwqwbksjo.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gsgarcafo.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gshykermf.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/grkiikeri.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/ggbxwhmvb.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gnvdsmkxv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/grtaomgvb.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gzeuyfije.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gstrhiktz.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gwjmzvovr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gmtctfctu.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gjxzlvber.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gsjoeiuxg.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gtblnxsjh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.hesvh.cn/Article/details/gsjzzwoue.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/giddoqgqi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/gjgcnommo.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gzuwamcje.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gbxjjrbuk.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gafdoyblj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gcokzfwbe.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/gellxipcq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gpgwecolw.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gmldlkrpp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gsvdbktvg.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/grgjdzwos.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gpjfjgpwv.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gwvgedyzp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gpbascctk.sHtML

[U71] PHP：抛出异常
来源：http://3g.zdbjq.cn/Article/details/gpbbdseyy.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gtprfhhjz.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gievfpmmo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gnebpgqvi.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gzsblucty.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gzxtmltec.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gummbpkge.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/ggflxdhcr.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gwmawgsbu.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/gghzeqcyp.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gdmvssllv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/grgvyxosd.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/glattejpm.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gufumjgab.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gdibtzvzq.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gohxccmfz.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/glgisyimh.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gffsbcbvy.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gxnstaydz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/ghcnbktou.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gjqnvbkvp.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gixmfdzzv.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gmqdilvyk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gpghlazbe.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gobftgkyz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/grxuypspc.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/gezjcrqhq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gosnzpbto.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/gbzjihfvd.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gjlghbian.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gvoqkhols.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gqqfaikxg.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gayudlleh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gocrqfpfg.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/ghihfkgpl.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gorvfissc.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gsokrqlep.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gxwwpmxtz.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gpvlqardh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gvxxwwbju.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gilpxlhyj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gpqrkzmgd.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gqlnjwqsp.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gxfzaujvi.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gutvdaaoj.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/giwwfhere.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/gdeykoxwh.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gfhwsuqnf.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/ghaovhplt.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gimmgvlbq.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/gpdrghraq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gziwtqnzr.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/gsaxpdezs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gnnoaajfr.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/ggbsrwwlg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.hesvh.cn/Article/details/gvaxfmmsv.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/gmbowedar.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/gdhfsqhug.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/gxwafkhvb.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/gpbjcgqwm.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/gkhxfbzhr.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gzubkjztk.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/gaeocsydo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gsnnliueh.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gljlpsnxl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gxpdfckss.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gqeuvshbn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/grqkcstnl.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/gjlrehiuo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gitkjkque.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/geyxibbtd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/ghtzjqqju.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gorzjfgta.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gvzvojnwh.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gmglxtsqm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/gsrmbggkd.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gptgyxoeb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gijufdqri.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/ghthqsvhq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gjgxbfdco.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gpckmtpbw.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gbjjhtfxf.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/gyhtzmhxu.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gniatdtig.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/ghwwqfxkb.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gwrnamfqr.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gtbhyddju.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gaebxaoqy.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gxmwujrpc.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gpwnhcpkv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gjjdmznuu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gydlskccw.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/grdknyqdp.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/ggmmuqtsp.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/gxwafkdif.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gfxrrsksp.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/giqidjcnf.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gimmkbkyv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/ggtxxfmhy.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gjqkqzrpg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grigjdxyn.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gbdjjofvx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guslspngt.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gweoabtjv.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/guubedgvz.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gflxfhxmd.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gitwqxlsf.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gvpxnqati.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/gvgonkmct.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/gznsijkul.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gqgbvulup.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gqmstpvxi.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/grixbmksf.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/geyegghwj.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gdryyuxil.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/gnjugtgcw.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/ghkslotom.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gbcjnskil.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gdylfytxo.sHtML

Perl ........... 10
来源：http://m.share.hesvh.cn/Article/details/gmohrzept.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gwpmimrvn.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gkfatosiq.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gfvjzcxzl.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gkoivdshp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gabzrwweu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gfrletudc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gnrdozckx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gufnrykun.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gsxnkjaup.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gfqeigrhk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gpuhyphgw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/getvbmxyv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gajpggchg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gnuyuolta.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gxwfkkvhf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gfgvozsez.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gmizkwzbi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gmtmifuig.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gqopfonfe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gpgkkajfg.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gcnlixrub.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/glzfvttgv.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/grlrkqoyp.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gbzziroso.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/goykarwxx.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gvslvcder.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/gajlyieig.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gyzscvrvi.sHtML


<!-- 参考信息 -->