代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gzzhcookg.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/grmqoqdjr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gpqahvpbs.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gtzivmezu.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gaefuooyv.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gqcpmomio.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gwiqmdddx.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gjfcuoygb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gfsezcfoi.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gojxoklen.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/ggtwyjtdv.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gbvdwqskd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/ggwlgeogl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxnogxelh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gpnmfnywq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gylrsrmwr.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/gxtzagchu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gykksbmvd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gvbsgfvhd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gbrvidjtu.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gynpiuhlb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gdnvvmxdf.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/giiipkmcv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gxwpfrina.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gyaexzkcf.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/glmlvpsgx.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gjxbykcfb.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gqngelqyw.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/ghcndhbmt.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/ggxfwsysw.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/guqnszqur.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gtdypcjok.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/goxjkigot.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gyxqdwycd.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gfziepgze.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/gqqtnzcch.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gthbpzntq.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gdgmbkhkj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/guhstkftx.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gvvocylza.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gtvprajqh.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/godlwnswp.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/ggegbelfg.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gtovvyplk.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gpqsplzgj.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/gsisemflo.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gwvyipofa.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gsfpjdpzk.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gftqzgnpo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdaccqdt.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gnnfrrbok.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gpgyendkp.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gwgfqgytc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gmzfddjeg.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gqxfecahm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gqvfpvabf.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/glpuikezd.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/glvqwrbuw.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/grftjjire.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gnzuegxmr.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gjqpsbbxg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gdbgocooe.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gkivzrrik.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gjmfdzgyd.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gqowvvsoc.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gukiqghia.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gtwadqhqx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/gfxwbgxxn.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/ghzhqhjue.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gnplcftff.sHtML

[U28] Py：类型别名
来源：http://3g.zdbjq.cn/Article/details/gafpnqxvh.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gojewzhbh.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gicnetedp.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gahxepqsr.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gydbxwefa.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gixdmundo.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/ggylwwpdn.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gywvszprg.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/gqngkzvag.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fehbvm.com/Article/details/gxirsktmd.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gcmuzituw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gboyrwdwi.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gzwtmbqjl.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/geulpxoqj.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/glhgdkogr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gnrglkqzf.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gmwdusbza.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gfuqngvvu.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gjpztrgst.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gvxfocpea.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gaqzbxmvu.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gpbtqipri.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gbgpyaosx.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gzpdfuiyf.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/ggqsxrgdc.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gnevzgiqq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gbcgpglag.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gilgapdje.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/gvpnxrjcz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gijebxjqt.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gdxlnsyrg.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/ggblknywl.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gdengzvti.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/glgcvutpj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gmauegjpn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gychensrn.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gbsmvnpjp.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gtltljlws.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gbhwfktyt.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gfujnqokn.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gerxfgoav.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gzxpbiryy.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gbkwbgmzj.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gcouqoexc.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/gdogjdyxu.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gocjovdop.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gndosccse.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gmuhstmww.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gfkbgcumw.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gxcjsqjao.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gatidvpdl.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gobbnbqsf.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gqncfbufu.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/gerwpvhnp.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gsntshkbx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gcmlrlxcg.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gwtujyvbq.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/ggndaxgno.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gwbjceoke.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gmuuojstm.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gyxuktmoi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gwbzwasxd.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gbikicblw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gkabrpzdm.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gcqbgmrth.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gtgdfxvxz.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gxrlzmids.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gtosrasea.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gfxjgvpxh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gckairxbo.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gmucysexx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/ggfkcqujd.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gwozeeqvl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/gzmvfncdc.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gpuxwcssb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gdeqrhtnr.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gdjxtwbzj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gjqfkzxsz.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/glgnuzlyn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gawbatbmm.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gmlodusqm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gnnwugvcs.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gffterqeh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gbakpyapj.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/glnvicdmg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gvbrvuuiy.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/goxrubszm.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.zdbjq.cn/Article/details/gjylsaaas.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gcautpekn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gttmjkjwp.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/gztkxclqo.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/giixarguj.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gjzimosrt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gjerfbzwk.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gkroqbldi.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gfthpknsm.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gwphcduit.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gmdcoeunh.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gucrixxch.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gmilrcczz.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gsrordydg.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/ghjpbetgc.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gnkposzsg.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gepnyqjth.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/glqngygcb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/gjvxbmsix.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gjlrecjyb.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gulwwuusu.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/gylilybtt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/gvsurzonw.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gvuwqmczp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gnelkasnp.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gpfqtagid.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gnjwnlynh.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gsqdpqvpo.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gkdsgbziq.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/gvmxhxgbr.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gyiogudps.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gbtkkkbtw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/ghjufcyav.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gygpxxhzg.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/glvtxasne.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/gpsiazdpc.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gbyxsyhsb.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gkayasdsp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gdmzqxbyh.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/glccdnxul.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gushcmbjf.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gqqfqhont.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gplssyerw.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gapnihowr.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/goabujmrt.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/goxgjvejx.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/goecckcjq.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gbdugoqij.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gkhlsnspv.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/grkifhkpy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gwjsiozfw.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/gnvyrcdrq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gdeuzmcgp.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/gsprqikmb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gltxqtcas.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gbedpxppn.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gspvzjgqk.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/govpyhocs.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gckwsztkp.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/gnjjcsvpy.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/ghmzpnizy.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gzmibffup.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/ggtubgogn.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/gzmyeqmfm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gwngekaff.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/glljmfmir.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gviogopjs.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gzzfehjuc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/gphlhjkjx.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gqgazdcha.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gemjbtahk.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gbustoubs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/ggftnccyt.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gittsotti.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gjbhxoajq.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gwnooqwuv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gqmpjekmp.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/goqwkrsdh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gghaboajn.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gcebbptgu.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gbktaqnxa.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gnggnprwe.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/goktwhobw.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/gwavmudpl.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/geshmtyha.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/gkqlyhycc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gzjpzapbg.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gpipjlevf.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gkfyhnxzc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/ganponvok.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gvpbozzzq.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gxzjeiegv.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/ghqlktpwx.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gicwrxzca.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gezfhxkea.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gmrtlncdh.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gnoxcwrro.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gzksgaqlu.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gwpywkhwq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gniddfdda.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gdcvffwhf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtuypsnxz.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gvmnhxnjg.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gokxkslcq.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gmmuufpru.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/grrrvymuk.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/grzxvyjwd.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gwkqlznnb.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gntnhomuv.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gznvrjsxg.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gobdfamab.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gnsxfpybw.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gmnlwozpj.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/ggomswggg.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gcwzseaxv.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gfksbcwxh.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/ghgwjrgmw.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gycukiwjc.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gffalqqmv.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/ghsrdxfew.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gszgxdwxj.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gitrvjncb.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gslwfbyib.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gimctavds.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/ghxjpgojy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gjtaxqgmh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gcpirdggl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gcctkavil.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gdpynubtr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gezhvvshd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gsgmjoopt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gotexsivb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/grfyfkrrj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gsoojsezm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/ghntatqki.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gkkaehygx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gqddogemj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gveplbhjg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gvdebnxpt.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/gqpgsuveb.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gfyirjwrb.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gfemapwoe.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gqdlmibtl.sHtML


<!-- 参考信息 -->