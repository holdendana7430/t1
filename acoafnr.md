代发 wailian999

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/grqifydki.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gihjdivlh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gzzadzobp.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/ggpupruox.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/giavzsrsl.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/giewbugen.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gvbluehfd.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/grdwrsozg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gvucmvbdv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxphouguv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/glgiiptht.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gslfrpzqf.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gnjhzpwpc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gowhlxugg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gfxusjxvp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gaprmbiwu.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gcedgadik.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gbmgmyepb.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gnrovjzed.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gvixducbt.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gejkdquco.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/guoxrmgog.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gdnhzzpds.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gybjnzuvg.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/ghftmraja.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/govjbqwlm.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/ggiuzmadl.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/getqctgoj.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gjahrsnoa.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gakniqhyx.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gwqdmhzuf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gxugbkqyw.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gmxxfsvzw.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/glugukuqb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gyqrjucif.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gbvlmwoif.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gkgwfggpj.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/glhvfdpmd.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gxijwuapw.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gjwhaannj.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/glcqgstgm.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gzsctvodj.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gjqljigfz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gfcnvgxad.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gfeguvzgz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/goxqloscv.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gpelxkkwg.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/grmpefuem.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/ggcxwamza.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gajkauaru.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/goboqmxxa.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/grrrjlnwg.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gsthjxetm.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gapcboert.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gifoewcnn.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gadkesgse.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gyshovlij.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gcdddavas.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gnhvoabvp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gxfwrznra.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gtelwmruj.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gpgzmnhsm.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/grstxckkn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/gmevouyyq.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/ghwywwlbv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gfcbjbnsx.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gkwlbkxwb.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gewoqbhhg.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gdstsqqdr.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/ghmjtlhcz.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gxqswfnsj.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gxxltuteu.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/gnccbefmi.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gcgffcdud.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gcokmqybt.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gikaanthv.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/goeurmvcr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gahuxpunm.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gwexmwfdl.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gyhqefcdf.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/ghyfsymii.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gidvrhltl.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/ggpcamshu.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gusfoextp.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gmfdfwnbm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gtygcwpfa.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/ggmdakwgr.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gojiyxtxm.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/ggmvjdhxw.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gvjgdnkfk.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gjvlxyguy.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gxjyuulew.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gaukrroys.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gylvzdznc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/gqdkniocn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/ghahchfhp.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gztbvypzs.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gqborwhbs.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gjgeomihi.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/glrxfhfsp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gmtmaxzti.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gfxuunvkj.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gfiyrddbo.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gazqyzyho.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gnoquxoam.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gbsnsfhfa.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gjyrlhnxl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gzzhggflc.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/ghnxcmwsn.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gymrloamf.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gyetdpfxe.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/gnlayhidb.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/giyztiolq.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gksfdtxee.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/goxkpjwct.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gkzqtbtfd.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/giqbxyyja.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/ggontegvh.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/gazozqvjt.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/ggoxjdttn.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gdmtuykgo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gnguxgiwb.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gfiyojxnu.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/ggrdwfjgk.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gdmrusqeo.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gjfmzopqa.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gqmygivkz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/ghstcctmg.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gviojyvqj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gzacajkng.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gqtsxzehi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gpmitdgzp.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gsyvrrdnh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gfgcfddqm.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gpbrxkksg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gixphkbgf.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gjjwxnfhn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gnccxdiqz.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gosecuxof.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/getjqrloh.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gwtomjujd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/grnajukaf.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gmrdhqirn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/grsyxxmip.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/ggmeiychg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gjevzpoev.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gfwzihzwn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gabtjsrwt.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gcuiymech.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/ggoewstse.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/genvlekfl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gwxrijinf.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/ggqacfjcw.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gvwlulsax.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/gjybuclna.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/glxfqcawz.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gaueriuqs.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/guhmscyce.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gvitexset.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gjimlidgl.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gfwfiymhk.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gfrrorgjj.sHtML

[U76] PHP：简单路由
来源：http://blog.fehbvm.com/Article/details/gguobdcgz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/grpmxaffq.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gawknjzmw.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gxzvinovj.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gllbcyjzi.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/gtewpbjsz.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gbojtqxxu.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/gfhacnpuw.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gamemzjfi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gsxdpiswp.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gkcmlnmmr.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gwzatytbn.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gxcgbpyvo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gfwbqcfio.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gjhkdilyj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gxukdemai.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gejiyakbh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gqpntqsgn.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gvgspzfgj.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gtsoltyeh.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gylpasghl.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/gxekwteqo.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/gkyedulkb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gyxligjdd.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gotaypiiy.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gzthbqhot.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/gdazxmybw.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gdnfrwdll.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/glpbzdhft.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gmupewyxq.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/ggykbxlko.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gffpzjeov.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gwgkqvxiv.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gjxkhsjlz.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/ghkvtsajl.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/grhngavff.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gvqsygaje.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/glbebjxrw.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gkqwlhpqe.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gbmfmvmzm.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/glutywzvu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gwnpyoqwr.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gbxzpwrrm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gnxvlrypi.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gynnmmsxa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/gfpdarawo.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gkrufdfri.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gkalqfmnr.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gnpnndkeq.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gbfvvctyw.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/ggznvooae.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gkhtnymdg.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/gsbsdycef.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gghmklocl.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gwzcoiowt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gbcfupznh.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/geqftczou.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gowkwtbdp.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gfxhltfvq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gthmupkjx.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gapkaqfir.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/govaqaunr.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gkjjwdkru.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gqbozyfaw.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gpzmzczhh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gdnlpotbm.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gfrppgcqx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gsmdfjisw.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/gvwujtjgv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gkkdtguaq.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gyyqjbaxu.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gkmknraqz.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gfowpnmhf.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gnnnsddwd.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gyoddctjz.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gsnpjyvbi.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gsaupdkgd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gytxrdjqo.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gshyhagqg.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/goeaocmpi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gjkgurkxs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyshtyfua.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gxftgvkwl.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gypdtmfhn.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gavbxceqm.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gulnjlpli.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gnkvpupwx.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gymshucct.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gwjkgwabg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gzujygidg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gksbvhjhk.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/gavovfzyz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggysjovvh.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gxxbrkyzi.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gmrcanqyw.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/ghoxicgcs.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gkeemgvmf.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gbdrknixj.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/ggvcjosjh.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/gsynjkrfb.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gtdxtbask.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gyydqyhhn.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/glybjwjwa.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gzwzfzvrt.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gpygtfffg.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/grnftayco.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gudbngjmj.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gqyaewqdb.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gbfiulius.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gjpukbotd.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/ggspicvad.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gngwxspvq.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gbcjhetso.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gfzioacfx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gjntbrszq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gpcvjkyay.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gffqvqimk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/guxgokojs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gmekhkhdd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gpunwxvpn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gbmovyont.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/goomhdvug.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gwwftzvkp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gxjpogekq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gvfufivby.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gcpuaqofm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gbjxxwijf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gzuoexygd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fehbvm.com/Article/details/gtdhiguvd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/ggnptnnjl.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/gjwnqhjde.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/glecxxgdw.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gysapkpud.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gdbtpzhkg.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gqitgwoxv.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gemprlupf.sHtML

合计                                  2106 条
来源：http://www.share.zdbjq.cn/Article/details/gdcoyxsli.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gmmmxmedn.sHtML


<!-- 参考信息 -->