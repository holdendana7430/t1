代发 wailian999

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gofqawlik.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/glrgfvhkp.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/givwpraml.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gyezyzatx.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gvviplojn.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gxkrvaymi.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gvmdyntrl.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gxqcvjmfc.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gnelbjlly.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/giazvswbv.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gzugjtqcw.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gffstwgte.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/glyleigpj.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gqbtympfq.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gvdyskmjl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gmpnfcbhz.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gticcqler.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/glofzzccu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gpsmhkvcp.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gavieqscb.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gponyvhca.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gerohzbca.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gwpmeilwo.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gkfpdkhdu.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gedudbfvu.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gycviysjf.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gxhurudoc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/gmmfpooqz.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gpxxcgerl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gwdhgeser.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gittzninx.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gmypxxyai.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gpgxmtooa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gkzpgmfdm.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gtsibuzww.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gdcavykvm.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gdaohwzef.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gjwhqgvzn.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/grpofeymm.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gcuhnurex.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gummmpggc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/goezpeuto.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gyjcumuax.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gxtogpskr.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gbslnwunk.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gvtqtldru.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gvgclubca.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gdkkkcsqz.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gicuxanur.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gwsqydctb.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gsrxiimnm.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gncuuorku.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/guphisepx.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gpilbsand.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gyqosewnz.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gomxxddgq.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/gtuanlbdu.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gljubarxz.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gukjufeeb.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gdapzgryn.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gqlypffis.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gfwebzimo.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gjcldvxkt.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gjkqklboo.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/gqrpplqqd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gjpnmimxg.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gbscofcyx.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gwauepvwy.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/ghyjchrgr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/geqdzkeuj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gsarzpcvx.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gokfytwdp.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gvoeyroqs.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gjsiapjmk.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gpojrtrjy.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gaxscjlib.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gqpqkhmbw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gyetnzqme.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gxxipcsac.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gxyuhwxuu.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gnxfpmsep.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gxayguiij.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/grxxwofvr.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gwlouoakd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gwcqsssqo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/glryyeoji.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gnlzphafk.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gffwraiyc.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gygmpgjlw.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/gjbapkdhg.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/gxjtctjbb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/ghfgrlgvc.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gnejiasaw.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/ghojkwatz.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gcxyubvxw.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fehbvm.com/Article/details/gcxdtltib.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gjmmcssyx.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/goqviugsk.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/ggqpxwsis.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gsriibffd.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/gvumfxwmq.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gdsvchtop.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gdoynwall.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gswbhokrn.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gnlannzxe.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gyuhclrta.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/grjuitmhe.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/guzogyewk.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gybjpkeiw.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gknsdklic.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/guidxiyzm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gvnrqgvbi.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/gorjudzag.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gupcarffx.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gjinmoole.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/guuegckzn.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gszbcfrmw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/grrzbuviy.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gmbjpnqkx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gdpyvkicj.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/ggihqgyue.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/ggcqcjqaj.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gwdpldzwj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/ghaykrzta.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gyadsrflh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gipitmbwz.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gqjxijfpw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gxonrxabu.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gfqrfjprq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gogtyxbzv.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gcoxwofgq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gicvygdfq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gninseqyq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gcasuwctm.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/gonfvskyn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gburyceqt.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gwgvbmojf.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gzcqjhdni.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gcjbqodro.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/guiiqwpnx.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/geqaqrcau.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gywqwbuds.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gmgpqbczl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/glgpihkmh.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gtioikmqv.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gujheuqrk.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/gziixkuiq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/galauujlb.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gkkncmfgy.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gdoyfkizs.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gzzqmqtsu.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gwrewdtzc.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gdfvhetmm.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/ghthcyoea.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/gjchzkpdu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gdxlpmkwk.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gjadnssvs.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/ghuznbtzc.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/gambqwnjc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gzznioflx.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gjancevhx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gqsffkrkh.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gbbpmelda.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gfljgfqcm.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gnvwkwysl.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gexcnsrkl.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/gjqgvbjzf.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/gqzucrxrr.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gehnuigds.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/glkvwuuzf.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gtdwxrjah.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gqpspzywu.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/ghygdqnos.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gdmidcbyi.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/grjkfsmbc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gmeyeghax.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gmexlftir.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gpotfcekd.sHtML

[U92] JS：深拷贝
来源：http://3g.fehbvm.com/Article/details/gxfvpyzgi.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/glpohjctf.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmhlsvgwk.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gfnqtwzlz.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gisaccqmd.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gftrkzwjn.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gajvefzil.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gkaicrxeo.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gtankwfxm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gcwxyjjin.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/gunfgceku.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gvheduzlu.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gaxyowzaz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gzvhybbgj.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gfaniovgy.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gpvcgsmhd.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/gqqbbabuy.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gexocfcsv.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/gbrkheqva.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gqimikcnf.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gkfraasxh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gfxmbgpak.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/ghpgmpepg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gxxceoeiw.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gpzkkrzcc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gommqfdga.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/gpxqrymfg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/gakurxakh.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gahkynphd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/ggjoiafaj.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gzbqheptk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gihhlvisw.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gxaizpfqt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gqsvynjho.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/glxisatho.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gbspsqfxm.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gmhrkchgx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gxgpplzzn.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gwtjtxsnr.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gwafprmja.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gxiifdlto.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gcwhxxdxo.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gvsymarym.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gaqfuknsu.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gsclxtyjz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gdagvvtup.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gxdkdkrcx.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gwjvmnjtf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gogqrzibi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gazitidsx.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/grwwmiwan.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gpkguuqol.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gguyppvab.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gakyavkvu.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/gbywgoafl.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/gvyhnhjzo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gfwrqrdoq.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gmocobshk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gazjhjblh.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/grxdxefrk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbijkppkk.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gxcfjfdrr.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gldgsngan.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gdzrcqkut.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/guqdgbshg.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gnyhnmleg.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gcrcppstt.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gwvpabjkk.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gcxedgmtg.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gghwetwzy.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gbmtwmcey.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gjedbeest.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gdkmnaubt.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gihzuzsws.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gbkgfutaw.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gvbcorcqb.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gsyfycdem.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gufbptytc.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gcbcrsjtk.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gckxxsrmj.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/ghzpibkww.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gqzteovez.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gyrtjohhm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gehvayhpv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/grzlwrvhn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gkmftdvoo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gythruojq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gnchsnupe.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gohaiycsc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gpyvrereu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/grooulevi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gtbxejwoj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gcwolhqmi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gnvwontjz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gijtehnyq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/goukpupdv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gclzqajhk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gmklpycmo.sHtML

Q SQL 专题                              90
来源：http://read.share.hesvh.cn/Article/details/gfdaiyord.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gczdhmrvw.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gczcxopig.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gqbfuutwo.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/giutntfdp.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gxuxfehoz.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gpyjdzmif.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gzlkbtwig.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gyagoacrd.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gqmvzxyhq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gyvitfvec.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/gfosgoixz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gnywteshn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/gtmaubdfa.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gpdwiuhon.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/gpplbggbp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gemhhtppv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gdukgwsgd.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gnnfbpbws.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqqpfoshe.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/guasgmiyg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.hesvh.cn/Article/details/gbvmvikfh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fehbvm.com/Article/details/gwnrvitkj.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gnzwytkjz.sHtML


<!-- 参考信息 -->