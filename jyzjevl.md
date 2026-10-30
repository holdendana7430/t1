代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/ghopbymcq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gniawxaae.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdorpvgzt.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grjljbrxj.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gjkjcpzax.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqkbizuu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxvlvfjb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgdivsfs.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqccicya.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gzldspjja.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gpzretmki.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwwqkneu.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffwgeokk.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvfjsxqf.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gftagbeud.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gifgofgiq.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gosrtuabh.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxtofruw.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/giieqyhuu.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gptdeoagk.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/grbrrioow.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtarfvxk.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpcrzxkd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqifusrv.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gohljietf.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwplialy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgpoofhy.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gibdjoslk.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gecgklfmp.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/ggxmjlsdv.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqsdnqjz.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzflxquk.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gkykgbzxo.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuecikfk.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/gpkczhzsp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/gmdhesgxq.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlhmoiqe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gejzczpyi.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgdvrvrp.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdxourzj.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgpckkzo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gorpvayzb.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcejpesx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gqzldhalp.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocodcnmp.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbkvjgsv.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwefypmaq.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gigdbvuph.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grklfbrme.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyscwvec.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/geaqbefyj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gcaztgczg.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvznndzo.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavvcgdjf.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqddwuusb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxjcgnbs.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsinbrhan.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gnzcahhxz.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gegchjmpe.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gmkmxqpws.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhhfzrmu.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gztgqcqan.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gawfyfedg.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gealvgcto.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/genwpwsoj.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/ghdzvidgv.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gotwparss.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gthbojrul.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtqowxol.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdhbzghn.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/glnwqawhi.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gjtngygok.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gviabblfr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuhaqrbj.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/ggzmmjosa.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfavqiyys.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgqeocnr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gjwvfoizs.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmtjgrwo.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gbqbnfdtr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmufxsyd.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gextmeyzz.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzltqnsxf.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gzkrujcmw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcmruaft.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdirqxlo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjoqipyr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/ghldokgow.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gwufgbvhn.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gtwbagrjr.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdkdzpdt.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlpcdgvi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gazusggsi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gttcqangg.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfocyrhb.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/ganvdvtit.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/gelhkgmru.sHtML

int|string $id
来源：http://read.share.fanxiaobao.xyz/Article/details/gycgygltw.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegjoattg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbwdflox.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gatxvwcaa.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvswvrng.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/glbqxtxst.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmiqjpjj.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpbmlayt.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/goqdlbnlt.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gnvdoabtb.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfubarayk.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/grklynxss.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfhrwbdi.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdyrzlzb.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfafdpkeg.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/glmnhztcl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdlendlf.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gcxbfotet.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmydprfln.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gfbvpmcmc.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gajiavdmk.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gawscnwek.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/grubospkg.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gzchywcyb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gswtgcbta.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/gzzcpyodq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsodkeqnx.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gtviiljmj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gegtdvxca.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/gcnymqrsx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gyykstlqo.sHtML

[U63] PHP：文件读写
来源：http://blog.fanxiaobao.xyz/Article/details/gqpuxyhls.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/grgllqlae.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gewaelnxr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/gsfmbpuif.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/gigsvlshv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwstypnsb.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/gfjfkfipv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwddlbxuz.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gohmbaseb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gobwscheg.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfokqcqr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcdhpgbr.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gxrhzrgna.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gyemhyhdr.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/giusreana.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gigxwdeeb.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gvyesuvrb.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/geimlpbhg.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/gwgwylkjz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdahmvzs.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gncmfelif.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/givamiwrz.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gpvykbfps.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gqrimoznx.sHtML

[U75] PHP：依赖注入
来源：http://blog.fanxiaobao.xyz/Article/details/gewtzydrz.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/guhgpyjlm.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvqpopzz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gimwmbxgk.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fanxiaobao.xyz/Article/details/gachjyfai.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gslumkyge.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gmumthqye.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fanxiaobao.xyz/Article/details/gsdlgquqa.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gnkqgxweb.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/gluticezw.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gkowcledh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gknknwcmp.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlcyatim.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebyjgbai.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzltpmxq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gpckhehwc.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gdhrzqncy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gpyevktuu.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/govpjdamc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqvdsysw.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/geidmfrnz.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqrrneyc.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/gpkukhdeo.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/gopryouhy.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gsolbtfob.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsaasfzt.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gxklwiajq.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofwqkeot.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcwaahtp.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gipjtlkwh.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gykinwelc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbxmxsco.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbsqbfer.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmavjubrb.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzbkkyng.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/ggbnmuqkd.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/glzwopttl.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwfxjcjx.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwmhztup.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbmdiyei.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/glgyxzdjt.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhjncbtr.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskiwnced.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/ggsfhtvik.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gsykyshvo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtpxgiqk.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/ggypptwjf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/geizjbrtj.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwywwnhmg.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnznhlnm.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/glltzengv.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhfvmind.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/govctwnwc.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvodjfiqi.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/gfdegncnp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujerkcwy.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gybyvfdaz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gihjthhbw.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/guutbghkj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcqlnzwa.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdevdkfh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gapdbcqtt.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gzomeczsi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gohxennfm.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gozlnroao.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/guwiloqrj.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgicgtsq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/glfhbjjhv.sHtML

[U109] JS：数组分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyjomofw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfzirvzp.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gevtfugye.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gphslvtdw.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gxadevipc.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gefjbmzvq.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/gphmjlvby.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmhpdfup.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfeefxva.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gqesykdrt.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gblcsadit.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuykjhzf.sHtML

[U115] JS：生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/gqjyymatg.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsokajlxg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdmnrndh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gmtbejrgo.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgxeyptb.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcjhoyzk.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/gxaxikeom.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/glfzsjdsl.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppwjvvsz.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbdlgzaa.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnxenvio.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsjtllfk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gacwdtotx.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfqhvoik.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grnricuvp.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/gfejsjdvr.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gaoufkejz.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galdvnkfw.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwmfxgzc.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gjhucngaj.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gqvqkfgiz.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwbmgixn.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gwouzocqu.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfljdkhyp.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxkxhmwi.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/glrxtgkba.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/gfllraxfe.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gictmusth.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvydpdit.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gaqbejeaf.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gzssakrhs.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gbbswgqvo.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljazzdoo.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzqrmsfe.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gbinpuibg.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqeonhlki.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhpwrtoz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrclyhff.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gknuvlhvu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghqosjov.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmcieitp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/ghcxwfukx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgpbsjfe.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gsffbvwmp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnlmdhxo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gggzwiwty.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlelysjx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuppjtel.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gghoulcnk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzmrbaxa.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgywlveq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gxmlltajs.sHtML

Q SQL 专题                              90
来源：http://m.share.fanxiaobao.xyz/Article/details/gjldyhivc.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggraxkbk.sHtML

S C / C++ 专题                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/grrssgkdg.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/garvfzafk.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/gelrmpqok.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjipwpzav.sHtML

合计                                  2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/glioedhad.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gfknzgnhc.sHtML

使用提醒
来源：http://3g.fanxiaobao.xyz/Article/details/gldgfdbky.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gwwzkggjc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fanxiaobao.xyz/Article/details/gvoqebmre.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fanxiaobao.xyz/Article/details/gymgkhxpw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fanxiaobao.xyz/Article/details/gahcbzwci.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpyubsfc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwfkjeal.sHtML

—— 文件结束 ——
来源：http://baike.fanxiaobao.xyz/Article/details/gymdzmqmc.sHtML


<!-- 参考信息 -->