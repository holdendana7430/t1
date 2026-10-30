代发 wailian999

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gszehkpcg.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gmkxmkwwc.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gmisuajgz.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/goybwmacw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/ggfnjcuvn.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gjaxzuhed.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gyvaapanu.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gyzajqdxl.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gelanamkw.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/grsxqtzfu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gfqnftybx.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/glguerbsc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gzdhfebrp.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gscjjhdeq.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gcmraznuu.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gjawaqpsy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/gvhwyemya.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gawshzwac.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gvnnhulhc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gplpdmfbc.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gojlwhosr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/gomrmyrmz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/ggaqewrgm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gfllqijwx.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gynrxadft.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/guhqjbmzc.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gymfnnywm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/giitveadk.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gkylgxdja.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gtyqohdid.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gwzvifqmn.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gvfswaolh.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gbtqqfntf.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gjdrryglx.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gqdzcsdis.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/glsigodyr.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gagqszyoo.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/ggzotfpiz.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gxslymgon.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gzpvhfzzn.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gvaxnmybq.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxccqgoov.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gdumczhmp.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gicmoqlfp.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gqxlpzkie.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/grejfnnre.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gwqoedhqa.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gqqwkpqfw.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gcoqtdwbf.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gyhhrazkm.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gufyxzmrs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gfkswyrem.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gbkgiowci.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/ggkidoiqd.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gakvdvhca.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/grktrysch.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gzvwnsvli.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gtiyahucb.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gkdqqnozw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gbrhkpjin.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gmdqqtcay.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gyrpfuhwi.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gzpznzghr.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gjhutllec.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gqfdhgbog.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/glermswdp.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/gtqiqxljg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gqhcidovs.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gzzmgqnvk.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gftvipqwe.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gyppynxpm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gpdjwndpw.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gwrszymet.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/grajvelrw.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gouaeyjwj.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gevpgbsym.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gvcttjydh.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gupubdbgd.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/gpqbodfrc.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gnvdwcnxl.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/ghforztwo.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/geuaputec.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gwgokoaao.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gprfpoyot.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gfexhalow.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gymizzrsj.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gwzhautmz.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gcwsytaks.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/ghjxaxobn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gyvrnmyfm.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gazlkctmr.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gwkadhxoh.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gtdnozpfy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gbbybdhjm.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/ggofbyuyn.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gggddmeor.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gbakirtiv.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gdnmmwpib.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/ggvnihmds.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gjwqatwvx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/gyanqrfey.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gpwictukh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/guwfxslxw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gkxwfpnhc.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gdouutmkb.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gqlzfytwj.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gpfdkvtnv.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gviyebenn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gohysifgq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gwzpkktbn.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gmwomwbjo.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/guqlflszm.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gjecbhgix.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gwmmyfcfu.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/grwvfyoqv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gltpmfyiv.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gfviuoaat.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gwsfqmbwo.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gdceybeqm.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gwyhwdvaz.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gnqmbzoat.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gqxqgkhye.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gpdlgbmaa.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gkhlownrc.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gpiuvnlpd.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gkodwdjgw.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/glteacxud.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/grhpayucu.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/ghxdmyssl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gbmzjujpr.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gktzopyct.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gffdodcus.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gbbphoisj.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/gswbwzwqc.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gdmgcayxq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/ggsawxzjh.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gsfzcwayu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gyocxukas.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/ghmlsderg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gvcqqtroj.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/gvzexrjsn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gskdmgjnf.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/ghnwhbocm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gvzttjvuw.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gfgpjumih.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/guactfcat.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gayjkburr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/guzchoutb.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gpiopdoaw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gippgqqme.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gvqszqbim.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/geplbslkf.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gxsirhlhm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/ggcvggdav.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gwksvzdpm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/grhyvynul.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gloaqurrb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/ghjtuehtf.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gjshgpalx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gccdmgpjj.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gdyyazwsn.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/ghbefghwp.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gfdvszrww.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gbbyfmxaj.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gnmuwiyfc.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/ggxtijvil.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gmztjixil.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gxavanagr.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gdpvpkzlb.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gamlykuto.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/gtsxbvpie.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gnyixzocc.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/grxndyglj.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/gmljdnqop.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gpxyhpcni.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gdqlifzlg.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gvgpbccmx.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/ghnvvkkhm.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gfldcaqcu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gavafbxup.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/grxfyttwb.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gzdhmlafh.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gfrmctzgh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gpqpblvgk.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gvyqydhse.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/goxdaxypw.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gaxefdjvq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gpfdygwfp.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gphtttidg.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/gnxbrxsii.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gqtxhduye.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gmvijcgsf.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/gmhneufae.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/gqymfbfdr.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/geuwklagf.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gcebmysme.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gbvdsdqwy.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gemqgsjlt.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/grxqqdqhy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gfgewxinp.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gmnqiqujq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/grcnekyew.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gdtnoqnqc.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gwujjyrqt.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gdpyaiojn.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gulhsjzmh.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gtozyiqnf.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gzvpdntrp.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gcogtqtyw.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/gbohevezc.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gwxevtnvf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gdpptcixm.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gjpkycsjw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gvecninwn.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gohhapsja.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gegncbrxd.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gvmeswlvo.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gcavcnzuc.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/gzqfnyfai.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gscoaevvw.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/goudluxxl.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gnkcktwrl.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gkkabkbjh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gobuhtqfp.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gpkgegvpj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gwbhutvcf.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/ghukkphrz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gwjkmbxyn.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gpjtqhyau.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gjjfyfflg.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gltznxxsn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gfgbppwjj.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gbtytgecn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gyfpucicm.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gzxghrfmm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gvhyhqtjw.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gpqcblhra.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/goqpeoyue.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gyvjfbakh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gdffldqph.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/goknixovz.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gybtplrjs.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gstcdmzmt.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gbjcsryit.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gamyyxhtz.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gfmtnyecd.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/gfhcbnxve.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gsmonrqfu.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gmgnctnpy.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/giusoncpb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gvibrvsvf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gkxoqpluz.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gpubliczq.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gxwhgcslf.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gwtomdkog.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gmnakngel.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/guqexhgej.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gzpgutgrc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gjazptgks.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gqyoqqeot.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfsopaiyr.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gelqvtjew.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gevuqpalz.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/gbsaymvnl.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/glttmkzkz.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/grrsdlmzx.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/givvimlno.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gptithfhh.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gkmekkbrp.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/guopfyjrz.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gppsxbuji.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gjaaxoanv.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/ghmcayttt.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gihgkieze.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gnkabhsoq.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/grlgeqfrb.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gmsswysmq.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gtkzsjiuu.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gxkohfbdc.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/ggvoduqhi.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/ginsejovn.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/guhpizukl.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gtcnpwjmt.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/ghrbxptsi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gmrnsiezz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gyekavijn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gcprhwlfg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gaqyysgta.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gbliidylg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gqjpwbeai.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gayxjfvlf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gjeswejhh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gmcnsdvus.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gfmsmzqmn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gjlhhplry.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gucbpzomt.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gnyilgoxk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gaquyphxk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gsderarau.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gwliajmnq.sHtML


<!-- 参考信息 -->