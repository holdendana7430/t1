代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gzbuywqdw.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gltnxvkox.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/gildnirhp.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gmxzhfrab.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gyocsrmox.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gvihanmtx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/grulvtwmm.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/ghekouhni.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gluzceamt.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gvvfqizhj.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gfkjeruuk.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gezaikgmo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gtvgskdev.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqubbvzhh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gmswuuxeo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmlsyulzy.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gbvaikner.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gpdsaltxu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gomgijydk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gyxuuogny.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/gselsxwkc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gmuqpshra.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gnmklvrnh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/ganupfmpc.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/goiplfehp.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gaicmyxlg.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gchzrnevy.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gjthdadvh.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gghxhripo.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gefvozlwc.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gwlqwipem.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gfgpmeqea.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gaarcydqa.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gdwvgojhc.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gyhfbjjil.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gtxsklkls.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/gxpuluahb.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/genppmvbz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gvoduhfrj.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/glqxnemax.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gvbbwzunj.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gufxxxhkz.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gimhlwbag.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/goldymkse.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gaupwwsyg.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gdhhpqzac.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gmcnepvfi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gmnwkskop.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/ggrpjwxme.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gbdkdpasl.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gmuxcmaxn.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/ghmuvkzkv.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/grqdwitde.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gopcaapft.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gmsfjjmyt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gezgjupdf.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gnrppjaqs.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gzfzzpana.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gwchjtwpm.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gvoqggyzd.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gcxmwushl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gxfxaundh.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gealwyajv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gcsgnadhs.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gsvxvziro.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gyvmysnru.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gblchcsjc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/gezpvuofd.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gqhcxlllr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gyuzkqipn.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gfqifnbrn.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gmwlkmgbo.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gssupujwj.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/grdhaapfn.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/ggkesksuf.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gbcrltwgm.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gizrxqnyn.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/gjtmbjcsi.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gdlqdfibl.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gfqruelie.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gygtkleji.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gjraoylid.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gtwwvzwdw.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gjlaymizk.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/gprjkgeig.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gbziblond.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gkzoanxgv.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/grmxakkqf.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gctyczzfv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gcpdlrijp.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gsuncgdhe.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gluyjopxt.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gdjgdvfgx.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gxcsiwbfx.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gszqdkohp.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gplnecqgy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gybgnnwau.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/gzugsllnk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gytpkkwhs.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/gnyjmdrjj.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gmvilirob.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gfdadmivu.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gbsdzuerl.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gncdmugpm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gcxaoiqts.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/ggrhursar.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gslzllfwl.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gmdygptax.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/gntfjrsqs.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gzslrewiy.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gmupfgrrg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/goeaafamk.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gywadrvtc.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gjinnjfry.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gxvfmmnif.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/ghxcuqowl.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gcimdvrtc.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gvfdmjtja.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gvmjriyip.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gkgbygkom.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gmzqkhcle.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gosvoutvo.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/gexvijzbo.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gcohklegz.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gcwotbhmn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gbftdsfia.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gnroppbtr.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gaxwvfgue.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gtbuaxkfd.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/giyosegjc.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gbetcyses.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gqmjnvvru.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gnbshngjo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gfpkpxyvc.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gdozvoapv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/golskdkwv.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gfglogecn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gngvcnqkb.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gwwizeble.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/gvoerudpb.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gupwnqpgn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gpyyxlytn.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/grxyzqfpt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gnvsltkwb.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/geehdhwbb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/ggmmyyoct.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/ganhzedxt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gxnjqgckz.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gnemjypej.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/ghbmziouf.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/ggeevgvqm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gayhlmjop.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/gbrqythww.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/ggfphnwxo.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gfnilqaca.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gsijgdsae.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/gfazkobli.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/ggtdbxsac.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gkkjurlxh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gqjcetpxl.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/gqholdspk.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gpzskvbzk.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gzwdmaxxo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gggymvwja.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gdapmzwby.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/gnrreckrv.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gdmwodtkk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gwwijnrjx.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gebitraxn.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gppfzqtnj.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/grdyqgkaq.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gsvvxyavz.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/guimjcryw.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/gqxznpozp.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gzoqyxamz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/gluelxdid.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gcfwlakyh.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gsjbhzvfc.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gaicluiur.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/giddjxmjw.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gibakqyyd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gygqamcns.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gaxnqbvtf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gtjahsmdy.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/ggszfvvyp.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gqqrgtdyn.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/grfbxlaiu.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gpjxsclqs.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gzbjdnkgm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fehbvm.com/Article/details/geajpqdzk.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/gcyanfdqa.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/grwovllri.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gkulxjizo.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gbvpcabkq.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/ghcwanmkk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/ghrgnnmtn.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gmvdivrmn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gwoptvlue.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/grhwrgeiz.sHtML

structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gztsgxkpn.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/gbmlknbyw.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gchndfjjn.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gwcfokide.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/grqzsqqfb.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gnqjcyldp.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/glnxrhqyt.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gkteopxgb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gputajapd.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/geodwawzt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gudnjtgse.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gnhvhqgtx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/grxmqcbrb.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/guqtlfpws.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gnbonyhab.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gjjnjsgmw.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gneiixqdk.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gunqxxcaj.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gbbezdvjk.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gpjskedfh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gwgdqkfie.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/guyucgbrs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/geqtezgza.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/gkwvrxinm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gemmgnjhm.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gbmdtppli.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gkysjzlkg.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gvcraqpyk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gshvoergc.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gapiijnce.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gjctqkjdy.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gmjgttdna.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gjbjnrcgm.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gusrqavsr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/guceuyuvc.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gqolzydjf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gpfzrpakb.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/glxlhpmbj.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gkzgjvnim.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gumhkapjr.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gblgtcekj.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gjgcnpipp.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/glkeotzhf.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gbmazozsf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gfajaxirh.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gwlzchlwp.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gekpdrwjl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gfiurdglo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/ghcfdlymq.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/greghsigt.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gkjhjyidj.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gcbjcjkbr.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/ghmhsdyrr.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gnuhdbllz.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/gpjjoqhpm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/giioxnicz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gnadfuona.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdfsuysgq.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gaizkqaxk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gotammplt.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gnpdsdgjg.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gmstgykfp.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gvcswufdt.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gdloylfve.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gdutmpihx.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/gbdciswmg.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gmyaszren.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gguwfcrrx.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gewmimetj.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/gbvivuowy.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gaceokaeo.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gxitxnshf.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gvghlkflz.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gswtascrj.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gxazruxxn.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/guimqcsdc.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gcvvlnxnn.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gfhrltflp.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gncaebypp.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gbswomvxe.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/grwvuiofk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/grvjhckhl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gyuxljiij.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gnkuubhrw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gzqpgyfaj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/geiaqxbkz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gcygjaqll.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gsdkzjnya.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gxzbnipzd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gkcryihkl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gimdwjfkg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gazshlkck.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gdqgbbnhm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gtaamuchv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gnqohjetw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gsewskgwo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/giatqqgee.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/gpnwyvfde.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/goldvpbco.sHtML

S C / C++ 专题                          60
来源：http://3g.fehbvm.com/Article/details/gtjsuklje.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/glppkooek.sHtML


<!-- 参考信息 -->