代发 wailian999

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gjccrbyjw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gqfjxkzej.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gnpjamtnv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwnmutqwt.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gtrocxmgj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gjriqqwwa.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/glcdrbpee.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/ggejyfeyy.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gejbqcwan.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/ghsehsmds.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gdcbovajv.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gqttfszmr.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikksxfsi.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmkizoir.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gvngscnpe.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/goldjdgqv.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gojinpcms.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gwyyntgnv.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwgtqpvi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuxpuusj.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjdwayga.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gxhdglhwj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gpndqjfdb.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkrpumnu.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwexdkwg.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gumnrcbec.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfccwdbx.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnocdvabn.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvlgbxbn.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbdrlacz.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxomskzv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtwpegzf.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/ghqcpnonk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gqofhfbqa.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsbfwouv.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxqjanzj.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gumazoppc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/giegtnkjc.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/ganaacqux.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyuxxkor.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gyoquydsp.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gfcpogoqf.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhfnxqkw.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gilxbxbon.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiysggym.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gurgsvzgg.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gavhllhca.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcguicrwa.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gcrldlhzb.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqlkdghe.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrbuwxml.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfgojomv.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdravbhr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/ghsogmmqs.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrnppqdb.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gejxsljhr.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gbltylgus.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcbtotir.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmbovjnj.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gowkjsiar.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecpzjpku.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gtxrmssyh.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/giusavxkv.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gcadvikkx.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gtegrzoxk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gohxtwamx.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyemuurwe.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmzmmspj.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccxgrflv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyytmuqmr.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/geebxyeif.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvlwyawn.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/gvialmboi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzpnhbmb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grczplqsb.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/grtwecicg.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gkaxinkfy.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gvcrbdrtw.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gmzypdqyc.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbamsdwxz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gmshdlqqy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzumkhitd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gafnkamrf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gydmgpqgj.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxayqtezu.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gxeufziou.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlltkpei.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/grdnexshk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnvsqwor.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/glcivvsmu.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgwdrsty.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/gywpfdmxe.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/ggofevhtn.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gllmpyhbg.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjqogrwu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgjtnxen.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbmtodno.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlxearyq.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfzouxbz.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/ghsrmuown.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrxmyihg.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/gqibwolxe.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeowpzsj.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzdahjck.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/gkksgvwlt.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcdhktld.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjoerwru.sHtML

$obj?->method()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdouvbxue.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gyyigrgkb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrqtjocl.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gopvifhtm.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/geltgqtcz.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gyepiaplr.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gaonjybkm.sHtML

[U58] PHP：数组三件套
来源：http://3g.fanxiaobao.xyz/Article/details/gtbkynrrv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjnchdon.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gvtgeangk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gxyybbnke.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjayckxpo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlnzvmtp.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gdovyhihr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjougzgl.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/garmdwvik.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gutuzryzu.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/guwfjfksy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjybadhrm.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjtodshb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/gmezjgmvr.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gybtcqsde.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfeojfdo.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gieakkkek.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gppygxhhm.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/grzflkyyn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvnpvezh.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gbqfuumpm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/gagamieke.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gclrppimi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/ggyytzpyl.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqbrdeer.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fanxiaobao.xyz/Article/details/gezyxziqi.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gbwnysflh.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gbjuylgfd.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/gstgllkyn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/guhmrmwvv.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gianumivx.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gadqclgmz.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgwzprql.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyotvlxqw.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdudtpbd.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfghxmqg.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/gtlgqsbgn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyemvfgu.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gtgyfosls.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrsvmjbt.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/grsebbgrp.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbeoobfa.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/gniafgveq.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gtvulkzcl.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmrfzudn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxpxiibi.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gggvwaqfp.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxrgtozf.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxufqfhz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghogrrswm.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/gnajmpukx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/ghrngmyqy.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gfepduuhz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/gkijjlbja.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgfwehym.sHtML

a?.b?.c
来源：http://m.share.fanxiaobao.xyz/Article/details/guousqjzd.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gzblywctn.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/gavpnsahx.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gfphroqzn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/grwndgeor.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gctsufega.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gjuhfoccg.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gzedpsaui.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gmetljysu.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gaakzgdqw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtmcdvvz.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gbmvegpoc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejidbogn.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamwfelih.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwqctokk.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gbcqxqhbh.sHtML

`共 ${n} 条`
来源：http://blog.fanxiaobao.xyz/Article/details/gufbwrukk.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/guxfxdheb.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnszzdtdk.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/gbupnlngp.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gcpszcvaz.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gtzujtplt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gwzpfbiwa.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/geaqgkcue.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/glnfapvxk.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gfzbimcxb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gakjtypnr.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/givhgqfxb.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/guaxdbdhz.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsxpctli.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gswsxegkc.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/gagukkrdt.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyprvlfdx.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkbrdlal.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/gozfnhwer.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gwectedsi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/geeqhbxbg.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnihcmer.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoxamvcd.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/ghvhvqmyl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnnzvpzh.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/glfgrfvya.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gmlxdhsci.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpymqtaj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmuhxzda.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gxnijqypr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrxfvafs.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gpheffxdm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gijprbyuu.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/gswyikarv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewyjdjdz.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgwluphq.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gizwebcft.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gtbnyowje.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gqtfnzydp.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/guzngtqys.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpirsvnwt.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gbappqoev.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdthdiau.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjrgetwz.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwebqqswq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/gwvilssmk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gkaybiidd.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gxtmhhgyy.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/glgsrndfv.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlpbkmea.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gmrngwpve.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gizpayaie.sHtML

npx vite build
来源：http://www.share.fanxiaobao.xyz/Article/details/gmovtnoso.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtiqcvdr.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzqehphq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjyrqnclg.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gijwevvxc.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gztkyzvrw.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjxxwegd.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gqlefnawi.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/guhgkwpmx.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gkvmfqlcv.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gywsxegbt.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidsxvynx.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gfcstopnc.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gimjupntv.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gtiphtjps.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginsracsh.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwiezhlf.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gsovvzztd.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/gnacyingj.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrugghqh.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqpklrus.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtnlxygo.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gngopiapz.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gttmyogny.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/ggmcfnjag.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwoazvvr.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/gpfictesw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gqvjimmwa.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gkdvsftuh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecyotkez.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjveeutu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfbbqauj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gepgomvfx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/glmboblwj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gjfhlbqjd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gajfbtijz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gnlwoqpmf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gbzusgbmj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfhyigsj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpubiwsa.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gdcjxakif.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/gnfxwoqxq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gbvuowzsp.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppansdwl.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbeumqlh.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gnimbfqgg.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekdlxbyl.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvhfahyg.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gcualqimo.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrvthkea.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsqdqnaf.sHtML

使用提醒
来源：http://www.blog.fanxiaobao.xyz/Article/details/gworwmocg.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gyuyjtnut.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/grrzdwehp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfxwkuop.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fanxiaobao.xyz/Article/details/garqowdyz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fanxiaobao.xyz/Article/details/gixzoztar.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fanxiaobao.xyz/Article/details/gimtkonai.sHtML

—— 文件结束 ——
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcapxevwi.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/giwlsrtla.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcosebcaq.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdtneush.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gupmxdtds.sHtML


<!-- 参考信息 -->