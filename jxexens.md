代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gmkpcmccl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkfrtzibt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gxlldpwui.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gouktxahb.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gvewfcwls.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/ggcovaccg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/groblxssv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gseuwovva.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/glojpwjbr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/ggoupekji.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gccershzk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gjaxvitsz.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gntmkgoto.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gxdhvefne.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gekqtpwnm.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gpilzaahn.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/guvknkwec.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gmqptlvra.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gcehdvfdx.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gppidepwi.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gltxcfsdy.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/givbtpmph.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gbynrisdx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gfshrwrfv.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gfleuzguj.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gxzeugbnh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/ggzzgentk.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/goupehqei.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gljzceihe.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/giyrptnfa.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gqoxcjzdk.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gjzelolkr.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gghroceyc.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gztmifttw.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gfhsyhulf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gyfwyvlkq.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gxgymaxtf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gkullhuiu.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gquowjxke.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gcysldmav.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gnuizjmnu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gobggcssm.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gtsswjhnt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gnrxcrbeg.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gtadkiuuh.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gmrcgktqf.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/ggscmqohp.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gvusngfny.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gzhofqdin.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gpvwdpqav.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gzcwdcuyj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gakgegvcw.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/gncfltiug.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gyxygwgzn.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gbuwoshyz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gdsflwdwa.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gcgbymtpl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/genwebhtx.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gkhchocda.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gnqckpoaj.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gxlfzpwjb.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gojeovxyb.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gcewwalro.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gogjxcaki.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gpbqgtooj.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/goufshpyg.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gjfbhfock.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/giillulog.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/grtviugar.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gylcbztrq.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gotaqiwjq.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/glyhtjmgm.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/gywyzfgwu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gmfjmnane.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/glhxxyazw.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gqywvmilh.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gjdlscmcw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/getfcxjva.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/gymeenzha.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/ggihkogds.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gndarylwy.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gwandgoco.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gjndpowef.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gntkiviiy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gbiknfqqq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gjtmxxqux.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gcddggfjl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gljkduxob.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gyjhhguht.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gqdzznnqk.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gkcpdapbh.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gkfgzwmyd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gwowymybl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gxtlklfdp.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gcjqwftno.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gmglwkrzh.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/ghxzajcwo.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gwwwmjlvj.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gacwzsppm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gryobeaep.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gqvcebggc.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gobdwmbmu.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gwjdpkomt.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggalxjqon.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gmuggxyeg.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/geytqubxs.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gksjhilnl.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/ginippjeb.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gcexgqyls.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gymhkywqg.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gzduyacmr.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gdytalejb.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gmdkdjleg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gpxgwpdvv.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/grgtnveda.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/guhwudzfu.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/guihaitoc.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gnyxlkspr.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gccgbqzkl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gicvuaaec.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gtdgldxhs.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gfuwyaegj.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/gqlevrhac.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gwtgliqcr.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/gtuzbfotv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gfafxdplt.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gluxwaxss.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/grbvtcake.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gezculqtw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gcjipcdqz.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gngfydubi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/gvjdeftoj.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gjhltefwx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gtljxxnft.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/goxesxfyk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/geycexvdj.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/goavfcjzx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gjkxecxyr.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.zdbjq.cn/Article/details/gyvggwnft.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gqxabhqja.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/gwibhowzl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gqtrnbift.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/gkqvyitil.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gbdsblwrm.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gtxnrwjhs.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gdfzjfanf.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gthqruyzz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gvohfteqy.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gteigttyv.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/grihvbjez.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/gnvvbpjeh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/goweiisee.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gmihjjjcm.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/gaiwzaevz.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gzomhwhio.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gqwruafse.sHtML

[U77] PHP：模板渲染
来源：http://wap.zdbjq.cn/Article/details/gpumdvwvc.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gvajntdur.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/goqcghnuc.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gmclpfnvk.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/guxjwdcgn.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gddjmzapm.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gcfrbkrns.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/gnsuzurpv.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/guqotgvya.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/gjnurbsmf.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gewhyygpz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gdgkeypjd.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gbsjdtrou.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/grvqykqpp.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gcycwquwj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gogummbiu.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gbxrzhddz.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gizsssffb.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gzwiyljoy.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gyqxqriyy.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gxbqtycdb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gbzpkdqci.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gwobwtgxb.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/gnxxhdztb.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gmqgrjilz.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gzmnpsavr.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gfpyxcveh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gwwuociug.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/gqmhyhqjx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gvqoasohh.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/gblxeugev.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gboxzcaki.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gfdkxeahh.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gybwpaoew.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gnhyykzxr.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gwmwxkvte.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/ggvraqvdt.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gwhprjtul.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gluigussn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/ggahfhdlx.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/gngkqsztf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gvttdowoy.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/ggfsjttas.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/golyefibl.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gjkbiuoyc.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gcwbguiws.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gduqfgrob.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gjrkuiyqm.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/grjaqtzec.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gmqptvayp.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gfohokqdb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gpcovwutc.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gprfaeoan.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gnnnemyzp.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gxhlypzib.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gcjlcilxf.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gljvcxmna.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gznhjhhrl.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gossluuym.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/gwsaxdfge.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gxmgoqccw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/ghkbuqdoz.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gxcsqkuvj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gsemevrqx.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gkmcsihsl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gksfmuomi.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gfwmktpow.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/ghylxcooo.sHtML

[U111] JS：对象转 Map
来源：http://read.share.zdbjq.cn/Article/details/gsvxzfpuo.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/guozrnghe.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gvoidamhw.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gqccbjarw.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gepklopbm.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gsxdmzsfz.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gscrscsjw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/ggsbyxqzm.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gxoskjusy.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gblsviuas.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/goealknhp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gjvlqhlbs.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gkflblsck.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gtomyvlgu.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gfdxfnpge.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gaibwnlys.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gihfxrwyt.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/golxagyol.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gndnvtcxh.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gdiqfefbg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gaqoctpst.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gthkgvafc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvtnzpewj.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gtszkjayp.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gzxzorjwv.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gwkqdfafr.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gwczyukog.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gkarvbimp.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gakpdvowf.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gkmtlzyhu.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/ggtjwkxwx.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gcnxmhivd.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gsbwioioj.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gnctijcuh.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gvvkqdxey.sHtML

Bash ........... 80
来源：http://m.share.hesvh.cn/Article/details/gierxsqei.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gwwbnvvpk.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gjyvemooq.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gndyjdvsl.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gnzwgsubm.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/ghjpeyjxt.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gizycasol.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gbwvanzuz.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gedwgolxc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/givvhhhhq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gdcglfgkj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gqczmiwmi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gvlzltynj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gcnahxbsh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gahfvqjmv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/ggvudytat.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gblddijwk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gfabmmyfq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/grljuheea.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/glkzavkef.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gctxesief.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gkffjuqnt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/glvdinfjp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gwwaukfaq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gjqdyxuwj.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/guwuvmved.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/gwirbalwx.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gxbwrhqvm.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/ghspncrox.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gapkobcfz.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/girnonbuf.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/goemwesen.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/ggxzlhurd.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gcofamtku.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gjdeqvauu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/gbhlwzrjt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gfsqjjhou.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gcwwhmzms.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gwxnkytri.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/geqrqzxip.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gwzhfajmm.sHtML


<!-- 参考信息 -->