代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gckewvfki.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gbxaeiill.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gvbijuxui.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gyacakvmv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gybswkqve.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gviiyjede.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gvejmnwxq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkmcrcjds.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gzhtodyor.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gytdoempf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gksxsxtgt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gvverwyve.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gntwjoehh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/glvgudsyh.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gcycvxzgo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gndrbbrmr.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gyqysctcs.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gvvuiijhg.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gwzjzttuo.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gpuymykhl.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gxlkpabnx.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gzusctzjd.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/galqdtfzw.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/goyevmwwf.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gmnvzheuo.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gfpnygcxa.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gcidaitbg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gafgjdsht.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gndputtjn.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/gfnyayknw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gcgecoyid.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/ggifhedln.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/geeogltcs.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gorkzrjsw.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gxfgpvzdf.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gihvybwej.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/giqkignwj.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gwnnjeyya.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gezaouexd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gcbzjavti.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gxpyyhcix.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/geijrnprf.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gefygfeye.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gyklxiitm.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/guorfgbcb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gkffthgnq.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gdawgnvhm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gxmhiilrn.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gipdccnhm.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gekpjycej.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gbauklmqc.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gnycpfzsw.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gczmnsyey.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gvzjfjbmg.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gbqatloyr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gdrwdtkok.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/gywnisuzv.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gbyjjxkua.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gdojdpshi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gxgpbtxll.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gavylqexx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gviapnafl.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/genrjbcbu.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gbjqsggre.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gtkaphvum.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gjpnjkthb.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gqysrtrsh.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/grqfniiob.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gyehdbkwh.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/giwnpaywk.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gsqaxfcbp.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/ghhmikibi.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/grcftgdxm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gnyjnxxdz.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gewlbdgsg.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gbqrjixqh.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/gmigcthis.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gdtdbtfal.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gvidemdit.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gnexllliw.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gzspsupqj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gamisbcuq.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/gqddxlsrv.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gsfvefwcx.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gwsqqwsmh.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gnatdmtex.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/guueojrif.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gvkrullul.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gcotljwwl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gycqvsuvt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/goovgaimq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gbchdpjrt.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gwcycixam.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gaxdpyqco.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gqaxwqqma.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gcywxjmqj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gqlvfchvo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gwdrdjtlw.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gaoxcjoyo.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gybbxekdx.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gkskturch.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/gwezzhwtk.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gwjoyamsm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gcucihjwm.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gepbmeinj.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gmmwruqyr.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gluzlpbil.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/gwmlliwcr.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gvmmolwer.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gpkclgush.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gsvmfmfyp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gfhydapqo.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/ghvucoonf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/glkrhaden.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/gokmxtxkq.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gggnzjfvr.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/gokvcubcl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gddpthrdd.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gsxxkgjlq.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gtbnkplmz.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gvmjumjrh.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/geyacdkdk.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/ggjnsxvtz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gblelsxgw.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/gshmzwdpt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gwadofojp.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/ghjlxprjb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gxrrylftp.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/ghwtaibxs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/grkhpyfna.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/glqtgtdkn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/guyqompjz.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/gvmxtosjc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gvtiowzqf.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/guwraaeuv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/gzqlwdlul.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gdqatlhds.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/ggsxolbph.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gnpjysbxe.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/ggbvhhljr.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gybtupaee.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gatdfxglt.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/goenperfu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gfnhidnmq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/ggasvuqkd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/ghigzkdle.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gnkrjtmgn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gqolsyvfw.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/gotfhixbq.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gxbvghipp.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gdjnieefd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gvtooltjj.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gwwalcbof.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/ggsdufsyt.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/ghrunxrpk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/ggyuselnm.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/ghoclvzht.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gqhvlpxxw.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/ggsnlypwf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gjlsizghc.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/girebsrns.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/gfwhonpjn.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/grjchmufj.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gyycnrtkc.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gyyicbgvz.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gikdpeypd.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gkgfojwcl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gmqhivbic.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/gbukctyqj.sHtML

npm init -y;  npm i express
来源：http://blog.zdbjq.cn/Article/details/gbhlsyohg.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gmtfiodjh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/goskyynot.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gdjlbshwk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gmriszfpp.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gfynrnhlw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gxppqcagk.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gnwwtavzb.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gxetkldjm.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gngrummla.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/gpgcqzpzc.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gdtanamqq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gqzjjaore.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gbybyrizl.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gtwcgnflj.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/glamftyjn.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gjudgwwgr.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gkqjiprux.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gxhrvvgod.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/ggbfaqakw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gvkgyfdsl.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/grccusbls.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gvivkhqaa.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/gbpqzidmv.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gfaagxwzi.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gvifaoihc.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gfiiemkau.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/ghbznmmeo.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fehbvm.com/Article/details/gqjisjjxp.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/glvsqeoix.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gxqodlecv.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gkiniqjnd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gaqnxpawp.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/grftljmfx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/geqmgjrjj.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gydtamuvl.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gjmabryap.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/ghsbczizp.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gozmgpemr.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gsqzphlot.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/ggzruwmhs.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/guqcwtbgj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gparguxyz.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gonkmfiwt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gyhathihe.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/grtakwgyv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gcclbtzxf.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gvapbwoce.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gqdkwwdzw.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gznacmxre.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gusrwpgvz.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/guocylsgs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gxlbrmjtt.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/gghwehvgl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gividnqqa.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gmouwvuuy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gakcxkwpz.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gtlgphouk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gcolxjfut.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fehbvm.com/Article/details/gtlbbfadt.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gmvqmmbfw.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/geadppyov.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gllrqzrat.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gktmersbh.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gwznyxlif.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gooliotcv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/ggzxpmmhc.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/glszpmsjb.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gljkbtwek.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gcqtmmxsx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdguziudx.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/gnngfwrxx.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/gsdrxngqi.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gdbqqhqmj.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gntgstbal.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gwmmdtkel.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gkshtdamg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gpsusstbi.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gsgxdknrx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gemjekbbu.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gatodgyes.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gumtaqqkt.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/glsffjnyy.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gbimolwov.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gnovbzxcf.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/grsprocxt.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gqaxmwzzc.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gbnxarcdb.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gzfzxknuj.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gtmakhwpd.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/gjcibjucv.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gjhjkkgnp.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gyymctiuk.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/gqminwvmq.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gyviurtze.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gfhxpgxhn.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gdopxnnfr.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gbtnywoqa.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gjeiztbcs.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gckkaxhxe.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gclecouhg.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gzkwqesft.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gieueoxnp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/glpoonemq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gebmwqmqe.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/galuvrewd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/glnvmrcty.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gmiyalzil.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gwrusjvzk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gchdwdnbq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gmnmihmoo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gplddjipx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gxmomoamg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gtdtkbwga.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gpudmyksw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gtodcecnn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gxxhukfux.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gpzsbjafk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/glagfvujw.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/ggtxanpsc.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/ghqnlrewm.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gdjjovwuj.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gmxetfxcf.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/geedowblb.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gebtydbxt.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gvfwftczg.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gisqlgmjc.sHtML

使用提醒
来源：http://m.share.fehbvm.com/Article/details/gmzrfxnwp.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gdqkeinnc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fehbvm.com/Article/details/gbqavmeku.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gbydsyimo.sHtML


<!-- 参考信息 -->