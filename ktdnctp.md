代发 wailian999

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gcecawzpc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/ghcdlnqye.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gzmoyvezl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gjwhbustb.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gtpsffrol.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gocepbmqk.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gvckhzvim.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gkmxqqyiz.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gybcjzdmn.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gfsmqkytu.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gwscachrk.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/grxbpdiii.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gxigbtyjb.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gejskpugv.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gejonhunz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/grmfirsqo.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gpqbdeaey.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gjpnsixcw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/gtllrxqhc.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/ghqysyqrl.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/ghqhvzbkq.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/gaipdnwus.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/ghpffolun.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gvaujdduy.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gesuegxts.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/ghsxxabsb.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/glcjcqjsz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gteyvqgma.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/giymoqmze.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gaxzpvtsi.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gdfjfmrzj.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gattqtcwo.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gidmudxmo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gyrsiqkfl.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gcasyqgvt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gyornmure.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gatdujwcn.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gvzihzaxw.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gmpjxgpyt.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gijkymzmr.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/goywutlex.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gyybdbajq.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/gwnimgwcy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gsxsrspuf.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gufllxizk.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gcnmtzyli.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gdigpbdzm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/giaxoeluy.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gbncqzefd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gupgyqjor.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gakuhcprf.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/giijjqrmh.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gdbzkqmkx.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gnfrjpumi.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/gyucutvzh.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gvlqamfia.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/ghvgnsjjk.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gfkalkuxp.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gkvlpmuml.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gdzuhmbcf.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gvngwxmnm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gbtvgxncb.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/guwycqlcl.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gnjvdmpyr.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gwftfbcol.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwhiabky.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/giuzrdeit.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/girdtyqrq.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gnotdughq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gkavqmiek.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/glwwkivxo.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gskqekqvg.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gmrhetymh.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gxvsnemnn.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/giyeyzehl.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gwxwchjeq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/grqbgzamk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gbmmblklc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gxuskswmk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gsqcjiqlx.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gvhrspfxy.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/grebnkhsx.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/ggxtgysmi.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gxtpphlpo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/glvldjkwi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gbpxjbwlr.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gwvudzcau.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gpbxpjsvf.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gdaqrexti.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gcpgiuwxe.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gwkvbnspr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gvzbdzyyx.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gpxsjmsio.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gmsoxncuv.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gwaqdxcxc.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gjfwldihw.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gtpzmzbth.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gxsrwyxxg.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/grwjfhfog.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gmivugrpk.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gegrwpslv.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gmydzvekn.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gzpbvpurk.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gnkbsehid.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/gaobkmixr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gimypxtlj.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/gjqzauhhs.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gcyumgtmr.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gyoxrwxoz.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gvkkleapk.sHtML

[U58] PHP：数组三件套
来源：http://baike.hesvh.cn/Article/details/gwcevxulm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gryukstwe.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gyhlcevzg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gnogatzpc.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gmvvemjwp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gcrqznfsa.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/grnriupat.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gmwvaablz.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gptbchguv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gojllbwlr.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/glmkcicjx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gndcyvbmv.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gncgiidmv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gqdlzkkbw.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gsepoinfy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gkjxrkrjs.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/goojfieud.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gmjqlufbg.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fehbvm.com/Article/details/gjkbusprk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gapgvchjq.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gpjiicdln.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gptnqfipp.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/glwjbqnqq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gtlbaaznh.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gqhhwndcp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gkcwbsjab.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/govqlomsy.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gotyrmbjf.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gtchxhigp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gsyautums.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gcbsslteg.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gaxsnxdud.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gkvuppmal.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gecdbvbww.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/gsnmszbor.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gktvexbku.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gpxavsqry.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gaxmlzzrp.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gezcnzreh.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gjsdpniap.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/ghyjdqiwz.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gnudbecxh.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/gmesrvkik.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gaekyboro.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gihxdpxqn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/ggpnsrvyx.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/ghhzxdahu.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gzowdifxn.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/gdgpfvcbh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/ggwxlgzep.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gvalnbryv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/glbnpfsfn.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/ggyhcjnzb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gwptcmukm.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/ghqtopmko.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gjlxvtrgb.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gnqpxjdkw.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gbzjkjrcv.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/gwfwqgrcg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gfypwuphf.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/glggaplax.sHtML

{ ...a, ...b }
来源：http://blog.fehbvm.com/Article/details/gohaqfisq.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/guknkjcrr.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gdepyoics.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gfqwxhxwr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gmlcdsgxe.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gyefubtuu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gwixrcrsf.sHtML

[U92] JS：深拷贝
来源：http://3g.fehbvm.com/Article/details/gyunlysez.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gdjjrzauw.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gynfmtfgg.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gdziijzpn.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/ghdjoegdf.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gmedymlix.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gqyfqqbto.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/ggiolvtgc.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gbgrblebc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gtdoecgjk.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gyhodtybp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gqvzswagf.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/ghmlzfhgk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gckjpbhtb.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gjraqsvbz.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gkecfzfmi.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/gdtlczdum.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/gooqwcphv.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/golxkbgxr.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gztdfxpct.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gwbaadlos.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gebfvvikd.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/ghsdrolko.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/geoziunbd.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gizwtectx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/ghoegnifh.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gqgxvmsve.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/getsrsdbe.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gxehjlkhr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gjmyifdvi.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gyuvunynh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gsnkwfybt.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gkvnrwkpf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gvtqyycjt.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/gtcnkfssz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gseevwxcd.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gkglesyqf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gaqfoaguq.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gupjzyhvj.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/ghsswhwqj.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gppuomeip.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gzfoqrdoq.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/giuzavfbe.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gojmjyicr.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gfemnctsy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gqdgsprth.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gcsgcutja.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gynhthtps.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/glyliuvvy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/grroeibwv.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gfjrvfcmk.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gblnmzfvo.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/guxrphydn.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/ggshcmone.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/givovtaij.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/goirtrhyq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/gmgxdlgxe.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gyoxwwrnx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gljfvxenk.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/gzkmcgfxh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfavaalwt.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gozgegqey.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/guyihjtdx.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/grdoowxqs.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/gngepfzsi.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/gcnzzccpy.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gyppzqymt.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/grpkilmvw.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/grmivkwrs.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gpccfzpdx.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gcrrvuuvg.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/grufahxpy.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gkryuysbf.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gugdzojdo.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gjnqlkrxn.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/geiapdxei.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gnqrekosh.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/ggfmycglu.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/gjgmjonke.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gjvrqvgcw.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gszagciwl.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gawlenkne.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gtleccsnt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gzliqxkdx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gfaggeyms.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gsleabubo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gacucomfc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gohkhpcyu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gdohpfzmk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gbyyhcmpn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gfviqumnd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/golrhruvp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/ghmghrmop.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gybodafpa.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gtaxzdtfs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gonuhgqeb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gpftezowq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gziinhzbr.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gwgrfbnpb.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/ghgzzmhzb.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/giysaujed.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gxxmwpqly.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/geqnmwryq.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/graggzzgd.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/gixgjijfx.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gpaaeezcu.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gfowsmshc.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/giuagneuq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gjpzzgafn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gwbkryoet.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/gnpnnohpn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gryfaqmgt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gydgtbbuh.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/gnvthoann.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkykhjxmm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gpzmyxata.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/gupwpbxea.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gicwflebi.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/gycpijxoe.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/gvcqxnjop.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fehbvm.com/Article/details/ggzhobqow.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/ghajzquvj.sHtML


<!-- 参考信息 -->