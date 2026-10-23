代发 wailian999

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3lfwddgmi.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eokobkuy.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3bdhpcvcb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3slmajjle.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pvomcjrw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sgcwhczp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3iasbpnil.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3lludmyup.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lvmjsmuy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xanptash.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3llbtjbqb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3myfwwpte.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ikerzlni.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3vfdejqfm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uhdypxix.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3gcmdkctd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3sjokvyie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jgopjnqy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sgfnhrsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gpealrvo.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3tyaamkre.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3gaixhfxu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3wvyrtvel.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3unnhkxlg.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3gfxigwyy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3vqwgvnrq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3msqywwap.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3wpcidxkn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3bttciiqm.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mqmkegfm.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3lpvzhdai.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3mkwayfft.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3drwdujwe.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3kydfnprj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3nxyvmgds.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3rsomdfwx.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3unujlkcr.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3pmdjiouy.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3mzpqxnvc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3jhsrbypd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fpbrahlz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3feejryed.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3npnhtuje.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iqbmhrwl.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3rudkptrr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3tnpqgdee.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3krlsjzlm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ujtmkzmt.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3kqzjqvsb.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3mdlodnwv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ekdyludh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3asnncnrh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3bttsphwb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3kqiorepa.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3jynykrxu.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3jbehypqv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3dgnybjsd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ddihigpz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3hcssyjto.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3nyeopsld.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3hdgrmrss.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ugdgocek.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3yyesxppp.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3pyxmegnm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ufzvfysa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3mblbzgou.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3gkexchsh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ntrjfmdv.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ljnbvjdo.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3wxngqmsx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ibtoxmbx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3gpdmdhhp.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3rqtpzyyz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3zydbfery.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3bgevmmly.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3gekhivgf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ktaztkkl.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3azcafhoa.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3quokyspj.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fbvlzadh.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3hxbrddlg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3gwxpowwy.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3bqzlfrbc.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3mrbddtcd.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3lnxiruni.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3zpoloeuo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3anpupdqk.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ldkkoswx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3oscopncs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3mrivolkp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3psxfjspg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3lritrrfq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ramatzrs.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3tzbxznrg.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3gezxunie.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3banyurjv.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ottebcvw.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3vfngrigv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3vhymlbbs.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fyziyznv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3urscobxx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3isjcvyms.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3bcnmfcvq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3dmapwilf.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ployrviw.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3eejftyqo.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3mzwktxab.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ihzbkpzu.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3yhdipsbw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohtpfmih.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3whwgmdtw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ogaojugu.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3jaaesbba.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3qhfalarg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3pwvieiam.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3vzmakolo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3tyizelfh.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3mbrtvlxc.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3vwzvxjzl.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3crnpphey.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3tnunurbw.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3sjjankks.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vvrubveg.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3hxyaefop.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3tycbcgoz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3adfwjglb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3sltrnkmd.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ddcnqtvc.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sfrvzeeq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3uluxpmig.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3khdsljpv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3erbwycpd.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mpbyconu.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3lzdgshai.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3qkittbjd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3rrvoefbm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3jwgnjxub.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hslawcsy.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3vjeuyqvh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3eicdpjgx.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3khfbzhsl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sxfspkdx.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3efbhvwxg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ryclslmi.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ggsnnkiq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3tksdxhjg.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ltiusxqv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3bdirphcp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ozxnlokh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tosmppqi.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3mxwjstlb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zjgddhea.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3qefwzcso.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3eoqrpygp.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3pxlktvmo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3rqkarlzs.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3muypiqhr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3uhbbxupl.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3apnlbdba.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ctpuwwam.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3qbogrwyv.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3uunifqxj.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3pyiwsxgk.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3smpfwkzn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jhtqgtzi.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3awlncnnj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3oqecclse.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ghwvyoat.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3yxqcvzly.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3jhcavgxt.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3vtghehhq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3pyerukgt.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3dfeuoiyb.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3qqfggeqm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3brhgmani.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3xdrkbzgg.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3lrlakqhk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3cyucldsz.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3bsjcydpa.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3rsxirwhj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3azydosdv.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3hkklpfec.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3fcrlwcoq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3dlwqdscj.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3lrkysjhx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3krfejelo.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3tbhvztkw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3xdengofn.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3lutobsfd.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ucbrpvpc.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3yqrkysks.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3fyjzzenv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3kriqtjtv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3noyrmonh.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3gjgzfheq.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3vuxtmcvn.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3gbpwnngg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kbasrbsx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3kcqembgw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bdbkpatd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dgfpbuig.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3vuuaoyui.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ttjhspic.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jxevndks.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3fmgotlem.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3omgvwoke.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3dyishvdn.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3seuidpkb.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ozvlldjh.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3lerkezsh.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3cknmpvqf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jwblxmox.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3komdvftq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3edmxjohb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3aqwztrgq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ljpishap.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3tmhlubdo.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3fuonhgyf.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3xdcrakis.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3bpwkkejo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3xhlmjaae.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3lurnwejp.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3bpgcbnkq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3jzktkhce.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3cgvltvve.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3eeifalah.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3sjetgmaj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tcceuyta.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3rbbigfwh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3sbxgsggo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hmygfqre.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3pkfudnfq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3umaxsdzr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vkgfcdwi.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ehqivftv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3ifsdykqz.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3gdfplbkj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ftjbzbxa.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3bwhdauav.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3mphfdwgb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3uawlwnbk.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3zsdjuatp.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3zcnsndga.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hdxwnkts.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ylqooumg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vjtyfete.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ehumzdwm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3emnzrhcg.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zltcsyzg.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ldhigpuq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3zuifpyhp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3shdlwrzt.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ffmqlaja.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ecmfqnno.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3jlkxjkrk.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3tvgfweuh.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3blujoexn.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ytmcuutg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3tosntwax.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3nvhmmuwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xabiakhb.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3yfviapsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3logillhg.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3hvucjqrn.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3vrgqsxhw.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3aiqisomf.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3thhmbiqv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dvlsanku.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cnrenvze.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3cddqqgem.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3mvftwzdr.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3fjofrapr.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3igtgsnkd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3gsridjed.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3cevdcvpe.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3zjooonhi.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3rfvhvjnl.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3gftqtlhy.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3tfnqsuet.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3fljbalgz.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3akpgujvk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kgkwvvue.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3swttwuow.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3nrvtplnv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hvvjchyf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gpsgxqdz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3pespcdye.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3uihmjwjb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3safkeiic.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3uiaspshy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3wtroljci.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3iqygqidt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yotrwtgp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3hoisejbd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qormogbu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lhqkuxun.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3onlqeerv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3agawhjji.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3aobyjxwd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3svfwfuhy.html


<!-- 参考信息 -->