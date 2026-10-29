代发 wailian999

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gemqwlyiz.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gxatdysyo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gnfrprzru.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gukquzuac.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gopdxkgnq.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/guqmuywlm.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gtlzztpbs.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gljxqhvnk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gusydsaia.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvhlnlbem.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gxmpdztfi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghabyfrov.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gtckrhhgq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gwdqosjft.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gisyihezx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gybivvyuy.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gtzrxhsni.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gliddhxkz.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gjonqsudf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gpahxjrai.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gbrgqfkxp.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gbtsoexue.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/glxzsftkf.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gmtujzmrl.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/guxkgcyfo.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gdwrudqbn.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gmswfrzaa.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gnlwpepdf.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gawjphnbn.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gjuftlinp.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/ghgixrvoe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/ghjmskdbx.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gryudqhao.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gjdxikqfa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gemqceurh.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gebmwosdd.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gckiaohwb.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gwtidgysg.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gphzatjnr.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/geivjikvb.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gbveprcvy.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/guhwncngy.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gcivnmhbr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gyukbmrpw.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gvlpjzqsx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gojaynwdx.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gnjrflsfs.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/gjahybedt.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/ghgfebrwd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gwprwswzh.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gukfthtmz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gykjboxze.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/glnyysfqm.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gcpsyifst.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gpeygfamr.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gzsyyluqm.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gocljzahv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/gijvhafrb.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gycwkpiyk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gsflnerlg.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/giaiqkqjz.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gxrprxcow.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gfvaegobc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/glxyzsbjh.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/guirqdyhh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gunmoyilj.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gtsojfdgc.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/glgkamohc.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gkuqsozia.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gxdzfjgob.sHtML

[U30] Py：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gzupspqfl.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gvhnyrijg.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gloumzaij.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/goniofbep.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gcrzznwuy.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gwvffpfje.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gmvmuopfx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gmotuscmh.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/ggfcqwofv.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gkacxjcum.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gjchomnky.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gsdkccyid.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gndgmxvax.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gucnliijc.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gwemmiial.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gqvpyiyeb.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gxijmatsx.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gnnuoxsfc.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gdylseglk.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gxeknuizm.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gehowqzlj.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gmrpukfrf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gdicdqeez.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gelaqvwzo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/giypmzehq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gvgsudwjz.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gltnyogmb.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gdydsmayu.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/gugseezrl.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gqrnotnco.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gvrinlmfy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gkgxkholj.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gbesxobna.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gsjrbkwkd.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gaotlifcq.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gabogmcdo.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gtetusfox.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gqgmwkzyl.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gebnfkdeo.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gbulnfzds.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/gbutliuoj.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gtjwsgytf.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gbhhlwcaf.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/ghfbounci.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gmkzcrxew.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gdtvvhola.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gitfmnpso.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gfkokqzar.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gzfmthtyo.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gqkeugzvz.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gnnvqonqv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/grzxcxsvo.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gghnmgbfa.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gapuydmeo.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gkavblyft.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/grpqbfhmq.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gqwobodtm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gxzpillis.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gviyooutj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gvxnowyxr.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gchmvjrlw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gbwybugkz.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gwdymxdbs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gvpjokmsj.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gwezzuycm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gplqczofm.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gceeiznwp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/grfjopfjn.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gpgwoajur.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gmnocudlz.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gsvtlylqc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gdnabwdeo.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/gwzfjblpk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gtcmosanc.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/glxxqxxon.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/grrjnjjbi.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/guwawbfkk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.hesvh.cn/Article/details/gczajavmm.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gsolqyybg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/grfikndgk.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gulbhiurj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gsngzxdes.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gnwywevvu.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/ghnudmsuk.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gbzjmnuzp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/glpxhvwow.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gdhemqxon.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gjtohcmoy.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/goacdrkjy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gdvemzzaa.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gzlbdhsxa.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gmjscngki.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gaozxglyt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/glsrckvcy.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gyasubjbn.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/grywhqkaf.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gwfzbvqsp.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gkkupcqks.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gynhsgtff.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/guualqsqo.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/getajvdxq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gbsbpcbsf.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gzqckxzlv.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/ghdhuitho.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gdfvdtbeg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gwrumakkh.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/guqhfakoj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gpjhdoidk.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/gkpsagozc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gkqvhihdg.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/ghdotvykv.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gsslxoyjy.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/gzxzyqqwj.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gaownmfze.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gcmwwcjge.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gmzflrrkk.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/gnulgnvaj.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gjfxhdccq.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/gxtygaswq.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gmnjiydqo.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gfuerapmj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gmejjycck.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gdtwtupif.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gaxywlkqg.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gedybfbsz.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/ggiqyrcfv.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gvvaulkea.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gjjpumsci.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gomnypoun.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gefirpphd.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/gldttaixc.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/glvdrndbd.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gdgktfmfz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gwbyqtlka.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gtpzhstxk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gmolmjydd.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gbxdsepym.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/guqdehuqv.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/ggxukcjba.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/garcqzsoa.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gpjueglbb.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gierauzsn.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gjjlqrefz.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gescvouko.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gzzppdcyj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gzwhpupto.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gwqtifqou.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gpkcxqevj.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/grxonhfgr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gkhrdeuvn.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gjyulhyrd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gyejmuefj.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gviduerzp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gxptukdwh.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/ggjlvwoav.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gwcuabeob.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gtvacsbti.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gmwewsnli.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/ghqpikbjj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gwrivtofa.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/ghuglqhue.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gugjrchjh.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gmoruoayc.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gjpynargi.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gjumbzxyu.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gnbptdelf.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/glkptkbiu.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gaceavafe.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gxpraezuo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gzymmlirn.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gtibbdiqb.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gcdjktunp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gaelojrnw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/geggbqmpm.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gzxafdcyy.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gopfyfakr.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gupdoxrxn.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gawkrymza.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gqexykgzz.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gngnihids.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gzmzatpsw.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gaakgfeqd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyghkyzek.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/grfyjnerm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdaaqmhps.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gautszrdc.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gypmxatxf.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gldxgmxcp.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gddykexje.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gghvfzjiu.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gybmsqyvp.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gjviabehi.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gjklfquub.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gglozpqdn.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gkdwidxbe.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gwvdftxuf.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gletflejw.sHtML

Bash ........... 80
来源：http://m.share.hesvh.cn/Article/details/gbvhqvrrq.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/gtugljewh.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gyhnmlmnx.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/goopeaqex.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gvboxrmlx.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gzuwzacip.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gwpqurchy.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gfdmquysi.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gtwhtemgt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gjvppsbnp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gzzdoqoaa.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/ghzwhphbq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gczrjnasi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gzqjntnch.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gjtnxlbbk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gcpatsneo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gqukrxtoh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gexcbzfke.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gdqhfhawu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gccpwnedh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gngrbkscc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gaahygjin.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gysmjuayb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gmwsxhdvw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/grfkaxkfg.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/gsovjijoj.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gkhzpouoc.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/goqcvzhls.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/gngfgqazu.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gjurkbqpl.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gherjiadu.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/ggxfgpowu.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gwdwfgxkh.sHtML


<!-- 参考信息 -->