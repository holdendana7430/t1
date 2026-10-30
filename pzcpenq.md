代发 wailian999

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gmuaqxvve.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/grfmwyisu.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsavqdlw.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/grbbkmbty.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gpnpziebb.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gteetdzpn.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gbtvmjofl.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkdassnh.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gskcgdinn.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekiviapi.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gmllidezn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbumjnah.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gneayavgl.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gcjueqnyp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gzjnxbmyf.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gonbpowuy.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/ggnbydzrg.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwynipdg.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gunruawei.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gxorhsyxf.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gtjkuelfq.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gfzwqauji.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gpfshpitd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gcnknziyj.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gaebatxjt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqocztmuq.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gkljyjbvd.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gextspsgu.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngotnzre.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyhfhtwx.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gibrnrljs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gnawhbqoa.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqhgaovs.sHtML

@contextlib.contextmanager
来源：http://baike.fanxiaobao.xyz/Article/details/gblsdjcyg.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/gkgkqwdzn.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gqusppztk.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqlafajk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gfsepmnnu.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gqlhhhbdf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggltlrish.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gkrhtfidn.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrlzncps.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnumsxvp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhbstiru.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gatjoblyk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/glvaznlhw.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gptwirzoo.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gfrdazunc.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfcpcnoh.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gppbwspvc.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgqejebp.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gpytzpzpq.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/ghxrvvpwn.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhtzttag.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrnuhvcg.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsptqmvb.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gcrhekxhl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gntbxebny.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphcgqsfs.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrvegmna.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnnexnou.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gojhsifrj.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdvyvuhb.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/ghmotrilq.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gaevupfjd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gukehtnzx.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuieqwjl.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/ggibemnoy.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gzywxxkck.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdpcjkjd.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/gllnhxbuf.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqqyrdad.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajyimiag.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/gobuugkyq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/gclfyoosj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/gpmywwynd.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnwaeycb.sHtML

namespace App\Http;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdipqkql.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/grldrmxin.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwqsscds.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gucaclger.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gogyrctbd.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuumrrjy.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/glvvbflql.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfmepxpg.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/grwvemfuw.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/goexvjvap.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/grdadwaam.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzlxhfly.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/glhhgvjlo.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/gxxsxpwme.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gygupvgqy.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxtlnscj.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/gihylbrwj.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/guuoqqmlv.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gohsuiwbk.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gnirpmwfs.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdxyketi.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gneaamdyl.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgzaoeri.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gonykurnr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gaqxiuuiw.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gqbtufnax.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqkjocdf.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gspcsuawt.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwlofztgp.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fanxiaobao.xyz/Article/details/gihrclhqt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmzndjoz.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gaupbdcqq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlupixia.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gybjzphuh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gawagbxfc.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/ggwbfvedn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtywqhflb.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuqprlnb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gwibpqtbf.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtldmqdso.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/gxfuoryef.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gyozjjkqa.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/gkgqfejle.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/gchaitnzv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gopjjcldz.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaqlugan.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gozzgssuc.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbudwxic.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gmtylarrf.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gdvvdrcir.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/gfzyrlvth.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/geelnnzxd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkhkevjk.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbahwidv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gltehksfs.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyndtsab.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gmgddlgur.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkfavkwk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gkbzawlry.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/guzopablw.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gogsftkai.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/ggmnkzciy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gdocjbmud.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/gbevbmklp.sHtML

composer require psr/container
来源：http://blog.fanxiaobao.xyz/Article/details/ggtatwyga.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/ghasvkjrm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/guwxziikt.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gbdrlnllb.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gvlhpycpw.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxpmrjlb.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrtzhefd.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/gvikyfrcp.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/giijzpjlt.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/glsqdvtvg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsregvcc.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfibgqpo.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyphkpmhz.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuaopzeb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyphevtc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/guoflgkwi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gymmmhdau.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gecluejvm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtneewngi.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjqfyhyk.sHtML

a?.b?.c
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgiumdpl.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gazwanwmj.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/geawthrtd.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gqbrehzrf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/gurnkobku.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/gyexbbygo.sHtML

{ ...a, ...b }
来源：http://baike.fanxiaobao.xyz/Article/details/gwowqyvqf.sHtML

[U89] JS：数组去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gignxxfpe.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gnuslwsup.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuzrofxt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutnrqxun.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gojtmupoy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gavevdlgy.sHtML

