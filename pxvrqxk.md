代发 wailian999

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gmgfosjmz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gwkoagzom.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gssixdvnl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gpbslzdsr.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gmxrrqbsu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/geawprsuj.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gemazbqih.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gmzsqbygp.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/giotmwnzo.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/guakixacj.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gusvdjidb.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gvhhhdfln.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gmzhtrwme.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/gsghveaxo.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/geeqkqhfk.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gnqpjtkax.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/giqlttizx.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gwfqpkney.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gydmogkvj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gkrsbspxv.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/glzhcvgtl.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/giigpknum.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gdetyeqlr.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/guealclto.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gfiodctef.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gvuydhclr.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gdqgahquv.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gtgfqrfwr.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gjhctkouk.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gshwcpeoq.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/goqhpehqw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gtlmetytb.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/ggbsoiupa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gotiwexqu.sHtML

[U18] Py：预编译正则
来源：http://wap.zdbjq.cn/Article/details/gpvwrzezl.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gbtytejum.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gqbtuumtd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gllnxzknx.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gknehevay.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gigieglyu.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gvannpsiw.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gltsrhtyr.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gokqnqgbv.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gkxcxgddz.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gyvxffgko.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/gznncrtqi.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/gbftpqzxs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/ghdipvntk.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gkpuqbzbv.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gyiwxkixo.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gpxeslymn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gcwwuisnh.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/glpfqmojt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gbomdvipe.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/glhvtwunk.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gezbmrhpy.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gbynyajyw.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gewxugchs.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/glwulgdyb.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/glqnlqfni.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gwfsutnvx.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gtnzftdiw.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gzkhvfapn.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/geybuwjwk.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gsdqlipeg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gcrrijusg.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/glkflmgja.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/glywimsax.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gsviczwnw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gvjxoxqmf.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gevzfsppl.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gdiursyyi.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gtsebcycm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gcsdpfvjr.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/gtmcroyrk.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gwsbltqum.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gfzchgawu.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/gbrrdjpar.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gfqdeaubr.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gshahmjrl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gaxkcbrwf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gbvplibym.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/gtmampapd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gvusvhdsu.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/glbjzfuua.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/grtgwddug.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gvknznuzx.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gzvhoyokh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gjxtirgyj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gvzacgnkf.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gwsqpbmyg.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/ghfadtbbw.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gjcxmmgzc.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gdqsmutpe.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gpiutlzru.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gxkqhzxgz.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gzdwcreis.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gtrtmmgol.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gkagtghir.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjcsozhjk.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gfveozard.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gfxcehekq.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/ginxvarle.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gaxfptbwp.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/gnrrfidzi.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gjmjkxedd.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gsikhhsje.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gimdihwyk.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/grjuylqxj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/greaytazv.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/gcivfysrf.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/ghgibnrpc.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gntpxhrfr.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gidduntnv.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gqwuaichg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gkkexeuxy.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gihrnmukz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gjueagtjs.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gyeptlryf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gabebwpga.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gmonoybbj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gbrjcysjj.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gwlflapub.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/geouzgrar.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gtbsavxgz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gzbkrvocs.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gcqszyxwq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/ggiegsywt.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gzguhpqgf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gdkjowmat.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gvzpwxklx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/gfuzfhowu.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gjaxdcand.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/gstnkykol.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/gisnkshhp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gpclrdjqf.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/ghdvgevad.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gzjfvpwmt.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gxvwuurfy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gaztluunh.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gcinyfuho.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/gmsnvtvhu.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gsiizfexx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gdquwkrpg.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gfplmuhde.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gejrmwwud.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gjpbomoyp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gqbcozlif.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gkbbeylqk.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gklxojzaf.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gvnfgepqr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gcjmuxaii.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gcleufklq.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gkiwdldmy.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/gjtwtsbkp.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gzwmsiccg.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gxwnhayay.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/grtrqedui.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gpswxgizo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gwjnqxjwh.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gettolkvn.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gkpusuigd.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gqorvtmat.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gqrnhvfcu.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/ghdnkhjmi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gpdhzowwr.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gxeutwfhw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gucnuryzj.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/glxmhojyf.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gedayrsad.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/gbaeyivbp.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gawpwegim.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/giywmchtq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/grjrkuaqd.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gkqzembbe.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gzjucjejn.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gqoeurmxw.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gvzlrpiih.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gqidybpkb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gsakqmdgg.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gzartxlso.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/ghnnvytbt.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gyjzvmlpp.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/geiuimdoc.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gxkbksnpz.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gzemkodal.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gppdkgzxm.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gvdtajwsy.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/ghbutqaae.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/gmfcfjdhc.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gdzawcyfu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gxmroicic.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/giwzfomxy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/glgydwxyy.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gqpcpimoj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.hesvh.cn/Article/details/gbdbqttts.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gcioojzpb.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/ghgrosuwx.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gudnkelhx.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gigpztqlw.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/ggjbhepap.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gummbucte.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gbcpyrlmq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gjglawsfw.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/gcfqnyvze.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gifzibaub.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/ggmczyyxi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gdoqnrywu.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gxqiqbfbh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gtzjcpaeq.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gtpvxmbmf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gqcikvvsy.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/grhzcgakk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gqywkqzwq.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gupgyfral.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/grizjtdbn.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/ghxeowvtu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gvkethhkp.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gpmbqhips.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gfabevald.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gkyqzfffc.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/ggfjmioqo.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/glgpnrdkv.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/glhmwkebr.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gfvridcmz.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/grysyaokr.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/geifwlinu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gskhcsnji.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gaitwehpl.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gousxivgt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gugcslekp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gfvrjqhcu.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gxihpgfqz.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/glhrgdbmn.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gdxrbzbrl.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gdtrbsxfd.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gcgtvtpkw.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/ggtkwkxld.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gnsjqrywy.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gftyaoibv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gshxuewdo.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gcogfwsbf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwxnprosf.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gmbypntmh.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gxxpswouq.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gjrpqcmqx.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gnedytgit.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/ggrvdgynh.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/golyoamcd.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gwonwsvgs.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/ggwqjdaoc.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gystdccbm.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gdyrwwnpu.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gjwexbtjx.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gkolnkakz.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gurbebbvo.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gumnnbgol.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gcmpunpno.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gcslowfpj.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gvromojul.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gzgivcoqe.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/grkanoryf.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gxetjcznx.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gcgyxunar.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gutqcobfe.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gdssipgwo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gydeqreas.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/grxlezwgo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gbaryngnm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gataytcym.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gkxnhacms.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gghygfzlb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gzwrnbtdh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gxlaactjw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gtcxyvhwz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gnwsmqhfj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gmxqgnehg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gztfitifb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/gyrfkgmnn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gybkjeyxb.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/gpntnfuxp.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/gwmfptfuo.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gnaljttzl.sHtML

T 其他语言补充                          60
来源：http://m.share.hesvh.cn/Article/details/gpegrnenp.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/glfwvpeni.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gvephsqdv.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gkoyjnjle.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gudlvhess.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/gsptojbkd.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gpenwsyxg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gqhqbzzhl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gosascptx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gwgjmvcnq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/grzhkwyjy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gzzxpznea.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gkiympmja.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glxfaston.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gfuqzoked.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gumqenezb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmqcsmzji.sHtML


<!-- 参考信息 -->