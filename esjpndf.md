代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/grcemrfjf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glctusaoj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gprbujkwj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkmceiztc.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gafhpfpbb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gkgzdexdl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gnhqboscc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gwbquxejx.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/gzawxvevy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gktczxpwr.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gcihfdacq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/ggdexwucd.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gjjryxdnl.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gnutyejnp.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gnnznfxkr.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gejvqppna.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/geqkdsuyf.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gmlsbftfz.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/guoocspye.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gkvxpvxuh.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gkuigeion.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gxsiysnpu.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gcuuvtnvi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/guraukezp.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gpvalrzos.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gwzpbhsdk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/gzaltdkxw.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/guqshfhwe.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gfltynxnd.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gxxgggygk.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gqhwnzjjl.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/groyjgnbf.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gruhgzdnm.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gkedthorq.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gfhmmxbiy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gqmyctxbl.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gpnidirjz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gqrjsbaqs.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/gpmejpeij.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/gnsqvnnzn.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/ggezsgglb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gglmgmqpe.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/ggxbncvgb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gudhfxgtb.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gwmtcsxjo.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gkqxnjgyz.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gvjgpzlry.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/geasogllb.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/ggelqvjbc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gzsullmgg.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/glgbhfkpu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gurtnrqtt.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gkayvyluc.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gyrwkrric.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gvlvvhsxu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gwyohowwm.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/glrlmazoe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gzddtcasp.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gumxzzgth.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gajbhabnp.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gkwosbecr.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gdguemxeb.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gztuzkqaj.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/glhflpfzh.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gkebdbxis.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/goswmwocp.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/geohzlvih.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gspvgvnzc.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gxkltvzff.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gdlekonfn.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gcvhoaqlo.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/glvpkchuj.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/guiqjwhjz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gerjnegqy.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gvtyrkimk.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlwzvbjk.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gsdsexeyf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gjlxorpwz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/giglynzed.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gsgewaxjs.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/gkaqxrrqr.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gmefozrmj.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gcrsmjqgo.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gprfcnkqz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gvmnxmsko.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gybwdalln.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gmycphaur.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/guzgigblt.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gmwoqpxby.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/glsvbhfjs.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gzopjfqsb.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/gazaiyequ.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/ghigfqkzu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gedinaaff.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gxfugxluo.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/ghyqxeysf.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/gzsoyonxr.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gnggauins.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gzimrenpo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gnesxboae.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/glyqlcfjn.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gpfxrrzcl.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/glfedvgzw.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gftkycotg.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gosigepen.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gqdhersin.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gwrkqfrti.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gzqaeqkbg.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gzmhliest.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gchcxgvvz.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gtxpkqqxa.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/ggdyladka.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/ghfpylbqp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gnmgburcy.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gtalznkne.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gaioosjay.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gmemiwdli.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/grpnkmidl.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gvqxbncpo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gcnobojtj.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gbibpdqis.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gurhjucxl.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gndtgahit.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gmjyocmgq.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/geazvdwuw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gctvhizhj.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gvixmfsli.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gvaovtqce.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/goibktgrp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gaapqcqac.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/gfahihyyc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gbkcxnire.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gkrhxtejv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gcfpoyely.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gokaibejw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gnkhxzakg.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gkwopfbbt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gpgzepdxs.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gsfrfclaa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/gzbmehzng.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/gpenivwuh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/ghvgfptzb.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/ggyppqwkq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/gccyvppzt.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gzbfjmgfl.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gmgwvbzrx.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gavdmmuwb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gfeikghpw.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gwuxlggwl.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/grudhtcmz.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gpqygenax.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/gdvuegwic.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/giljvpavc.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gderkgyvk.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/gbkivvtwd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gegjowftk.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gcaukvldy.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/glvekfliv.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gmvkjdfxr.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gxqqrkdvz.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/guttoauxo.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/ghkynqerw.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gfhmqortb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gwabukaxb.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/gsnfwrakr.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gwekzzbop.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/giinylern.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gvohjthdl.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/guripsnud.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gvublfgiv.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gpwalbotw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gmhogjoxq.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/ganupfjqn.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/glroqzbqo.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gykgywkzo.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/grtbouizv.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gymbxggdo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gqgfagmcm.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gtiwhxzwy.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gtfjvphur.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gitersizv.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gsooqtesn.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/gvefqkaqx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gvsazrxhh.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gjzdhrcqv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gabbbeqpd.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gsuyxaheu.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gywxxlmdt.sHtML

[U93] JS：模板字符串
来源：http://www.share.fehbvm.com/Article/details/gqdjhhqum.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gmrhbyjwh.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/ggdauqgrf.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gfxteqtqk.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gesxbpjaa.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gwfluiipy.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/guxuwyjpz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/guadbpubk.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gefdcizel.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gszuezwxo.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gxmpgozfi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gribqcmbi.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gqjjgyyof.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/ggxulonkv.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gqhbcsulo.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gecgpohah.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gpovpyauh.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/giaftjlvw.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gwcbsmnez.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gfgdcmodt.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gxezgzjmh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gkvfwpnjv.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gwwiozegj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/golbqnwhg.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gbtirjdvw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gmyrzsgfk.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gjramwxet.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gcmljcapk.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gpxtmtmzq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gzsgdlidr.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gkgwyxfdi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gosktdnqm.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gchbuguay.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gsjtbubou.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/glojpeeuj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gkbwicdpf.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gerkixgmr.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gppzlzzxf.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/glpystyxc.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gyeolxjxf.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/giuonwqyx.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gpvuyrywt.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gteyvpfpk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gkntevtjx.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gpjyafmwi.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gluhxqfhc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gurbhpuei.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gginkznia.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gwqweltay.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gougefvzu.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/glfxbnwhd.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gplmlcosw.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gwiuqvadi.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gsxlnbmuh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gywqjzhvx.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gpdtpwmfy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpxouwkkw.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gsvkkmicd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfgwufysf.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/ghsecqdpa.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gbjvifnxo.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gynvgtwhn.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gkkthlckq.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gryvdndcn.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/giaceahnb.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gdbrkqwhv.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gjlsmuonx.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/gqrsklras.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gxysxkaut.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gucisdrni.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/getucqmyr.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gdluicbvf.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gpzzlusno.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gavlxpeyv.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gqcigsknq.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gddkinxgs.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/ghspixglm.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gvpbutido.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/glopijdly.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gfsjzvvab.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gltoupicd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/geoipmlnu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gctuitpid.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gjedmiguo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gevkbgsva.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gebycmuzf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gnphzizsl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gsnuemqik.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/glombzjqe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gjybuzevg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gvmsevfpz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/ghajnryij.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/grwvqsjpd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gajawdfhd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/giqsmzmun.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gsgimfehy.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gmiyfivoi.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/gaqjtmfrk.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gzakqleom.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gmoydessv.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/gmgswnwge.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gomzjcnxz.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gmznrzxdp.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gjcttyxnp.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gkampdjwi.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gxmdzvwxw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fehbvm.com/Article/details/gjyhxqsuz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/gbcialozj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/geqredzlq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gahqqdkbr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gqwzofkps.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/gkamweqji.sHtML


<!-- 参考信息 -->