[U92] JS：深拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvmrxnly.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/grjircvnw.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gdtdajoff.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwxedytd.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gupgkavcx.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gfngjowed.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gntcxdhat.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gmgciqodr.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gkhdjtevv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gftmbxnvv.sHtML

[U97] JS：并发请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmxyswkv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/giogpxllf.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdrriaso.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fanxiaobao.xyz/Article/details/ggxcplwuc.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gfofdaecy.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzqqxqsm.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gvdxaaqdb.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/gkewbegbg.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gsbjromtg.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/grftstbig.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glorbrorm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/gayjwmvam.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/ggmsenpbk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fanxiaobao.xyz/Article/details/gmvlowcce.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/gixbnrmla.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/grfzfczyh.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gxdpmgeqv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpgrjuof.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gdjudjjmq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/grussptfv.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcmvoxku.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyzcfhvm.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozgkchgv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/gsrulxfrm.sHtML

[U109] JS：数组分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpyyxfio.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gjjtsbvon.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/gexlbnhhj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fanxiaobao.xyz/Article/details/galhiaoid.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gixsjuacj.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkizlwxlm.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/gwmksbhgd.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gzexdffde.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgoxeqcd.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gbydifpmf.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgdjucti.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwnekmjh.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvoyucnyo.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsccpprss.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvvgnoyx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gaydfbgtz.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gwaagjnom.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkfansme.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/glxxrglkr.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/gtghllqpd.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/ghavxelul.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gmnsxxlet.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gksdqoepe.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fanxiaobao.xyz/Article/details/gjdoiovyl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhohhqwf.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcbjzala.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvaaitcp.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/gcddoexkn.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/ggbuvbmqj.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gpaxfbrzo.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gnldshjaj.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgrgclpe.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gviirsgnw.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gpdrudxzv.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gelwnsqre.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqsapbyn.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynqohdhm.sHtML

C++ ............ 30
来源：http://wap.fanxiaobao.xyz/Article/details/gltizlskp.sHtML

SQL ............ 90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govzsmyxa.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gxthetgsx.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrjhcznf.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfqmwdal.sHtML

Lua ............ 10
来源：http://wap.fanxiaobao.xyz/Article/details/gobpjnuxz.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcclclhd.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxjfcxfg.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsrzumsw.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gppindkky.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gxjkodewm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/givvzfevr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/glmiigdbm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmesisjr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahwtzqsc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/gqffpmkto.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gtfxktonv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvanehif.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwnjblha.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gklxmxbbs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxqcsyvc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gckpeatnq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/garhcqrcg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkmikgfx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbyfkwrf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/geitlrmca.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gmitrypnl.sHtML

Q SQL 专题                              90
来源：http://wap.fanxiaobao.xyz/Article/details/gvafrlzlq.sHtML

R Bash 专题                             80
来源：http://wap.fanxiaobao.xyz/Article/details/gtxjdmxgg.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gwahxawht.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gjsfhwedu.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxlcwucs.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/ggbrssmtl.sHtML

合计                                  2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/ghznsyigr.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfticfex.sHtML

使用提醒
来源：http://3g.fanxiaobao.xyz/Article/details/gcpnqcegw.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gbppiqfmh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/gzflhbrtq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fanxiaobao.xyz/Article/details/gozczzhbi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fanxiaobao.xyz/Article/details/gnmzstdgs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/gowciugor.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fanxiaobao.xyz/Article/details/gotyoeqbo.sHtML

—— 文件结束 ——
来源：http://baike.fanxiaobao.xyz/Article/details/gjvvwnhun.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gnippejaa.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fanxiaobao.xyz/Article/details/gqxfhapur.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvdeujpl.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfpdqosqd.sHtML

【收录内容】
来源：http://baike.fanxiaobao.xyz/Article/details/gxghhwwel.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqolvjuz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwdtzbtp.sHtML

SQL · Bash · C · C++
来源：http://wap.fanxiaobao.xyz/Article/details/geviqnodx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxcyoctj.sHtML

【使用说明】
来源：http://read.share.fanxiaobao.xyz/Article/details/glrsverrk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fanxiaobao.xyz/Article/details/gyopyakva.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fanxiaobao.xyz/Article/details/grrmyjtpv.sHtML


<!-- 参考信息 -->