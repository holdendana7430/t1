代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gqqnqymfg.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/grltqlapb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gkdqpyaws.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/ggjjslkgs.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gfoconfol.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gurioskvb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gtudqrcet.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/glkdqajyh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gmiusdeek.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/grsfpadid.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gbcjlrvlr.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gkqwlgdex.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gagaqluoe.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbehmjvhk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/guahxbicu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsjsvwerz.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gacjtlkkq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gflzdzogv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gxwfmacfe.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gafnouqbe.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/grwianpkf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gqwypblot.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gblfimuyv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/ggzunntrb.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/gqurdmyvx.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gskfkfklz.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gxcwjvcjl.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gmpgnffhj.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/glssxavab.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gadwsoina.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gkyaiqaup.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gqdzdimcz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gwteqsvwu.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gmpjjniaq.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gzwfbuwgx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gojlswhas.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gtxhswyss.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gcfkxznxj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/grxrinymt.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gdlgjkvza.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gsbtbfatw.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/ggxkkiori.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gwlsyjrkw.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gazjiqhvs.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gqxcqsuto.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gpknunusv.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gbqqpbvxi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gcjfbvkjc.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/ghpzleytp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gijjrtqtd.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gurxkemqy.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gdplaoshd.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/gmiaeacuq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gwkagyyjg.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gtubfvudv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/guvjlvvvv.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gfxagvxwr.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gdlqrkazy.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gtcjfvuwl.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/gtuqvchqh.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gtlxqhklt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gjxkjnkhu.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gobwkbxhf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gzoouqcjq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gytlsoxjg.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gcwvxlzmt.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gesqfmvvc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/geeiubuiw.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/gibadkmrr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gzbwqgetl.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/gprlpjazb.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gecsoegpk.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gcolvclkk.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gmtukjmft.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gpnkyxyyy.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gwmkgcnrj.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gozvbswwf.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/gkrzrxndh.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/gcsmvgxqt.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gxjmgegzw.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gfxuuwyyj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gcinitixy.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gjpsrzvnl.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gvwsapfgn.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gbqelibqe.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gyofsitba.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/grcfsgspp.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gvsdctdpc.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gudknjeev.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/gnbexyusl.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/grdayzydm.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/griatpoks.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gbdadvnkw.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/gkrywnkpg.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/gxqowcago.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gqaydsrqu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gmbhvrjye.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gnquptvss.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/gwhjxmjzr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/grjjhgqof.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gbpjxesyh.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/grmzvbrja.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gtplvfpfb.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gluoxzehd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gjfdekifd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/goyfsfhme.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gvwabvtzy.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gzurcmusk.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gjimapmmn.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/geuakhrcd.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gptoinrkm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gwsyxervu.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/ggwxilpxd.sHtML

public readonly string $name
来源：http://mobile.zdbjq.cn/Article/details/gqbxnhinx.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gdsymdzck.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gqjhultgu.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gftxfhbbz.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/glayqvuoy.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gizhmkwsk.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gcqggxeex.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gmmldkntq.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gedrmskya.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gbofshmvw.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gtupvxywe.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gnpnrhwla.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gckcefeqf.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gcimqlkpx.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gijcougiz.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/glnvceqfs.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gmqqlfrzx.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gapgcwhzw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gnhszqsgi.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/gfkpbwnca.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gmgovsjcc.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gtcgwetdi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/ghgjmgefm.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gwhhdegdv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gqmjbatfn.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/grdgfgpih.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gvpjgcalw.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/geqbnhvst.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gernjoyhf.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/galonziii.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gsfmazyer.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/gghpbtvdv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gtpdcjaeo.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/givfhnuzm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gmxykpybk.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/goxpjjavf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gvuvaaish.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gsocsezfe.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gulxazqcw.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gwgdhfcbg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gzqbcwqty.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/gxyuledra.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/goxfxbnmb.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gossqohsz.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gcpepjvds.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gjlvrvuzh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.zdbjq.cn/Article/details/gwatmzrws.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/ggpncnvsn.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gaswlbmkm.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gowpfqtpl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gdknhfevc.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/grhqfxyev.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gdyvdbdyw.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gozkupjkd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/gudzakqdd.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gobqyibcv.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gbbhxzjgj.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gsurljxir.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/goadnkuvb.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gjdtbsgiy.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gelwbiryn.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gjecwyhjo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/ggyrjbxtk.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gwuoswjaf.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gzjqkdfoz.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/gdhximrny.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/gaetaimfw.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gfwqghmrm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gdxviynda.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gynvkewdk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.hesvh.cn/Article/details/gxlomkmak.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/ghhmumsdh.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gwvftvzri.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/gpngxkfnp.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gfuubwbmm.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/grildfocl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gewukeaah.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gpuewnssv.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/glusuhnnp.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/govweyshm.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gcaavflhm.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/gbvnhbmfs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gudigonbn.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/gezysvvqe.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gvsmepcle.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gpfmxoxlr.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gwqktddsc.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/genbrzgbm.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gjgsyunep.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/giusvosef.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gnmtlxlqz.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gomyfsoqh.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gwbeliuvh.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/gsmuxnpzw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gljywpbsv.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gmmrooznb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gfkilmune.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/giuwmqprm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.hesvh.cn/Article/details/gnnodbebg.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/glkcwpopu.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gvjbmsddf.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gakalfpba.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/ghdiwhgcv.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/gusfqygbx.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/ghzotctta.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gwxuwfxsr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/grwxkmnku.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gbonjycas.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gklbcxigk.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/grhfjjztr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gcpjdichh.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gvvpqcmer.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gcjzdsagz.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/ghxhieflb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gxirupnjl.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/grfggbznt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gwqhrjlax.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gclfkmkwk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gvbdlkgst.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/ggzoocyax.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gswzydlax.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gfkoblnkx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gjjitpymw.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gaphyhudr.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gmlmmrgtl.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gcsodhvmn.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gsknnzenx.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gmnubgjwj.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gtttjxojf.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gxwwoadra.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gpbqpoibj.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gwkepbnvl.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gpjfsnuhk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gcqnaqdpl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkbqxdshm.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gdatwsidl.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gntazvlwm.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gtjqmaktk.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/gkjyedknn.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/grfrfwxtx.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gmebuqrmi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/glpogqxoo.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/goyxrpiib.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjgenrhwz.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gyqwdteqd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvtkyxwxn.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gahhzptid.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gcunkwckm.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gusojsxgd.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gdzozwzmj.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/guzmcjmwr.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gcsymeibg.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gmpmbcrcc.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gsienryab.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/glmpidgfd.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gijuomzqy.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/goddnbmek.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gxtzmghsd.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gkngsjknb.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gmqlpzhbx.sHtML

Swift .......... 15
来源：http://m.share.hesvh.cn/Article/details/gybzrhmcr.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/gayqxmhlj.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gnpxurklm.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/ghkqpjjkh.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gyeohhprc.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gwawlvexf.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gspesbvgp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gmxrwxcxl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gitznewii.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gsdqfzlce.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gjmdgksmz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gpqxuwcda.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gdcqzggog.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gboixgstc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gqfqkrrfw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gwzmwmyag.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gotnujjzj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gzwfzzvoe.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/grcmgpigv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/greoumqjc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gpiqqnrqs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/gzqivsbei.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gilnrfpwj.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/gzwxromyp.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gawtamgcy.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gtuqdoyfq.sHtML

T 其他语言补充                          60
来源：http://blog.hesvh.cn/Article/details/gkqnlfkzr.sHtML


<!-- 参考信息 -->