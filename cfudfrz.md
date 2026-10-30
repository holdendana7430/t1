代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtdqyzix.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gznbvdktz.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gkrhfyxna.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxjwenmc.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gtpdvhysa.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gyjcztnnt.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtpldgzt.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoklwtno.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gqyetpkxk.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gqidhgrqu.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gesuywszv.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/ghipztabs.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/ghebbkxac.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/geslzjqpk.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gpsndbxxe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcczrxyg.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gvfdyradh.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiyyienn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/grfotvnbg.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdelourfk.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gghgeltgi.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gkxpleaky.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggroeilpg.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gsxkhywgj.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gxeogvxzh.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/ghqcfwmui.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/goykpdbps.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyawecydl.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gypyjfdad.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gvcjzidht.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gwiecqpmq.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcglyeizi.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwctbeeg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gtvbxzqfh.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gjvhzrmyg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/glijvmetl.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gegwzpfoy.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gusygxyof.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gpgaolzdk.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gutzafwfx.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/geblznkiw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gthdeujgs.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcshdckf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/glixycqro.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfielkbm.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gjavghuwc.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmqobxbt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzcnpwkl.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/greufybog.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gbpsuexwu.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gsocoynde.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gjacblbim.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gjuiwonde.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/gniwuemoa.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gbhbruxuk.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqlkgmzr.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdjfuuwq.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfhkwvzs.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzmwmidf.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/gpyflfdhs.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/glcmjojjh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpzsirck.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/gxlikkmgr.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gklghjmps.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/ghhuhulwr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbbkkcjr.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gelemvgyu.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gqqvyvxlc.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqmlkcne.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gtilzhbrk.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudfqondp.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzylzwwxk.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gkvplwrmu.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcdudcil.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwxywrjf.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gttywhwmo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/glwotvona.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fanxiaobao.xyz/Article/details/gvjhnhksk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/guwqarcml.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/gfswynbxq.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdarmuwo.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlcyvrxz.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gizziyrxf.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazleqqpc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gusxawhnf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhxmwxpy.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjxsofhz.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/gyvfinoej.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaavmcyxn.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqacpxwa.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gvswdivfe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gelbrqqtf.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/gwmqcgjxg.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/ghetrncvb.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gznnkgyvx.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/golkrrwrw.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaekxhsop.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkifnxwsq.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgvixpny.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbndltywe.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfclowpk.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/garrouufx.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gvztmzyox.sHtML

$obj?->method()
来源：http://www.blog.fanxiaobao.xyz/Article/details/goragguok.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gcigrtcsg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gllkmpmha.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypfhfxcx.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/godaqcwkg.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/ggquosywc.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhvpcbum.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsknnzawn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/grmixcbaf.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbhgxowb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdifeabe.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/goybmgjbn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/grkcoxkrh.sHtML

[U61] PHP：正则
来源：http://blog.fanxiaobao.xyz/Article/details/glvjrqzom.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyrfqqyc.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/gwmfbtppw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkhckqew.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdoijhss.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/gbeubjkmb.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gfvhbxjxf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/girjkwyps.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxwomqle.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqzhnxye.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gbunlvcug.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/givqdohuu.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemsckygn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/gwmvgioik.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/gpowiunum.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gwidkkrnl.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fanxiaobao.xyz/Article/details/gbyzglzte.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmqqmayd.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/gdlxhtpaa.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/gytpbkbhm.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gfaambhub.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdbumbzc.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfayiuuw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/gbzkbtdvo.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gualsjoap.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwvueupu.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gklaruqev.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fanxiaobao.xyz/Article/details/gjzbphdim.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtrhnvnw.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhgyryjx.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gswtgmxwl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/gxrfxtwgz.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gvuytklxy.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkkqlujw.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gumlsugyp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncqxtyjy.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gllywjddl.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fanxiaobao.xyz/Article/details/grparwkne.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcweifhr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgwlduht.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gpoervsht.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gndrafxdj.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gswplhzte.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gtaxqbqjl.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gijpkcbyr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/ggehhjzju.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fanxiaobao.xyz/Article/details/gdcmxcqak.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fanxiaobao.xyz/Article/details/gomdssrky.sHtML

