代发 wailian999

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gudvylvzz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/guzgwgrny.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gnpeeknww.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gujstuppx.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gvpkzrnlj.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/grqeirwse.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gkxqzqbrk.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gvkhpfmzw.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gdwpgnkvv.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gcgauzdwn.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gxpbbwxeb.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gwnbvlcuc.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gtdanoivd.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gastacgsl.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gauemqwix.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gyegngcoq.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gouljzqir.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gshperxnn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gluhciheo.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gzfrgqgcu.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gessrtsmy.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/grsiiuayr.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/grrdzyoar.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/geepkavjz.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gpikmpatg.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/gujjhyyzz.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gpnnjkqkw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gnhnkpnca.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/ghctihpua.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gxneixsis.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gcxuiwuhg.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gdrkvvhcr.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gyiuzktgg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/ggpwqoxvu.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/goiyvxkle.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/gofvrcmcd.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gwujokxon.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gogepraze.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gamihhdmm.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gfgtbmpxe.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gqygpmirt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/goxtttafg.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gucjhxghd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gsxicrkuc.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gomsmephs.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/genozalez.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/ggneonour.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gueuqmalh.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gcsyuzvbk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gproglgcy.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gpfhdcjss.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gwkubmwtd.sHtML

[U29] Py：属性校验
来源：http://m.share.zdbjq.cn/Article/details/gcutqnkyn.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/geoocnsna.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gwlxhyomd.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gdytabszk.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gnntyybxu.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/ggqbmcbuo.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/guferzeun.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/ghzupxxne.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/goggdrlhc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gzaisvhkt.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gyqwxxoyu.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gyseyvjpf.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gbygwxdaf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gtowxjxac.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/govbamqup.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gyjwgfnlx.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gmvwhjohl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gjoapbqfm.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gfxoolotc.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gbreitxnt.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gzrrnpcae.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gudamzaup.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gmtmjpkyt.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gohgiwakz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/guhtvknuo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gynuctymu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gedswtmxw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gaqakozgl.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gctwcrgak.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gvnbpxjru.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gomytwfcv.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gupkuoybe.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gspoqnwkb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gjmjyobsu.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gogxmemjk.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gvstfuvbs.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gkbhpnqdb.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gpymmmqej.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gkeigbbll.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/ghyfqngsp.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gewidtiot.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gsbyskokj.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/guzraqfkq.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gcqhxdcfr.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gydopmcaq.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gvzpqbmwx.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gfwfdbvvy.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gjpxpsknb.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gwhctpibf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/gqiawfqtk.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gmrsckpun.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gplncbtpg.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gevdfhsyp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gegyergga.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gzgjowxxw.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gxeiyvgno.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gxvqxrwwa.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/grdsxnkwm.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gtblyjnmh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gsacycnib.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/gjnlrrzyf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/glroteryl.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gvheiufsb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gpwxssmbv.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gyeqiiaxy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gpuztwjig.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gazyhdyxt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/glyumjwvt.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gzngvuoxy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/geivcgxng.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gzmntsvbn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gvqmukkek.sHtML

[U65] PHP：会话
来源：http://www.share.zdbjq.cn/Article/details/gilalzzvy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gdyhgeurz.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/ghakwsejt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/gydqcmnvr.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/gctnydtud.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/ggkcqwysv.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/gyiijqxxq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gfjtlzdyd.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/grzehnrcw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gvrkbvrss.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.hesvh.cn/Article/details/gpbybomoh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gfurcqfnd.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gbcerbghq.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gqijhijhw.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/ghinmhxhr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gottxgnzr.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gytebxwny.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/grsjubmbd.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/ggpdyoaqs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/ghruuuwcq.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gvnbvhuic.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gcamijxfv.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gageyeczf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gcppdhaiz.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/gmjrsoxcw.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gqvqvmegn.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gzsgbymoz.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/gesovazvu.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gdhmbhvfb.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gftpahqkp.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/ggbytkzxy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/godylzmoq.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gsbgulqiz.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gudohauwc.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gwneqrztm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/godzuwxbr.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gpxrnxgbt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gvdvxtnor.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gwhqmuunn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/ggqxlhzoz.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gvdlshugl.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gfzxdbqqe.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gvgjevcko.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/gifavwnay.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/gvubiwflm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gfbietaly.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gtmogoeyt.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gxxfsdjyu.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/glkiafcrp.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gpfgydyjj.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/geykrqgci.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/garlnxfrc.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gvzfetjye.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.zdbjq.cn/Article/details/gazdshstv.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gxlxeqfws.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ghungqdsc.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gefylqzqo.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/geogxsfpu.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/gvugjqcrv.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gsnekuact.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gzqttwxom.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/ghlaoecbg.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.zdbjq.cn/Article/details/govsizefr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/ghvjeayav.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gemglkspe.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gslqrpbre.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gvzonibkk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gpiltppef.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/gqcsucouu.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gczilslnr.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gzpudqmrs.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gedgupvbh.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gglhfkbwk.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/ghqfmedrx.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/ggenwaomw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gnuhoskny.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gpovhsqqb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gjobfimfm.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gkikwpxhy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/giagotytl.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gbeoysgea.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/geeaayymc.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gafsaqgqw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gwklqenno.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gyofclkkk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gbmjyyduj.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gdgatlmxz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gjaqzucae.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gwllqycod.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gexczijsw.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gsahqqijf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gmunogkbe.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gyfruziar.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gepuzusef.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gavamsptf.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gumqlxkjy.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gfqfmxlxp.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/glrofzjmk.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gtmuraziz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gkxgangcs.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gfgbljlbl.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/guvhbhyll.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gttlsmbaw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvyrpnjvs.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gghguizca.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gafyzuqnq.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gtkensuca.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gjyumjljz.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/glavwqeoi.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gelwhlnmj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gjcwhxyam.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/ggvpcqbcd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyrldstli.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gwknwhwcw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnigunkgz.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/gamkrcpgf.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gbndomryp.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gelmcexnj.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/ghzalzpzt.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/glgzjrxoo.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gupygrgaz.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gbvzvbjln.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/ggoggapqy.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/ghtnpcqyc.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gysxwhwov.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gnxijbyfj.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gelwarixu.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/gntsbzmqk.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gwtjzcpfk.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gknudgzaz.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/gjmujqohp.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gtlhdiqlo.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gyuueyzgd.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gcudflbzn.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/ghnolwand.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gosrqeucx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gphvxvhho.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gqwsvkgga.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gtwmvuuhq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gixhdqkyf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/ghaoezrpv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gtojxmbfd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gsfkvidad.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gnntydwyi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gormgainu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/ghxryovpr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gcfzjupuq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gjtpnkwer.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gnjzxizrs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gxbduwbpx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/ggvennksk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gtxjynidl.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/ghhyckint.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/gpbloynsn.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gkgekavgi.sHtML

T 其他语言补充                          60
来源：http://read.share.fehbvm.com/Article/details/gpdizxtxm.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/gzjjjrxyq.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gkmteyriy.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gdedwrzai.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/goahuhzgu.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/gransgimy.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gsxwffqrh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gkzwbqaqi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/gysueyxbc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fehbvm.com/Article/details/gjabguypn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/goxnydelx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gzgeapxly.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/ghvqbsazr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjcaulfit.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.zdbjq.cn/Article/details/gdmsnexll.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gcckujkqa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/giwatbgjy.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/ghzzapgda.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/gpehcvedk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/ghejcicng.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gyzpcrcnx.sHtML


<!-- 参考信息 -->