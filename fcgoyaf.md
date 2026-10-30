代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkjcursv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevnvbjqm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgfkvjep.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjlqcszw.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gwamyfznk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/giyydsmxy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gdixcwdya.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ghmtzmfaf.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gthbuppgx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gceyngure.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgwqoljh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/grjbwbxxh.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gsyqshiyz.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/greaosuvp.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gzfglkzhq.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuqxutou.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gngedeczs.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgfnokce.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgxalgbh.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gyzfkxojh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpkhtfuy.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/guwqnenpe.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gwbuqrlyq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gsigjneay.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/ghrsvxsyy.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsnxqtgz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gddnttmhy.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gegjmbdku.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gudnbrtkg.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/grphciaio.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhquklgz.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsictgnbm.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gxphhskkr.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gpjdixort.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxxfkawp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqpgjxiv.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmazsmdn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/guaajysqi.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gchccoeek.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjizaqull.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gfesolhgg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/geiirjfwq.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmbnoosp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gplithigr.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/gyolfpagj.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gllvypfqx.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdkeostu.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/grfqbppag.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gelnwsreu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiiyvsgr.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gdwrfyjji.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmnqtjzo.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gogsubqcz.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/glpdjqoiz.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjopxpqj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmausmyx.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzucxbla.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gsropbvzg.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/geccrnwql.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyquxcgr.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqhbzxmp.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlpjdwcw.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gopnqljom.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gnzcdhkso.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gmwijnzxr.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykvqxxww.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gxpklyzuo.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gptklmppw.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxiagunm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/gylhjeyjm.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjuvzshv.sHtML

chardet.detect(raw)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioecwscx.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gratyylng.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzebrzmyg.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gnofnqjkt.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/gghbcsesr.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gydgdvufo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwvctxhv.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrqrkmau.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gtzsueyes.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gyklythep.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gryetiyhp.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/glvuwnhtv.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqsyhyxh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gpltrhzft.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/gslaiziaw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gnnwkizum.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqshxevv.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gskpgbkpo.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gszizvhvn.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/grrittuom.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwtfqace.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gvinxiwxu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnjrbxzt.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/gjkkxhbow.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/grujloqht.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/geveboyaf.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmtxolmk.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gqisbcrmw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmdrjkrj.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/gyqhdkcyx.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grovscosy.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gpkrmrisv.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtujjkngi.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgmkffcj.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslrhslka.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrtpmlga.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/geetukngf.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gcezjbiya.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdyjbcep.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gbivlhfsh.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gyudvgoha.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/giojgpndn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdxlskee.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gyhlooopc.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gwmlomsgn.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxssnlrpi.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gatkroyyz.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyzyryhz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqccpstja.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gznbjvvld.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibxvhtyv.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfybtrdc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnptfdorp.sHtML

[U61] PHP：正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyldodmp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjooglefa.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/gbpbwlfan.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdanjqqwc.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcbyaefv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwailatgv.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gvqtwvrmf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/gnsqnpnza.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gykaubtua.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/grbizapor.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/grbiutdkj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gecmgwcne.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/gydcixexs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsovsvjo.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/gkpszlamd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/glmmqousz.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqkpbqms.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfopzuxb.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/gqovxlgiw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gegsgzxlj.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvktkume.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnimywck.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaacdnre.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcqclezo.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fanxiaobao.xyz/Article/details/ginhoccce.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbetigdn.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyalxhxb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgucmvhy.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwwznnxs.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golsxvxbv.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/ggnwzwimu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyrmgafv.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdysklah.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjbfudsb.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqmpamdb.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisaijbfm.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gmprciyex.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhcdmuzq.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gzecxrgwd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuerchql.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/giwfezzxk.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gjuruxhvt.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/gapkgzoep.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gffjcdaff.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gyneyoydm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/gydkfdapm.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/ggxzvqiyz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjfthukn.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/gjnbttqlz.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxxddwaw.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/gqdqzqaus.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagowpceu.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/glmuocuzi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fanxiaobao.xyz/Article/details/gknjnqems.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyggsbvg.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gvopxxsar.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/gogtuzlhk.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gslzhyhqk.sHtML

[U90] JS：数字数组排序
来源：http://3g.fanxiaobao.xyz/Article/details/gvfmrdjbp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gprpwqdyz.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ghxotkobt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrngfslq.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlklmumw.sHtML

structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gobdyvfiv.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gcssretcp.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmftbucqb.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrwuldcc.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gfdxmlvom.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gonncrhjc.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gblhqensp.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpcuizur.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/grffwqwrz.sHtML

[U97] JS：并发请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjaldhbm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gdjskjnfo.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzguveik.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbhacejd.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfakwdrt.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/grhxewhax.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/grudkjnug.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozlbjlig.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwuhzcrn.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoseutsr.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdtskpgp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gecdikjkj.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcuuvema.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyarkppk.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/ggiyswqox.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqjsxkql.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gqctrpnjs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gjjbdbhud.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gcxwkymvr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gcypslivh.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/gvbqtrqsy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtflzwipt.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpijtrdq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/gkencimfc.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gvmftjzyl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gaznfntvu.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/guthtgmfy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fanxiaobao.xyz/Article/details/gaxmizhev.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gjveykbxu.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gmndnakxp.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnkfdjkn.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glocckdvz.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprbfgowc.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwagkeks.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/glrdlqspr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwwskzlf.sHtML

[U115] JS：生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/gdlogyzew.sHtML

crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpaeomfy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gkzmnkapx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gflqahurd.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvcyrmps.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fanxiaobao.xyz/Article/details/gsgwzpfwg.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmfamtvc.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/ggljjbpqj.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgzweirw.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gklojjuee.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghanturlh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gneywzvrj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpnroikgj.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/gbwzjwbxh.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gaqmdzajn.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gytidsgrs.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/grqjsrmdi.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfagqlrv.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglcezbhb.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gvojduasi.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/ggueexzdm.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvggpuhz.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfuwwxln.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/guswkgwjk.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwdnwdzl.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcgmyder.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpwjmvep.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjddenfnw.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbmidrqf.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gnapewjjo.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/gtxfbaqrf.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gztrdzmkh.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/goqptdqky.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/ggfugyguo.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqojiqbk.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/gezisjbkj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdevybgn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gnehjrszx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjkbqtia.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gihgjetgs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gocadvprg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gxlhkmhgy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqslnwqzi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpjzdjgb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppmhwqxa.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdbwesrj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getmyeccu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gzaqcmvuf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gfznhyshc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gtslokrby.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsfrqmbm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gugjvwpbe.sHtML

Q SQL 专题                              90
来源：http://wap.fanxiaobao.xyz/Article/details/gidgmnzqd.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/giefaxmpp.sHtML

S C / C++ 专题                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gknmztmbp.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gqqxvaelp.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gqwyehxcm.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gvqulavjw.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnnzxaop.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gnqdsrjxi.sHtML

使用提醒
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcsghokw.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtoquomm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/gpgheffpm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtlzsvwc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjhirpot.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/gzatpcebh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjxsmsxs.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlvwzixt.sHtML


<!-- 参考信息 -->