[U85] JS：可选链
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuzusclm.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/grffydoff.sHtML

[U86] JS：空值合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gazojqfnl.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/gyadfqlma.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlhmawie.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gjagueolv.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/gwvlmfccy.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gliiiilys.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbdgqylm.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gnymrvbfa.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gguymrdqv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrzfoiob.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gjcoaojpq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gmkuajobu.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gtiamiwlz.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/glxpsfkme.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gftrlsgwm.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjdlfquv.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/grkpscjiw.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gyjfzzfqg.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/godoftlqn.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpmqpijd.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gbfroerpa.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gbsgqtasf.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvuymktn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gzhqucgvh.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbtzgtmr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjbesbfs.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gynyfzwet.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrwunulc.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhfsmgxt.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/gyadsfnld.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/gegvuyrja.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxmtawhq.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gymqxklek.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcghwynq.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/ggwxmjxrt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gtvyozhwv.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnashijt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/ghbkadpoh.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gglvrakpi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gtsvudcmv.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdmuzxvu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gxhfwkvhp.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gtxngemis.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjeiycoyg.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrjhlpgs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gezlyeznu.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gwmhquvdj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gfsmkwvch.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/gixwjhfrr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaijvjvbf.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gaqqjpvvg.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gvlwlzylq.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gowclvovr.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmqpsaua.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/guvyuokvk.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gztzseujm.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgswgite.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqwlmfhv.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswwioogh.sHtML

crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrhjrhaf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/gptrcrnkv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmserpam.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gsvyrocex.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/geskjvzvi.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewlngpkc.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gbizjdons.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnlhytdc.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gyjsulfba.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gpxrtppvg.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/grvbepjnm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvqkdeyf.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gpclxfusn.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gthefrwbg.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/gufohzbka.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gvfksqpct.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwhajpzx.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/glavksbqb.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvekjppc.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gduxagmbb.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gsttdfyrl.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdjfbulw.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gknaajuks.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtelcins.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gfeizgeqb.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gilsixgpo.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbwtdifu.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiwamoxe.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnofklhm.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfrolbue.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gdodkfsmh.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gbqojdyly.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbfhxuwd.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geecswjmo.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdlowsxf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/glvsjmjsl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gdojhxfjh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gikhbayco.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gqjdhlncp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/gkmdnnnfm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gtledhdhf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeilacou.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gdygpkfmn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/ganjrvyke.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkiwxinh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpitmroc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gvszadnnz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gttoqagmw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gcnekxkyb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/gfbedejxu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjvjbwpu.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/gefysmsyx.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/glzggtcls.sHtML

S C / C++ 专题                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gwghbfzbl.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gkzuvpeqe.sHtML

U 高频实用片段                         120
来源：http://wap.fanxiaobao.xyz/Article/details/gdlusfcnw.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gfvmjosbf.sHtML

合计                                  2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grczeylhm.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gwubfsvst.sHtML

使用提醒
来源：http://3g.fanxiaobao.xyz/Article/details/gazqhzdvm.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gjdeykezk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfwyjdrl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsldlwwp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fanxiaobao.xyz/Article/details/grhnyiocu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgfkpyqe.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginjfjpix.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtnpjqft.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gosspsvji.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fanxiaobao.xyz/Article/details/gipoodhhl.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fanxiaobao.xyz/Article/details/gtbxdwgvf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpvdcidko.sHtML

【收录内容】
来源：http://wap.fanxiaobao.xyz/Article/details/gtkrlpclz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/gabmrsygn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnnxjmrs.sHtML

SQL · Bash · C · C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbrmoixk.sHtML


<!-- 参考信息 -->