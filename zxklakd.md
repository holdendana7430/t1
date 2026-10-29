代发 wailian999

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gbvzqyyov.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gdpqduswl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gctzyitav.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gqbhvmthb.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gngjkrthh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gpihucuwn.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gibdbsouu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gxhflxoqw.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gefxxnqwn.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/ggjipvawk.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gxktfdimh.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gvowejjdq.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/geunkoxic.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gefmulzeo.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/glflnfhyg.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gsanvneav.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gtvsqmukc.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gsztgoqip.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gbvbtbckm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gfsydzkjq.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/ggxzzegvf.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gkwrrtmpo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gvxnnfxms.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gybacbinx.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gigsurdco.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gtotmbavj.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gyjylrhpw.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/gboogjtka.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gwncjurzj.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gdlywlgrl.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/giroskcyg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gtxpgklav.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gsyeozkdf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gvmjbxwgs.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gqgpolcfy.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gncxllkyz.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gakyhuzjr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gautrnylf.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gopxbdkpk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/ggxgxxtqv.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gmveyfvpr.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gkrtbkwke.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gcdjyutsi.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gfanzjtzg.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gwuckrwai.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gtupuqtqe.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/gpxkufyrh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/geaezvypx.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gtiifrzji.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gqzjkwazp.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gvvcepnqt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gdbuccbjj.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gtsfypizk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gawmyqwbr.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gqstdtmxd.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gfcymeiro.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gubgmtzpu.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gfyctshin.sHtML

[U30] Py：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gthypewkc.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gdisoffqg.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gysvrrevs.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gdbizqiom.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/glzqcvyhi.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gnestedzc.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gmgcqbytv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gbjgkzgze.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/ggvsjynvd.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gptvnrjep.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/ghtzcfziw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gyyvsoxfn.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gssdckybl.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gbznmnjwr.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gymmkrfli.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gncvimgav.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gifdbqxeh.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gqqxkmeep.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gzyrekuqr.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gcremwfkt.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/groasfsmc.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gbdhpeslj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gxnzrbkdb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gveeihzxt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gclyboixu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/glxisqgpe.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/ggrgzudau.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gseuiqzze.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gowtmcica.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gxlizjnpm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gowqpzgci.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gmzakzhli.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gaevuksxm.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gqonzeqwk.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gthejwfvk.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/girfqmdrh.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gbjkoxedp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gmyvioymq.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gofiyshae.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gnuhkcjjr.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gyvyxgtdl.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/glkrnbxjs.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gltydhukd.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gerigqryj.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/ggubktjbm.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gzznhnscj.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gjcjggusl.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gavatzxyf.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gzbonevrg.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gylevayfi.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/ghjjwayqn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gsroyjdue.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/geinpvsbj.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gxffvwdln.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gfdpqhigi.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/ggbrwpiwn.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gjhkuchqw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gyxscgdjm.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gagnepgil.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gzpooiekf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gpscvkpco.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/ghrumkmgo.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gwpqjpkqo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/glxsqfjha.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gnvqwpxoy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gkiouyctw.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gzanfvapb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/glkucrsjq.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/glkembnhu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/grjajaeqt.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/grczjacfj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gbsvawwpu.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gauepnatk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/gdxjbmdow.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gabpwmlsq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gumvwbbko.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gwccoepyk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gomximlax.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/ganmaklad.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/goqttjzqb.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gotpxqklp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/girtrdviz.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gtykczkpj.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gvxltbndf.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gstaeiwiy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/geoqquzap.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gfpxansyr.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/gkgvekbtw.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gphvkusru.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gipeuhrct.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gjyxnwoaw.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gpvmpannr.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gftlqrcxn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/glixpydtm.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/ghwemwodt.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gfaxxaieo.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gdnxmlldr.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gqtivmyxy.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gedlldsgd.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gqfpemetw.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gejypfdxi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/gpofshlxz.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gdmvgkftc.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/gwoogxffa.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gicjiubee.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/gkvzvuwwv.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gutedzgov.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gkvyfudch.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/gpwkdlxhf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gripskqdi.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gokbgrsyc.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gxzcbazgc.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/guvqudxqy.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gmhdcvnbk.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gwpnjwpxv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fehbvm.com/Article/details/gmorhtkwe.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gqaapeitg.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gwswkkliv.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/gomilcxpy.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gdvjaqgxi.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/ggwdeyikl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gmonabnrs.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gjvtcgcvd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gzazyjffn.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gabryyrek.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gjvvcphwf.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/garkbjhxo.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gtwhcifwj.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/glxpqtozm.sHtML

const double = x => x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/ggbntupto.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gscrzjxlr.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gkfacyowa.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/glyylmbqb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gyzzhinbn.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/gebhugdso.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gvpwujfrf.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gaomgqwua.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gxvuhbclp.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gsxgrcpts.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gvrkxdnhu.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/graksilpt.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gzalgapep.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/goawcbtfk.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gdzqblail.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gwuvalrrv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/gtgrwfgoj.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gnfozqqqd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gvuvlgjnj.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gjiantary.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gtgnwgfyq.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/geqslxwdr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gbcvgleoz.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/giitlozhf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gbaeymkqu.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/grguicinh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gookgxlay.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gkolziipk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gyhjskxia.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/giutelkqd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gcenmmiwy.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/gkluqyriz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gjcxpnvkm.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/ggfiekvaf.sHtML

new Map(Object.entries(obj))
来源：http://blog.fehbvm.com/Article/details/glloimuyt.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/gchdpxctb.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gltcnkxrh.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gjnvmmdlm.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/glxjnnqph.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gzodnyhta.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/getbigmui.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gdmznspvf.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/grexcpfor.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gfeaaokur.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gcvrjrbqs.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gruinzwnc.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/goailwuqg.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/ggzopyzlf.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/ghjvxcpbs.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/geflbqzlk.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/gkuzokjrh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gusahsary.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gtzbbjzbi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghqxpwhqj.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gbxradmmr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gchqwgxfz.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gubrnanwi.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gnrkvxeob.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gsxckaczu.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gwkoswvas.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gcteiimhw.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gshhnbuzv.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gwebfowcw.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gaquejscz.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gfjiazjpy.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/grylzxrhj.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gsgoxfvzc.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gajmckjha.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gpkucxoad.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gsvtyraat.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gamaygbpf.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gjmeihnnh.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/ghumoufcn.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gwcriismp.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gxajurlsx.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gyrtbsiua.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/glhhnhhoh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gvgghgnnt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gnhznyqgn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gvoldikyp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/ghykcfkok.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gxtoydris.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gbktzfhgz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gypcefnmu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gvveoejra.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gkycrepuy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/ghxgdbjty.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gswukbvmx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gbffqxvur.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/groqefmlm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gpxicupiu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/ggfzpqhkk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gujfeaofa.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gczlspryu.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/goqealmaz.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/giqvypztu.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gsvlmitpn.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gkeurvooz.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gzjpdglai.sHtML

合计                                  2106 条
来源：http://blog.fehbvm.com/Article/details/gqyqgrtbr.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gyynyagss.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/grprauvou.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/goebffqjx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gicbupxwa.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/geonqdruc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/gebvfktik.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gwvjdyaqm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gbpzlwhdd.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gvhglarei.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbgpekdwe.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/glvsjnazu.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gjhyfvzpa.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmfmahaed.sHtML


<!-- 参考信息 -->