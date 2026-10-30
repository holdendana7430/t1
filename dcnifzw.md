代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqreuahlx.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gdozxagtc.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gsljzzjld.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gblcamcad.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavklfmjo.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqokdbfm.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkmssbfl.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gorqfcwlx.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gerkigsxk.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/grmurapen.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gvubxmdae.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjemlqrw.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvbypiox.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gtrlclutm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gfjufiasp.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gcnljkaap.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxsembam.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwoyvadk.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohwtuosn.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrpcocfy.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrkfsvbv.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/golgqgayw.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gvgjyjtle.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoprwbwe.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gflmejarg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/grvuzshyd.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/giedwmund.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gfowotuwk.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gdbmxivgt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpnpxfog.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gmfunwifd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gqhwbeeea.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcttdduu.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/geqsaaqtv.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gxdbllhgg.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gcgvvnjtd.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzsfuzcud.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gnumtcdzo.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gzjcwqhld.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddfcrczc.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/govgbrvwf.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gthlnrdxe.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgxxgnvi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gkudwanwi.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdetbnwkx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gcrzeyihn.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/guqucprrs.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaeuhebb.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszspsowk.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhxjfpdt.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/giofcupkx.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gldbjzodc.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiejaxqi.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/giuampwbz.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgazgkin.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gojysmeib.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxjzfqco.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpfbyvga.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdtqfbfy.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmsppkll.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwaheefq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/glpwyqoac.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gxdzonrwk.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbynlvihe.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/gcbwxxyog.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqbydmag.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgcbrphj.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcmdlisx.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzpywdaa.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufepobbp.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdsmfzaq.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gwuembtdd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/gbnfxjmyo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnajevrk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/glfqldauq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gugrjnwen.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gwgyexoyz.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtblffqpq.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gzgzsnxht.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/glqqecupj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbytmfni.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljongktw.sHtML

[U46] PHP：可空类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmwdwhie.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmlgbenj.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/gttzmyqth.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gkbrngwar.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/glfrxfgyg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gecixdgkh.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyndsloc.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gbdqjlban.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/gfaloyzht.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgtwdazt.sHtML

[U51] PHP：数组解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gqavovafh.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gsrlcqela.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruxhwzdo.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntitehhr.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/gpmsqjrob.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fanxiaobao.xyz/Article/details/guupjxbwz.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/gckawltim.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/gaycecqhq.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gtchrvdbp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhemzccs.sHtML

[U56] PHP：命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuazbkao.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gptntxhtq.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkskmhah.sHtML

"值: {$a}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfigepeb.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnnfaosf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gorujojsi.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotybdqvp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrhixgaf.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fanxiaobao.xyz/Article/details/ghfpjrtru.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gzmltnvrs.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/glkvvepvw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gtdkrajxf.sHtML

[U62] PHP：日期对象
来源：http://wap.fanxiaobao.xyz/Article/details/grcvwllzq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gaotskhgu.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gidzntysr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gbfxcedez.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/geyshslrx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfjapgrh.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/gvsxzjpwn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gawylknnv.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gkhnsqrxa.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaetkdey.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gqowsczeg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuusirko.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/grkuvfvjo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/gehvjwgyg.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fanxiaobao.xyz/Article/details/gdrfvwost.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsuceibs.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkjyiiwe.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/gygaaxviz.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcavqvsb.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gwvpcjxce.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/goteoudtn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvmeapfe.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gkhooaemi.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gpwoterqa.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxidnulg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gkmsbtrfs.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorrhwiim.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumsodwzg.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gkctgjygl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/gufoqxcaq.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/goqgkmyiz.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gtwbllxup.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnaobxld.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmzytlcl.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gxnrokpwz.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxgytrrf.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhuicasc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/gkonpxuxu.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/giiirobzf.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gejywsuil.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxsmddmy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxwxjkmu.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gslfypmds.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gaiuxyrqf.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/gjnizhtqu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fanxiaobao.xyz/Article/details/ggwskbsvc.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gkstokcvk.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojlkjhcp.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfwvmgdz.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/glpjpmdic.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/guthvmjvo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/grvaycpyn.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/gcmwpqgco.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/glfeqkgrm.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gmtvhshdh.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumloduon.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzdtzktt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gffyvbzwj.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmpchcma.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgipdkea.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gvpwybday.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaduheqp.sHtML

