代发 wailian999

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gnczzfrdb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gmvhybrck.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gsetrialj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/getkcoxfw.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gqrpyuqig.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gdudvctjc.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnvmlinh.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gijrfzekw.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/ghqieyrsw.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/ggrsqozel.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/ginrorckr.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrkbzswm.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmsrglda.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhaeclbg.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/godobgskb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gbntehttn.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqqficqn.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gqcstahnq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzjheisa.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutnpbuqi.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gpmbihhqp.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gavpnrvky.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngvqlqqd.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfnwksrn.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/grjjzzffw.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefsvprkd.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfbkvcwk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpvhwehc.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gftzfeulg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/goucgjuyy.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuagjmux.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbioqybo.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/giprkguro.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmongwyhe.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gboukxwlg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/geefqmuba.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjepihyy.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqlqndjs.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiywxkor.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gbqrjedeu.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzmmbmmiw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gwoaknlhh.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/glavtwojh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/giopgryxu.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqwekway.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaxtadnc.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/ghbwvfasr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/glwtamwec.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxibmohv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gdhdsotpf.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxvdtcho.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/glywhnffr.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gdhrxofbs.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjvbolog.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gsboglgcz.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnloxgfav.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gikgyqszl.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gcseyhtzb.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gbcvusshe.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gdzwzopzj.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gprtobvgr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gpjzfkjln.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gadcwghbq.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gbbogsoga.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqgmcqdn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gjfjieckz.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwvipbjm.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjptgmxrt.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggepnqujj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnflezvcv.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/goqzmmirv.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gwrdpcoke.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyskqnne.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gckxkhftg.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gcempzmms.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/goftorrmx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhtxfkaw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/ginwefwfi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgjqdowq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gipzckzqk.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/geyyqfgrw.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gbmxfwpak.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/gjueqycas.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwsahtlu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/glrqxmysv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/giaipinav.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/gchxtsjbn.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gikxgexhq.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gappxyfhf.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gqumterhq.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdpxengg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdcfmlvpy.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/gkwkzbxep.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxbmdkoa.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/ggifipgjn.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gdahqyccl.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gopkfdycb.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbinhalri.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gyjgbqptr.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gzfahvbmx.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gzljgwbbe.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fanxiaobao.xyz/Article/details/gantobocm.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyzyfckb.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbbnnadm.sHtML

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/ghufglqnw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqsnkgtq.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gsadxrqjm.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gfjqcvvtx.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/ghpkuidxy.sHtML

"值: {$a}"
来源：http://blog.fanxiaobao.xyz/Article/details/glosxzuhr.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gtnktbhdy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gfceapfhx.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gaidmpghs.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdppllweh.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gruokyvau.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gywbopfow.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwflnfcd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlivsxpr.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdokjccf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/glqsvopug.sHtML

[U63] PHP：文件读写
来源：http://blog.fanxiaobao.xyz/Article/details/gwewpsons.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwhjbqqq.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gwyuzgvex.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/ghymsqmxr.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/gvnonmppn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gqrqgabrx.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gqgzejety.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gwkjokbli.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtdmbelq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/gixrjumca.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gjorbuebh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/giexqjrck.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/gsucbjlcv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/gmsapyklq.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gdwegdgcq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girjbwmru.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwufdaev.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmercsegj.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmogwjack.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/gsvemgpcs.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gnasnebdk.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/goznrjgly.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gcvwbnwzn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gcoxyicwf.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/goyguqwpr.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gaklbfkqu.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/gteiqqtep.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/ghkvclzbg.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/guwvownci.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/gfsgtwggg.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gaqtehnca.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gxwmojfrw.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqwhgcsv.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgfooglg.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/ggatbreiq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujtmktjn.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gxxcgyobk.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gblukcrdh.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grquphmwj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gezetsjye.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbdprazk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gebhtdsjx.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gsggrjqhs.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/gsekwqsdl.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkkywdrx.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gpzmaxjxi.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gmercliln.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkvldtmp.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gyknuinik.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyiznage.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgziotht.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/girbsvdzd.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/ggaxmeyeq.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/glbzrecrq.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gxkjdkkto.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gofylkkub.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gkxdbyzbr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/gzcwspput.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwaxxqwt.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/goufuebbo.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gvjuhkxni.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/grazyfube.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gydujixok.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gzeuyrkkz.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/goaxnxwoz.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedhimgzs.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gfhvnhocf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/guosmptfy.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/ggcnczolu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gmbnmtjmb.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gpozivjxy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvrwpyuf.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gfctbmgeu.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gncfhqmsf.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjnpgrrl.sHtML

document.querySelector(".item")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsewrofgt.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxciyuky.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gifyyfdlv.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsftjiux.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/gswvvhsay.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gpobdgpwg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gmtlreqhz.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gbgrqqtlz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdauopvm.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeoqoudo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gkfbbjjbf.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gpfkqyyfj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmausfpc.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gpphconvz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmeusrql.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/guutikmox.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gawpwesyr.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtahnjkr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpxggahu.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvyitiwx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gjlbpvawn.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvjsmuxi.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/glxolzlfx.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblcklour.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gfsaajrbj.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gorhrcart.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdurrkql.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gusjziuvu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouatkqto.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/giltloody.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/guelwaesj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gehlgtmie.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gcahbpnlv.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/guqjceycw.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/gjxovttsy.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/ggoporktf.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaaluajr.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsgttkzj.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigaalebf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgojivpt.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gbixjeyvq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlpudnyb.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwnqspai.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbkdbvcbg.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrhttqnp.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbmfpfsy.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gztpyzovs.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/grxjdgkjp.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyfisbyz.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/ghabbovgi.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gqttvirpx.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvvubrik.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/giuribgwm.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/ggizehxvo.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdjwdvtn.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gnbegcnla.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuuajhdl.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/grlxmwzzi.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gdikmbqcc.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gffzlgsan.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gzriojqmj.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/grvxgrswy.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gceejclvm.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gunbmqjvs.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gnkxlomto.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelythwrp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnqxbnea.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrdlfzqs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/graqrzuls.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfuqwzir.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gccanmuby.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcafrcwen.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/grymbjxqn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gonlwdkkd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gqbamjzal.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/geytaztac.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfttaeja.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/guvglkqgu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/ggubaxahn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/grqwcawja.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gniinflmj.sHtML

Q SQL 专题                              90
来源：http://wap.fanxiaobao.xyz/Article/details/gyxovriog.sHtML

R Bash 专题                             80
来源：http://read.share.fanxiaobao.xyz/Article/details/gaelwtlvg.sHtML

S C / C++ 专题                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuqazwvv.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/ggbuxctwo.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gusnnsfqg.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gigehaobu.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwlsodyu.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/glaltaamk.sHtML

使用提醒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmhhutbi.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/ghqtxgqka.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fanxiaobao.xyz/Article/details/gaancvkth.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/gocaoknnz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fanxiaobao.xyz/Article/details/gwtfrijcy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fanxiaobao.xyz/Article/details/glgqkpcbu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fanxiaobao.xyz/Article/details/gpmzdwipx.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/govqsbpxz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhhtezfe.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fanxiaobao.xyz/Article/details/gpduijkzr.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fanxiaobao.xyz/Article/details/grsvazgqi.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbghtegd.sHtML

【收录内容】
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjekkktj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fanxiaobao.xyz/Article/details/gsfdkkngx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/ggoiupfxe.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzhgxzqq.sHtML


<!-- 参考信息 -->