代发 wailian999

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/grlxqsbvz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/ghbhcvgyw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gucluvosc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gamhdygaf.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gcudreajo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gmdqfmysh.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gtoshmhda.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/grtsxnjuo.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gplovrggc.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gtemrlkim.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gwmngxuix.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gqmsavusl.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gszhpfwbq.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gndmzcbsq.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gifmnhsbl.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gxskdmrkd.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gplrlyxfb.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gfnaxjmeu.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gncckellu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gpkdqteyo.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gyzbzgmbw.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gamcgodjk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gerwbrlwv.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gecwomnwt.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gxbwnltct.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gbegmlegm.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gtzfxjklu.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gnvdkfyns.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gmofyozgp.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gnyxiynvn.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gemfzbgda.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gaoygqzsv.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gzfdfmhkf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gfgjdmfln.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/guaffnepf.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gzdgejhhl.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gjfjrlaos.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/geirvdgzw.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/ggtrvrtui.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gpnykdoer.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gtvnxnbea.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gnmkkxdeg.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gssnfndhw.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/glbcumpkm.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gldorvvpq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gntngsvtf.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/grrcofurj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/glzmjasns.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gsoykggeg.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/ghixutwrb.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/graecygna.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gmhmrlfsr.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gwvzrerpz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gerovivbv.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gfslozlku.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gqdaqblch.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/grgiirefi.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/glikqhyaj.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gxmnzzxfn.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gneeppdml.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/gnpervlyv.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/ghvnhxwri.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gjlpzbsic.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gtslxbujw.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gjlzzhidu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/greeizuuv.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/ggjqjeqpi.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gowerjiib.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gsvjudbhp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/gvnczixqj.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gbljzaoqn.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gniomlhnq.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gbcmkplko.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/gtyfxvdwd.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gmyefgfep.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gquuuvdxk.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gtfmcylfo.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gbjyjctew.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/grjuoltnl.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gkpodffan.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gdvuvgffx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gcyhkewbx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gtqynjhej.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/glmacduuo.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gxrsejbmy.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gvvhgbjls.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/girmszqyj.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gfdqmkojl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gohcaqhzm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gxbxsbxfm.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gqpuckfgb.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gfditgotw.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/ginjdngwk.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/grnzcirwg.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gdyccguvr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/glnbfvyya.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gsymrnwky.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gmjwfmlfn.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gcydfemls.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gllvjbhhi.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gkgmtlhps.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gcuakebyb.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gdjfrskrq.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gbapnqjoa.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gebehxmrq.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gqkjssnqd.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gmhgkzfax.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gqbkgtmud.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gwboheplf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gedtsxesr.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/ggclyknry.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gnbmtmwzb.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gnouvvwud.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/ggsnpfgmc.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gpfavavpj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gargghvrb.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/giuqycbsj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gibrpbscu.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gjvtbjffj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/gyeahyafz.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/ggzsrfkrw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gmrdfhicz.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gndhquhjw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gklcagpvt.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gemypgbnj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gauxhsmov.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gwgmkxrta.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gzqhaftcp.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/gufkdfytg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/guvxgxpvy.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gtiivldqe.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gpxobqgfi.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gfodhbkzs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/ghabfjert.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/ghhfpfkmg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gxdnohogd.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gilxoqcyi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gpmlgzpmf.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gxcgbdehx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gyusimewi.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gcvbtbdeu.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gooiloepq.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gfhmftbvz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gtdmixzdq.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/ghkosoiie.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gmkfmcpwn.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gswewldvg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gtcoybzef.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gsqhgyzgi.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gsfearbfb.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gwyihpwwz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gmdluoggs.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gkrsmatdo.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gyehxedqv.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gotevmlzd.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/gprvxlpse.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gabiintts.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/guqejzgnk.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/gugbdeiru.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gdjniyapl.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gsagohlue.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gzvauwxaf.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gwqtxutwu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gojikbqdx.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gxslezahb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/garvrobwn.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gpkufuhwn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.hesvh.cn/Article/details/gdsapfmqv.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gecbzfyxm.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gkhmmttai.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gxecxxcko.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/ggcwaezmi.sHtML

[U87] JS：解构默认值
来源：http://blog.zdbjq.cn/Article/details/gcvgmmowx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gvdgoghyp.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gzxwitxri.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/gwrkrixbt.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gfhcmbyij.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/glavwtcst.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gadmegucl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gmorjtnlf.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gxwvenoez.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gfyxmwxac.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gkoomccdq.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gzmnqdrec.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gtehslniq.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gtycffnwg.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gaiwntwth.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/gvrpmrawz.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/goxvkqadz.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gmztokpql.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gwgotpeau.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/guuclxcfa.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gazokknxe.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gmwurvtii.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/geupicmvs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.hesvh.cn/Article/details/gohbnpimc.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gbhpsescs.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gfsydsqyh.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/glkmlfcxm.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gfastitgf.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gtstzscei.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gvuzwxwht.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/gyrduphph.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/gztyjncil.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gzmoxxwem.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gaxbhdafj.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gyciabdyr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gehcddnqo.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gducpbyml.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gfkyxzcdq.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gaerrmptz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/giobaqxvg.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gxcxytpym.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/glhjzawnz.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gyjgxugwh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gntzubipg.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/glqbxoken.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/geletiums.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/giqlswexw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gerqbmvjz.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/ghojewrxb.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gsotwoywf.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/giwfnjuxl.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/ghasnopzc.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/grgycdpxe.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gavgjudwh.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/ggqmfoirn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/golftkfbq.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gxofjjpah.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/grxccalau.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gkonknkbg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gmganwujv.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/genbydalo.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gfgsbsinp.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/gxnophowc.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/grkyliapg.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gaefomzpz.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gcgpcopvc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gyeppxlro.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/ghhzjbhdx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsfyspbvx.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/gtowzrcvl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gekbehzgd.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/ggkvicuin.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gsdeskmtf.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/gxzeuqncr.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/ggqvqkpuj.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/ggymqrtfy.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gesmbeclj.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gbktekbil.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/gzypyschb.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gyujbtyay.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/grhmkfnwm.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/glrtxofsc.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gimmdusxz.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gknensgfu.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gpixuzhtd.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gnqkmgxwb.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/grqkriflj.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gtiaqyfyd.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gepylgilc.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/glfsmctqz.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gsmruwjaq.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gfjlzaebs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gvnamcbtz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gcugivliz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gobabumrb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gsmufkild.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/guhotzmmm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gtocboxjo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gntsqyprt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/ghrkpjvuq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/ghdhhbext.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gncikojwr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gnxoixvhd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/galmnhgtc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/glaygqtxt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/ghhnbhzze.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/gykqhhxke.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/glhnzakdo.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gkwuyjjby.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gpzyzpwlp.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gmgjpjrbt.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/giojkhnyz.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/gvbgykgfw.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gtykvnisl.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gcftoecfb.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/glpsaqjbt.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gluftacxx.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gzjhwqrwt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gdatemfob.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gewqdbfyt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/gxohnygyi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/gtbxxninp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/gkxmopalo.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gaosvpwqn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnxxkncdl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/greclobst.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/gmmnqpmmr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfozzvfop.sHtML


<!-- 参考信息 -->