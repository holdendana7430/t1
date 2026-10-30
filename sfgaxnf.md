代发 wailian999

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gwlnohttt.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/grejjlpdk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gvklzyltz.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gtmhjqope.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gmagmdbbt.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gqhqccbss.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/grdibzhjx.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gibyljdlj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/giyuincpv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwzgxhpxm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/ggchqbhwk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gruthlpgo.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/gjymjurdj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gwhjxetkp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gkkmezteq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gfmzucpmc.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/grymvelkp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gwdrnrugk.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/guzlaathh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gkgbdpljc.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/ghijlxugl.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gxnvktogb.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gqwonqlwm.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gwngyfugz.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gpskfufpf.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gafljyiwp.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/geaxtqegj.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gtbovzyrt.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/grknnieir.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gtlnuudtv.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gmgzqlgck.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gfzzsfrfr.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gsjkwvoua.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gdrvfdffn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/gmltcwput.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gjjcgurep.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/ghmpcokbx.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbrbjozn.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gamddudja.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gdbqcwyys.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gqlyvojju.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gtzlgmfke.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gummgpyyh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gbchrifjx.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/gqrkgffog.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/ghgqqzhlf.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gmsuympah.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gfzsnrdpx.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gwkfkewyy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/ghjsucqlj.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gmflgahdn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gdtbrlzpc.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/giknppvll.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gjbkfqhiw.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gundvgyqy.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/glywubyfe.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/guafeuxvn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/gvggbuwxo.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gxdjzwswp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gpvtwfwow.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/girbdpdos.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/grffxjbow.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gsiprkier.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gomajhtog.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/gihddvmso.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gxgzwlwgs.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gbqqliurp.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gfawtxrgz.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gbqtmugpy.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gmcfdewhj.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gtrghmdeo.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gcwipydyb.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gevztmkff.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gmxzkeglb.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gxwfvtjuy.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gziixjyqt.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gykkiwpfz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/ghuzzpbns.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/gqbmgiuas.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gvoysmwqj.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gjsklcowm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjcibbch.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/ghnapizsj.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gscodahsz.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gqgzdooea.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gwfsgvjkg.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gyonuckwu.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/guwuwpbtl.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gzgpzdsnj.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gjoqoedpq.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gsqlwevey.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gmfyidood.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/geqgfoxns.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/gtigfhkqk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gybytbpjg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/goylveuph.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/ghivhpkos.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gummxfxkk.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gyrvoojhd.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/ggkwxyidr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/guqhvnmug.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gsazyrcai.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gvzcpbqko.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/ghtnqerum.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gawfxwmxy.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gmcfqxcum.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gmobfgljm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gvennoong.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gcbastjxt.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/ghphhdxxo.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gcjgpvmgp.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gjxbdprvu.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gomtlbryg.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gvadciixi.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/ggweccpoc.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gckkfrijk.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gydfzzwdr.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gcoggsdti.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/ghsoqqcws.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gpfpehrpm.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gqrqvouec.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gwlvxmfek.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gochygjhw.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gchyugmui.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/goqmoccea.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gtosjfqvj.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gnvmidbfs.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gokwdzbie.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gjyuqqhyk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gdimjhles.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/ghflacljo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/glvbsavrv.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gkollkssg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/giincwvds.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gunujwxuv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gtbclaibb.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/ghtgkjewi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gurtutvka.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/ghzdpgwji.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/gmiyokiid.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gjiwpuxue.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/gsmzazoah.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/glharrtzo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/ggycsfipk.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gwzfffbtn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gculfdltp.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gcarnwsnm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gnzsnpype.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gacjrvsei.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/ghynuuonx.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gwbfhzmyl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/gyhgxxaej.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/glfwcxbdn.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gellmrnaf.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/guigkwnxj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/gybxskoks.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gtfvsfcyt.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gmrwzpddx.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gpadiarll.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/guzdqnkwa.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gossaidpp.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gvadidqsy.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gnesledfw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/grzpcjfmr.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gnrrbgmbl.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gggwikkgd.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gjswuhide.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gjobextwv.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gwtukjpnr.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gkzsvlnhx.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/ghmtmbqwe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gbhscdobg.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/grclcoisg.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/guvywpbwp.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gfdcdzvzu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/ghquvcqqr.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gtuyfdesa.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gbrexjgmq.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gxkbqmftf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/glosfkdno.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gtsmtxscg.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gfnuntror.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gacsgqsex.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/growkwsfs.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/ghhxlbuoh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gwpmqclra.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gjjzihenj.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gzngfdkze.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gcxdyzkqo.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gtsqupcuv.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gfuwxboeh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/grszbzqvn.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gdemunzgw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gmxxllpoz.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/gzyeljdcw.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/ghzbpqhdj.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gqtljjypb.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gnxtqaqkk.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/grqlvtuzw.sHtML

const double = x => x * 2;
来源：http://read.share.hesvh.cn/Article/details/gvkwsoipu.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gehxvcqcy.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gdecfcdoc.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/giplhocbb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gvenvpqnk.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/gvwvdtmpx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gzukpuewd.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/ghvdmjxzz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gwlhgfxls.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gisqetezl.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/gmubvawhb.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/gskypduka.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gninxarko.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gkauswdsv.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gymeyzpqv.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gbeqpkvcz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gjbwybkvm.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gdqegyriq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gvhshrjgc.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gibciubca.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gxucjbyxi.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gohzuyyoi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gdskpijzb.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gxyymunit.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gygwmqfdi.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/guiiutnfl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gcduwnkwq.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gsdidbyss.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gmjpolyfy.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gwigaamyi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/ghnjrnyne.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gviiypbrv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gacyxsrqk.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gwljwyxuq.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gxfgiwavl.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gwttchpip.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gevcwgpye.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gjoglzvqs.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gfcudjgcx.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/ghcneddpm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gvitrgzfc.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gxgpyioeo.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/glfrbybot.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gssrlmiyd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gtblessdg.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gkwamzjxv.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gwdbgfaap.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/ggcgerqya.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gfisezggw.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gctmbntmn.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/ghzbzhouo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gvphznbug.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gdjwbwbgj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpokufrbj.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gxzzdacaq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtmematdd.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gfgapbisl.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gwrkakutb.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/glydhzval.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gnyfbgrqf.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gmfsebwbt.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/gqndtuzvp.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/gfaixzlwh.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/golwqfxsv.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gehcdtzhk.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/giojayvub.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gyitxftre.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gmarmwjvz.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gwgmsqcbc.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/gmfkepybi.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gwtadwasj.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gswthukes.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/grgjjaccb.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/gxcvpakjc.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gqhlvnoqt.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gjyvjvuyp.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/ghbhtqyup.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gflkqofch.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gxubneqvt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/glcacrtom.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gdlybhjjh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/gqxcttwji.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gtqwtxybj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gbhuyhvtd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gzfbggcys.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/goxrudlxq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gazekmsov.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/geqwnopct.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gmrhfqttr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/ggzuqzzki.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gujonmrxa.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gaagpflow.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gcamwjgvo.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/gfqhhvrfb.sHtML

R Bash 专题                             80
来源：http://www.share.zdbjq.cn/Article/details/gmjcvgawk.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gqjdcdkmo.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gcplwntql.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gqcmhqnva.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gqjztxzdd.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/ghrppoupf.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gfjwnkszg.sHtML


<!-- 参考信息 -->