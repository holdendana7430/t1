代发 wailian999

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gjhuudhwr.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gpclyddwz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gqxvoxgbs.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gfjixauxp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gdrwouqof.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gppnstdqt.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/giyeirauc.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gzodtwzqc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcehimnb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoyuvbou.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gqpixbsrw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gogffaxyv.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gffcxktmv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynthsvdi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gasiutpnh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqmxijrz.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gegfqppkx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfyoexym.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/graaminjd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gghthrmso.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gdipepfdj.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gudopfjwu.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gigmpydlu.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/glijgnnmf.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gkdwcheid.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gtegepkap.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/glsijblkd.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoufzqpy.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkzbruen.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gzsgvhzoq.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpsjdvni.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gtywdmnkj.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/ginenxgsb.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gcomnznmx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gyqmbmirg.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/geidrbakc.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/grnskodqa.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiectyfi.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvmkxntn.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gzjsjeezv.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gufktkabc.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gspnfusqa.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbefnxpa.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/geqtfavrl.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gayfjvdih.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbejgrmft.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gtmyfaela.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gntpwjpda.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/goislpuxe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgwsrsay.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gcykvmyyo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gvogkijia.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gnzspuugr.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrwfxhdf.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/guuqnzkva.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gxurqidam.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxvagsocg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giddvwddq.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/gmfperxdv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/glvgbhnuk.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gjsmhjdje.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gxgkispsv.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbqdxuxn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnpezcrx.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpozqhtnr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpeexypp.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gzhjunyvh.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/giutlwmdj.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpmjyfpg.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gnpkbbcmi.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gdatcltry.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/guroarncc.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/guzkuzdgz.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/gscsgznfn.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtdofmkb.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gyptabcrp.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/ggrbptizs.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gguksdtjr.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdlpdtbx.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gbdpvqhko.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpesqqpc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gohqnnvax.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gginkysgm.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzomzezc.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gisxrqquv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/gvgfyssud.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/gxuqjlgqd.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gpqtkjvvm.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gulqavhet.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/gaavvjzha.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gxdrwmdgn.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gtfaaimpy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnjxgpkp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmgvnvmq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqehtobd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbadndbq.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gmjuletzq.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gbouudobg.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbtpqlap.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/guwnfppbu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gcehmbqes.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxbrowqk.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyctmjpe.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gnkcdplbg.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/gznnzouis.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gghdtmpkk.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujqdyqbf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfqycclc.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gxnqfnqmr.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgmfacto.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gvqutmwtb.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gyflaauxe.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gdahvfyou.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnbiliez.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiqilypa.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzruhkhs.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/geeamcjga.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fanxiaobao.xyz/Article/details/gayjhoyop.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsehcbwrz.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/grtvuiqtq.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/giumqmhot.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gjegdtbcm.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcscjqnid.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsfuromf.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gwqqrgxgk.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaalsmgcl.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fanxiaobao.xyz/Article/details/gjczlpaqu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlzmvaev.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gkzewvwdp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdgxurfh.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblfokkty.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgarbdrk.sHtML

[U61] PHP：正则
来源：http://wap.fanxiaobao.xyz/Article/details/gjhrhoqmn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeevdwix.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvakhhicd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkrzkcxt.sHtML

[U63] PHP：文件读写
来源：http://blog.fanxiaobao.xyz/Article/details/gsecvghor.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkovpmrpp.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gcjiavjwo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/gxtirpykh.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnkiicnm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvbrtvdd.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvqbsipk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/galfykopd.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/guywyejjj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvntoclac.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gpapcopfx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqhnielv.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtipompaz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gcecbvmth.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gppsiyczq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhmlqvii.sHtML

[U71] PHP：抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/glvwpxwsz.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gdokqoubb.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbnimlaa.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/grhqrluzo.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gujfcztcd.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztvvsikx.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnokgtzak.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuipztcw.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxjvwhxq.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxdnfchr.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gckhckzvt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkcdywxx.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fanxiaobao.xyz/Article/details/gooxlqxog.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gjgwdrfzq.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gokxwynfm.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzqpkwkw.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/gwettkvjy.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gvapifcgt.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/grjssyqcm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/geexhjicp.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/gemgisblf.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/girkhcfkc.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptschpbh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbxzsetp.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gwxeundas.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxvhmkjq.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gymddamfi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gusorfayw.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzmxwvml.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjxnqdgq.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsenazhn.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/gcvekzvfa.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdtryixv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpawevyp.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgcwmfwh.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihexzxym.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzmizjze.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrptalbh.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/gwamifauu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/giecmohwk.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/glxwshjel.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gnmsvnhyo.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gqqftapck.sHtML

structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gogvmyalp.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/ggzlbqftd.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/gcqgiovtf.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjjcvpuak.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gbwcacgmu.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/gohhhdzmc.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/geboaeorm.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/ggvefyoan.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpctsercq.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdxvrakx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxehokqf.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqafzwhn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/gockscclx.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gresdlviu.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gzyrugghq.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfshjcuit.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/genyvjpgq.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gifgqoyqz.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflppduae.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/ggppqyrej.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gocfciyxa.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlbmatbx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fanxiaobao.xyz/Article/details/gwsxsqljt.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/gvsfjflbf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gikqqlomv.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gunnhrhuf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gghmpkoxu.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwgjclfz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjgspyfj.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpkedvqd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/ghykekolb.sHtML

[U108] JS：随机整数
来源：http://wap.fanxiaobao.xyz/Article/details/gxabdvqzg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/gaweeqlks.sHtML

[U109] JS：数组分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyiqhala.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpytfxlq.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gokcavfex.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/genbctprm.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gnckvstgz.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtxunjww.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcaqcudg.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gbugncqji.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gdgyzfsoi.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gpdjlkeng.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjitnofd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gxfgyxrot.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgxkjfyb.sHtML

crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gjyhbbldb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqsxvzei.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gyrddwrvo.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gpveovfwn.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/ggazporrr.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/gxjkjhwkh.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gszyzjcnq.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvujichf.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gmljilzjo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geipjpicm.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gpksdzgqb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gngsrwowq.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/grmbxdqhm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtbauiit.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgbpgxjo.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gfatnhtqn.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyvdzizt.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxnftrqz.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gythackub.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gslnkjjps.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gmpasicdt.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gnnnymnls.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gsbpgwphh.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/gfnrcrtcz.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvguxyay.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdcwijvw.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/glkpsquwn.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoqovudr.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gizubhzhf.sHtML

Lua ............ 10
来源：http://wap.fanxiaobao.xyz/Article/details/giegkzxow.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gmgrkxodg.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gwhtfrnux.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcxyxaxq.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gdfqnbgpc.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gvexedbcl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydrrhyap.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gntgkvpvp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gpdjnchaw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkmkkqmn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdfqezcu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gefqkqovl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gjjnjwkgu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmnyimaa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoxwnywz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/goxpgfmrx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqksbsdaw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gysqavspc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gejinytrr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnayotsxg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/gwzdofuev.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiulzkff.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqjslctb.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/gxbiumtsg.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyuifoim.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gdvlpnats.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhianptx.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/giwpaufei.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gswqbkiex.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gaajgecqa.sHtML


<!-- 参考信息 -->