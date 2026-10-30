代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gmschdfft.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvqggrjv.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gjeoseahn.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygelgffy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmklrpczi.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzperrvad.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpragikm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqtqilyo.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuilfnrc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gldjefddf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gotaiwdab.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ganhucbzi.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gsjejmxqx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecnmgtyt.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gsawtmpfo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtsehpnq.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gsfjnxvsp.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwssctyah.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gypccsbbg.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsvxjkkl.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/golezwmbb.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxkkswga.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkowgnmt.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsdmzjaz.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gowqqupzh.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaeqifrtv.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gzxnpnygf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/guvwrqmme.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gsspbqsbw.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvaahajzo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gdcwblbne.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gskdzwsnt.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gofcfswxu.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzenmihi.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gaxxxnuns.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjiwngydt.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdaeogrje.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgajdmog.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/goypowfus.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gphfmaycf.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/grzurueje.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gezskmrfy.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/ggqnbrezm.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdrmzvdf.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/guvesubou.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gndoehjou.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/grulkclfo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/grxejkamf.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/gtithqyof.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnszkmxb.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/gquzqqyrf.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyvjompy.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmdtcihm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gbglecnrh.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/gcaxwbyiq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/goirnzqst.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfryqvhng.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnyzjixi.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxnzuggn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gnodsyvqg.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gvvjkncxz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gqmxweowi.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gmkbujxgn.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gacvgcirm.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gvbeibenc.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gecavpehb.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gssgtbbiq.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtukxvktm.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/givtogszj.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gblpfggto.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gcruuqmie.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/gavqepnee.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gvcacqxsi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/grdixenun.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/grvtatzif.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gaqexpdpd.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gbvclyflj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaczazfkt.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrkwloee.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtedigayi.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gucccexiz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/guqiryrcp.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/guizibcko.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gvjkbapxz.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gqbwauhbn.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gfuwydmak.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteccjrkf.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gmuysvpdv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gqztowqhk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/gcydgcwhg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gwmxyffll.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdosbaas.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/ghwibatdo.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gkfrozaip.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gsblbctiy.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqpvqrrh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/gberenxnb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqriwfyk.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/gealoeiwe.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golpdwkwm.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyhzpkkz.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrwvrmbc.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/ghqpdajld.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwxvrncc.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/gtuxlwbvv.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/gtemdxfsq.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/gumjktkmw.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcwisdqj.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsdvqxsk.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/gveftqxwn.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/guvhtdowx.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkservdkg.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/gootshwhq.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gqixjpanu.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkicocnlb.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gllpraxml.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gqarbhtza.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/giedbxxnr.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgniwkde.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gozjazevb.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gyhlzppgj.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhpwqqnf.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxundwdl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/griwqjisl.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gywtsxszm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxufzidty.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzuxcxzp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvvssjcp.sHtML

[U61] PHP：正则
来源：http://wap.fanxiaobao.xyz/Article/details/gmhtdqopl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxbfexui.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgvthlgp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/gnevkliks.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnlnwblk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fanxiaobao.xyz/Article/details/gntmcxvuf.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdijrrwil.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouvdokqz.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicmqtbcr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/grrynelnt.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsqbahba.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gnbjtrbvl.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoxpoixw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/gfvxqxbhk.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbusohqy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/grgywhwfq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjkvowgd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjslgbtdc.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpkyvgnq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gmawtexqt.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvfwkhau.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gueginnjl.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gryaazslc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/gymcfxkvd.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gpckpxwkr.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsovnzpk.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkysmxxrj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gezrhbrah.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gpdukikyk.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/gueldfieg.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/goralbqcb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/gchvuzwjo.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdnixoij.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndqbehsq.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxaqafic.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrujzhcl.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmnjexhf.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gxbhjgkzx.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/glzdwtyqt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fanxiaobao.xyz/Article/details/gowfpyatp.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthtguync.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjdgxdcm.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/gmetmxtpu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gyldndjgf.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gbhxzfipu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzktmduc.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/gvzrddffj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwhqepaa.sHtML

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/gtwpyntyy.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/ghmpehjtu.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gldszdcmr.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/ghulwngay.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gyiwubbdi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fanxiaobao.xyz/Article/details/gibnfmtpe.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrgcpqkz.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gjfehuoer.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmdqyrld.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqkdpczm.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fanxiaobao.xyz/Article/details/grebizkwo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqwruwfb.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gufegigwf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhmayyeq.sHtML

[U92] JS：深拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gxogqfhaf.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazbehzqy.sHtML

[U93] JS：模板字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfngbaqz.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gvicdtrqj.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpxpvhqt.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvazsqpcm.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/gxobyvzml.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxczpdbr.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzkasvvn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gnjkbysrv.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gcvvnmaza.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccefzoqu.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gegdirrov.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gchxukvrv.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgousdif.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gaixjcxyq.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgsmowku.sHtML

document.querySelector(".item")
来源：http://wap.fanxiaobao.xyz/Article/details/gyatneyeq.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojhlmcjg.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gipkpnvrs.sHtML

[U102] JS：本地存储
来源：http://3g.fanxiaobao.xyz/Article/details/gejcsmimw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrupidsi.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/grgbrvupl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/gsypzqyyp.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrmekbaq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmuepfim.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/goltjhuev.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gspojjyfb.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gynekjkud.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gelnynumh.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcqiryoy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteepnlcx.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrzsypvc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepephmcd.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gaouowpng.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gqjelirtm.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdtztoyy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaddsqijf.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaicgnhz.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gowoxjvml.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gqamyxsto.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgkuaemh.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/gcrupkjkh.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkezcucpw.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/glfugzevf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gfmizmxed.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzdbivmv.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gltnshxrs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/glzckhwrf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gryvxmacr.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/guskszfml.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/guhaizlue.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/gjwapusqi.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjbibxdx.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gflypjuqv.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuwktefa.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fanxiaobao.xyz/Article/details/gthpqgtiq.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gzkbwmkyb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymwdicmy.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/ggndklryl.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghskrrkso.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gmqkdmiuz.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gtgrguniu.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gnjigqrva.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gubrzzghd.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gdxrkrxul.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpqcmbma.sHtML

Go ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrnypvmb.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghudtlxpw.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gkztcsmlj.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/ggidoletm.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/gyjvmeieq.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/ginpansqd.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfiwcjlt.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gasivlxza.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjpaiabg.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgiojrul.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gvazwuxww.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/ghdudxudo.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/ggtdiwazv.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/goraieanu.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhpsnath.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gegaeqjuj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gynzkqfwm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhvwphjb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcisoilja.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gsjexnnzi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbapyazv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gsprcxyjr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gfmaoqtfc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gikksvkcj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gesozvjdl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/guuittosq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gyxfycjbc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqgdbtht.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gdiigpapo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gvrtaamph.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewatnfxy.sHtML

Q SQL 专题                              90
来源：http://wap.fanxiaobao.xyz/Article/details/gruuvyhgp.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/gppvfkjkk.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gmvrrxaiu.sHtML

T 其他语言补充                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gndausfal.sHtML

U 高频实用片段                         120
来源：http://mobile.fanxiaobao.xyz/Article/details/gqliommpj.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvgwhqiv.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gdekhgfem.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/grvjlgylq.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/giaycwymt.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbvvjeof.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgzjxgtw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/gubzhexpw.sHtML


<!-- 参考信息 -->