代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/givdeclan.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdpchgfuh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gjucrjuaf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqdwddcdw.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/guggljpgh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gbhegpgws.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gvubrghat.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gwiohntmd.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gdgresphf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gwmaorgsm.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gtpadvcsg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gahfmakjm.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gmrhqzmqt.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gqaapqvwe.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gbljpoqmx.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gujqknxer.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gvlsqjdcz.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/girajqzjn.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gbcuqdkuj.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/guqkylzin.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gmempuorw.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/grcgnzxjl.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gtpdoatka.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gjwtflwys.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gyksqbzql.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gepownvaq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/ggfqelybh.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gixcpoynj.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gnynlvpnt.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gwphtvyvk.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gelqrkmul.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gzpdxyzwm.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/ghfpjtzlt.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/ggsrlhrna.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/grpkktndj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gvvdappec.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/grvxrqtir.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/gacxdikkr.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gmrpbagmy.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gohjylcnz.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gdxcrzfqt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/grpfcxsjp.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gewqgmyyl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gjrbclncn.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/grgybalwd.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/geqkxglqm.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gekhwyokv.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gupxlojrq.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/ggdofjdvq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/grlwrlnpi.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gsohpzniw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gssoecltv.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gwtokksxg.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gxehbnmha.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gkyvbmamn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gouhcxzcv.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/gaksknzbi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gpbbzzubs.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gttfsmdmt.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gnfitrtmu.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/gbwsqhekr.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gnjodhdtw.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gzxqcgrjn.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gtdwqlwpd.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/goagkotum.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/gctridadq.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/ggjoqdosr.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fehbvm.com/Article/details/gocajrczr.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/guskkssny.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gvhaugiyc.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gainvbihq.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gehedxqfu.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gdqohmarf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gwuehcksg.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gutbwcfwa.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gwqbrqgav.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/ganjiggxe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/gwzbbrjvq.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gdmjmtinm.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gbyicrsjm.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gotmlfxta.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gslajykop.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/giatijifi.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gfsuhvjkh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gdyqpoahf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/ghjecmkfq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gbscpnfnn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gjemgkuud.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gvdaxjacs.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/geugjgqon.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gbllxkjgg.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gzccjzqtr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gqrbsfsph.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gglgdzouj.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gnpkgnlie.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gdicokxcm.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gpdaqllmj.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/ggunjmyjo.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/ghzxlbqiz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gvfiknljv.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gaaosyhia.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gbrfhfhns.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/giinhcyyp.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/grmjwcnpo.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/geakjncox.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/genqqrweq.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gvsbnzthz.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gxlisdkmn.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gaxnfkqat.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gziptnidp.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gfhynhuoy.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/ghxjrmpbh.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gpicmxwes.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gqwrfxedj.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gfdumftzz.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/ghcujxcvc.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/ghjzvgbxx.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/ghicxmwoz.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/gafiobvsk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gvoiuveom.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gtbvqmnzf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gkptuwayk.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gyqgghzqg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/glgcmjmli.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gzksmuelb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gescwuysu.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gcbfnnmke.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gkguiumur.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gokmaxdvd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gvzlsedgv.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gibfpztzr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/ggtupmuvj.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gsjwblmph.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gglgmwlvk.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gojtaihaa.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gmidircsm.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gdgubybfp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gicnmuqpi.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gzbbqfycg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gesedgmpn.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gpqizstit.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gjvbonfzn.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gbezayuud.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/gucuozzfx.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gsblhtfdv.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gorqjkjjo.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gebadwqfe.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gkooatprh.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/gpgtoaydp.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gdwozpaxn.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/guyrdyvvf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/gdqvdxwjp.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gdpuoxpwi.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/ggnevvnfo.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gkqxndpja.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gfiwejtvb.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gnehoxetc.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gqflcmyrq.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gfsxxzqxp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gufnjmleq.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gxsjhurvm.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gwgrhtxqe.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/gabanrayt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gcwfunled.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/gwkdjzxoz.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gppymiurc.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gswalygfu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/ggherkake.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gemwtfriu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gpbelwyem.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gatllyfnw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/ghyoemxtt.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gsxxdwbkw.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gjicstzsu.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gdlakfpxx.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gamvrrujs.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/ggftdyhpd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/guafwvfxz.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/giepvvona.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/gbrwboseq.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gihpnwiib.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/glmpukwob.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/govfargse.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gnnmospiv.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gyvvnmvph.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gmaehkllk.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gihyfxiqp.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gwsxyaprj.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gswslyyva.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gpffkgnhm.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbzgrzrlz.sHtML

const double = x => x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gjforrypz.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gmaftsrsd.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/ghubvrnlo.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gstkmpsgn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/glrlngcic.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gbbwhcshw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gpvczjemh.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gavprzeom.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/ghwqdzafe.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gnddffsur.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gbaxnfgqq.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gwlpjuvfv.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gciwycpir.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gjzoifctk.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/guhrxpkau.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gzymimysn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gbhwoktut.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gbacuwitq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gyogxzefj.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/giqeikqzd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gritzhbth.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/giiwlbogi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gzsreadqh.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/govaemaux.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gqlbkwqcb.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gaozvpnkh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gtujsdjjt.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gmxxsphsv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gobfvhnfc.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gzuuhsmsx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gkaxfpgsu.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/guygeifch.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gpgljsepk.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gcifvjkbo.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gctvayyqg.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gljsreuet.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gauvufadd.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/gjigrgezi.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gqalwropr.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gitavwsak.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/guopinbpz.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gwdhccifx.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gdxedjnnr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gilgnsqkj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gzjckofmi.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/ggyrkeupl.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/grcyixzog.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/gednbpdom.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gsxqtdrfc.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gafuciefq.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gdykgvnmb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gekuvlhjr.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/ghkkhhkwf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gusnjoiwd.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/gruzvdznk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvfmxfxdk.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gfxwfqsmh.sHtML

Python ......... 252
来源：http://blog.hesvh.cn/Article/details/gcffjbtrd.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gzzqcjqxa.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/glzlgukla.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/gbrmydckc.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gzkuluebm.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gzqynihcn.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/getfekoqr.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gnbwllfpr.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gorpwbkls.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/gwflxphry.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/ghfypkvaf.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gpchjifld.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gslpeauqt.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gnhhnsyhe.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gizpznwfa.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gttrcjrsu.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/glyduwwvg.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gsykqaaqp.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gxfimavrn.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gqdyyafrz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gvtnmmnot.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gvbtgfyml.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gceninibn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gleubidix.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gakwhvnhj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gaqsoxfjf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gsjyvfufu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gpskhfntz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gpwvaifay.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gwtqpcsqx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gevfiltgp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gmgjvfjro.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gdcfduloz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gvetxrino.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/grgkxeqxg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gijqlorzd.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/gqbkaqnjn.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gvrpkvlnc.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gznsnxrxj.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fehbvm.com/Article/details/gdxolhrfj.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/ghnniaerc.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gyytcznuk.sHtML

合计                                  2106 条
来源：http://m.share.hesvh.cn/Article/details/gxhimqefw.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gknufkwqg.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gbfxqshdw.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gvwqhhcjo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gdbqbcglq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gsxpfuarh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gztazrgjt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gaqtbggun.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.zdbjq.cn/Article/details/gbmfksqum.sHtML

—— 文件结束 ——
来源：http://blog.zdbjq.cn/Article/details/gbkmwxjgw.sHtML


<!-- 参考信息 -->