[U93] JS：模板字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlqbjspe.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/gearddpdl.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhsshote.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gkbvapmzr.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gnxyicpop.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gdvbhrhdu.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gauhwlewo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjzkcfxn.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gmcaeuopj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcusecke.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gwqqfqjht.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/gbhlbtole.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgdimpez.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gmnzeurhm.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnudpfye.sHtML

document.querySelector(".item")
来源：http://wap.fanxiaobao.xyz/Article/details/gjiwpgfwu.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gjyklskyr.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/gowfkqadd.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjceitsmc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgqkrrxa.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/gxpxhkcsh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fanxiaobao.xyz/Article/details/gwdnfmina.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/grklnunip.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gdwdzodbk.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxkscfux.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/guavyxxsm.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafpswufp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gicypsfvc.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpehdmss.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/gdoacblxe.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/goeoxvkqw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/gsohycbnz.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gontbecyh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpoowkqq.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/gusqvnpow.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtoxdgku.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmaplxhn.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/grqdthsxk.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gdczadxbk.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkthaate.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/gjjbsgmpb.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gnsgpatdh.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gvksqomxf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/grfrdfzvc.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbmdsxxd.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdrhropr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/giyoelfgn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gcmcyzvrh.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gniegukdp.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gailxrmox.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/goisdjphj.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkgcpujr.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gaqeutlqy.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gvzfsvlmt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gesxwtbvs.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fanxiaobao.xyz/Article/details/gmruabrtn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghprbkluu.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gsdnmbwkp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbsplkdr.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzhdjcrx.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/goghqchgg.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gzlzgrjqi.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gofehlzuo.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkocpunhq.sHtML

Java ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gvhahjmgc.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gbmxyjzes.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzxpsqdf.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqbhileq.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/gncvxvapk.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfkftyxi.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqetmxra.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitbatupg.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmxdwqvi.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmpltfye.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcdqswlo.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjbnpnpl.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlzkuccd.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxvetrhd.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrvghwez.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/gzytiozlc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypffgupv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gqizvveec.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gtzawsbkx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkeiossn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/ggugtsjcu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmagdhogd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveliwwyu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gotcxcblv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuqdffty.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gsvatotpm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmmyutva.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gkdsqsgto.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwvsaqma.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvjasjhe.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/gwfxwhskc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gzosomedc.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/gbeteojka.sHtML

R Bash 专题                             80
来源：http://www.share.fanxiaobao.xyz/Article/details/gcygrnyqr.sHtML

S C / C++ 专题                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gmiwkqbor.sHtML

T 其他语言补充                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gcaxdfnpg.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddmqzuzx.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gpinmpkwr.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gjivsgprm.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gttzewvkp.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/gskioxlkm.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gsayvtbjk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozhdjlro.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fanxiaobao.xyz/Article/details/glypxgebi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjlsoiwd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrgvoyoz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjftndrzb.sHtML

—— 文件结束 ——
来源：http://3g.fanxiaobao.xyz/Article/details/gjorxwrjc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkythwcl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggprjplyp.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fanxiaobao.xyz/Article/details/gccerroob.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gsllyzbns.sHtML

【收录内容】
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzdnystb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fanxiaobao.xyz/Article/details/gobpteint.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/glhcqyaad.sHtML

SQL · Bash · C · C++
来源：http://blog.fanxiaobao.xyz/Article/details/gvhyvbuka.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fanxiaobao.xyz/Article/details/gvayxxvis.sHtML

【使用说明】
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvqtizfa.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqyetfqb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fanxiaobao.xyz/Article/details/gluapkbnu.sHtML


<!-- 参考信息 -->