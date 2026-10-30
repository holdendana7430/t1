代发 wailian999

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvyqalvk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdhgorcd.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtluboed.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gnenrzjfm.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzexxvbw.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/ghynljwwb.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gvnwewxun.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsbittte.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuqcderl.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/glukyxuac.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnoqlwgy.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gsooewzvw.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gcavnudbe.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjggqhqj.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gznwvhoes.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdecqtnu.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gjarhoscz.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitashxby.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtacnfyea.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/givvqgwjf.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/grdvnxwkq.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfukrzji.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gorakckwv.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/goimpovap.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrlgzsys.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqkimben.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwsqtlqo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqanyuayb.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezsgpekm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gastwziwq.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gaxrrkxag.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdaiadpcp.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejcvruae.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxqsgzhh.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqmiezij.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gtlkixctm.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmchvbmq.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gjudhuxrp.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvmdyqfd.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gtonwuxsa.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gobyjjdnz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gwzrlrmgl.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxihnetnm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gitgfrzob.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gkhfeeiyg.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gtxefwmtl.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/gjwxzfrwl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/glgbiugjc.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gywdbpjol.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gdmqvankr.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpyyexlo.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/gjckifjtz.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gdwzlrdqa.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gjctolpco.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknfrfubr.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gkxpfshws.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gexnofnic.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzooporqr.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/guhtlxjmh.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/gbreajvou.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgesytxi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gnznewgsh.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxiufwms.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gbjhtcvxy.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveycrryg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnvsvxui.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gwiajseuq.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfgujdcb.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gjzrwrpbb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/gqzeczsxi.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/gzqreyitk.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/gitxtwwlm.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gnzbekfiq.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gjqjbaghw.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gmetjjqlm.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gliwmhuag.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gwhctmmpe.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/ggadadlwo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gzldalyag.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gexaotnhu.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdnnjjgx.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gddayjirf.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwykkitm.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwgziypr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/gspnfcdur.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gemrnklzf.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/giplpgurm.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/gbnoidfpw.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gekjryrrp.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gvcgfpisq.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gpphxxpjn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/grobtnoqp.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucjezrxi.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzsxukdd.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdofybixa.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gqdyawweg.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/gfpewkguj.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/guwoibuyo.sHtML

[U52] PHP：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gveqzjexi.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gyqpbnkaa.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/gdqscrzzp.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gfsnhrsej.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/gidntioer.sHtML

$obj?->method()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghymzzczu.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/goccudrhj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/glysqakwj.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gnmzyvpys.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvemtefyp.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gjsptfwri.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcnfdewn.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpwkabbx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/goowxsfag.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhmaqhfa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioihjzpr.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjxjlbnu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqnmtgef.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmglvuuf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gelutujnd.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgvbqlyd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjaskens.sHtML

[U63] PHP：文件读写
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnidkafl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gmivkohlr.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyezheeb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfszaonyt.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/goklhvrsc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gjaozhjfa.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxurasjro.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/givfwumir.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/gyjxdpdud.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/gedgmisoy.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/golhmmjcz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/guqivaybf.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gzqpogcsq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyccbdtvz.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfuhigke.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgtbzowz.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdzyacad.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gwemponjr.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/gitowsuuz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fanxiaobao.xyz/Article/details/gsadhufvu.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogsbdwsa.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvirwyut.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/guvjqrmmp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykoyoumz.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjlqjdoh.sHtML

composer require psr/container
来源：http://wap.fanxiaobao.xyz/Article/details/gbooumdlx.sHtML

[U76] PHP：简单路由
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbrdpsnu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/gystzszrr.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/gdffeemei.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/gccvaieij.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyrbleyb.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsdjnxel.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/glwcwofkd.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdyifsxq.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkurnvpsx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gvcqdzmbe.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyudypmom.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoqtodcj.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/glbxielxm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fanxiaobao.xyz/Article/details/gurwmfihp.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gyluvogli.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxygvglm.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmboxqqv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlulfsqt.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gmjeghrxs.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gkwerklpy.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gceyxjbzx.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gkqijcyvd.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhjvcmbm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/goznljlvi.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/genyvijhs.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/glrdpbuod.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gcnmilynj.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/giapbeokq.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfzmvlpn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaybqfatd.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/guitszqtb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsjxbqeb.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/glmoukrtl.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gadvittaq.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/ggrhnrvkt.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoxtwfos.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gswgeijcw.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/grolwnfdx.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gautcamrb.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gxuksqlvr.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/gxegkemua.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlmnygvn.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gmrttqfzn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gbxzltvsd.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqjryihu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/giewdmgrd.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gtjgxuknp.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gnhhrcsxg.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplagwvka.sHtML

document.querySelector(".item")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxkrdlqn.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gfedasono.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/glyrkrjcz.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeevwobs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gzhjocitg.sHtML

[U103] JS：定时器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxlmtjdl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwbhwtvz.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/gebkgbhbn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glugcxlny.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gmknelays.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gcmamndfz.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gadvgvnqs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gxbiecspa.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbnqevnz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzmpynhs.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdknufkjj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwhporee.sHtML

[U109] JS：数组分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnyjsche.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmplizyt.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvchlbtu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtdmjsxi.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwhjiosf.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/goixbdbrt.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/gqygtgnpu.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprxinilq.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/gdapxwqga.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghekxgmel.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gcvcpbrnk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/geuexxysr.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gelijlish.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gtrmrtyqj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/ghbxydczp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlkqosyc.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjxrxbgn.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqenzxpd.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmojqnqk.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gxnkbtgxx.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnsbinpz.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmzhgyhy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwljdwpyw.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrvxwbhd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gpunqzlju.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/glivfuohe.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtrftqntd.sHtML

按语言统计（条）：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqpriqrq.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrqqiubo.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvcadbkn.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gejywwgiv.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmucwevcl.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/glsuloojj.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gyupugzgc.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkysgzzt.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzhxsdhq.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gxarertae.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbakhmct.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gxzjnfhdq.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gouyvhgrg.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gguvexcwe.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gsamvxeem.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gxidjdlqg.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggrageww.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjgelohw.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gclttxpes.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gwvsaqnvm.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gerrssfpv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gskgaxmks.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gnfbpdzdl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/geadbcmph.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gfunxufqi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcsfyxsj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/grdvnxzvl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gorvzchim.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpaxfkke.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gcyucimtm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gzsspnsjo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykrtolus.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gclhwzgto.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/giqogmmzn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxpbhjnr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fanxiaobao.xyz/Article/details/gppogtwud.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gynrzrhqy.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmbecvpz.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/geoixlagv.sHtML

S C / C++ 专题                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gypscdpuv.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gwfraxkyb.sHtML

U 高频实用片段                         120
来源：http://3g.fanxiaobao.xyz/Article/details/gbvpphavt.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gsvoitepa.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzgbsnyt.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gowszwkdh.sHtML

使用提醒
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdwkpnyk.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsdwhcri.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/ghyctwhkt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcsqkjty.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/grjzhxapd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecojhluk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclntrogl.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/gfdvqhsmf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbwpmgnkq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fanxiaobao.xyz/Article/details/gxqccjbnh.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fanxiaobao.xyz/Article/details/guzrsokar.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukbzcasb.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/gvxkclypn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/gjupdkhbi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjqruqfl.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsitgpuor.sHtML


<!-- 参考信息 -->