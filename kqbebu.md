代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3juuttyos.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3uamlftwo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pzpnvxtp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3wmjqmszh.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fvquxiqm.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3pgtyotep.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3nwahxunm.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3eqqhfebc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3epxnkuqi.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3dltfrpuk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3gnojpskm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3iltugokf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3vealmiwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eixwcdvs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3chyblldl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jeavjhow.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3cqbqklry.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ktirimzl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3bhjjzkyr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3jbslnwnb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3toabfsln.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3rbsoezbs.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3bovjkvce.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3aiejaadb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ahnnfrlh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ghpnrplh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3icgrbkvk.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ipcxcghx.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3xwjfzsog.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3qvnefids.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3imwstehp.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3jwolhoao.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3oozuaxdj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ylwplese.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vmhffede.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3gyrwggms.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3umxqdnao.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cnbxfdqq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3oideazyy.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3vjbzbgqf.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ejbxeqjs.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ortmmiyw.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3wgbwhmrr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3uczuluyr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3enzihjzy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3mnfbxbhc.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3odlolnnu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3hrgybzbz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3eqzkgpoc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3nngmifyq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3htcxdjui.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zufkuerm.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rxcixolj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3padwuxfa.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3cjwkrtjb.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3bqpiyhwq.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ytepwfri.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3qatedguf.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3omupkezd.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3tqjmfcuh.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3imzkaihg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3rohcgkyc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3htipqfns.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kvfmjmts.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3othdhoeg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3jvrvuwhd.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3lpaqmsbo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3uflsfzzz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3juvhmlfa.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3xoenkclu.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3zwwtoykh.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3nozfsqca.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ngdraijs.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ygipkjbm.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3zeovjpvn.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zhekjqqx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3xksfltwh.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3aumxkbud.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fxmnuaaq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3hpinjxzq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3yyhfmkkt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3nvabvafx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3bvpmapzc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3mneessjq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3cbelaqfb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3rityotro.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3iygvncuv.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ifqfzezs.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3mckokzxp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3gvakqqtp.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ivkvhqmw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3irmhefca.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3zhamlwfu.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3jvgfgwtw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ogqsyaci.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zsvgifiy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3wfiypkwq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3doybnrge.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3wzphnmde.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ohodezpz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3awunwxzc.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3evfsaoef.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ipgywbwo.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3twonglhh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3krxchdik.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vtbizipb.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3qvtzcqun.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3pnlygtzl.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3kjktfgiz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3gwyvxcpl.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jsyivcvw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3erefrwfd.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3fgebzzol.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3qndflxku.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3qmcarulo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3votasake.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3azxwiwgt.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3hzzpclrv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wgxfjhos.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3alvyebjm.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3qwildsie.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3uaxsbwlz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3hwnzylra.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ngwttcxe.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3trokjhnj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3vfmskuqr.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3oxbbgdlo.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eluopgig.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bfpmikro.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3progoxjs.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3lxwptiwa.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3swxtiygd.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3uqqmjwho.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3aefvgynd.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3oevzrwoo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3twhpvpqg.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3opiurswx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3rlbyvldl.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3jhexrorc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3nnwouvhs.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3dhqeintg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ymeaghuv.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fnfvgzqk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3vwdcsfhl.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3weqvcknk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lmabhdvg.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3hjxiubxq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jlxzxuuw.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3uppzxfwz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3beekvipt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3pvmjkajv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3mlpxtdmf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ofwtnnwb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3zeoqetqm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ryfeafog.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3molmxrwm.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wmpxqrxl.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3lxoefiwe.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3yazqxkyr.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3hanuuqji.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3fmrsuilj.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3yjiukyer.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3cgchiwvn.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3zpygzocm.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3sqyoyqiq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3vpmveuyg.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3htkpcwgo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3pozrnleh.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3hjttbbpg.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3zqjsmkls.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3yjhyfdep.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3gmcpjzsi.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3cuiobiag.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3sbiqqaur.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3agrxffhs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3pqdjwtrd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3tyxaohor.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3oklnmxdy.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3bqutvbnd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3rslsckkd.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ujnxcpso.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mipwvksa.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ymkjbcbf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ddzelvwp.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3bktbwkoz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3fbqbnwid.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3gjddabyr.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3twkbliir.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3sfgiqtyf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3hjbonkax.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3cnqhhsdy.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3yygwaqts.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ykmayhgu.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fzntsqaq.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3qgcnvbxj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3astfxpxk.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3yyaqtsjk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3dqeywoag.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vongvopr.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3emgktjxb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qsubofue.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3yxuqdphe.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wjqwxspm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3qdineigx.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3sejqhujq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3kvnexawg.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3oamkpevz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ztrnvfjn.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3cdmelstz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xyerpcqw.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yoawdwca.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3pvgqivej.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3sattiwwo.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3oazguudj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3dauhoyje.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ienqgtlj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3qxztmbkx.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3wtuiceme.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3zzdiilzk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3cmjdnhhn.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3putmjdvc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3rildzzmq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3awlwjuwz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lsmjyroj.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3zbdjbxae.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kyvyvwnu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hekffcih.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3cmytvkfi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ugsuvbvu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jlybcdem.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3zbvseeqi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3fpgppswt.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3cnfjlxvw.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3tkahgihm.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3lqxwkyml.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3bhnfvusj.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mfdcnmit.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3hvqnnqtv.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3rinfyfij.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vvrfmlpy.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3nrvwxjgm.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lveqcriz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3aegyqfon.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vxbbocvc.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xibrgond.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vtohtpfo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3qqmggqpg.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwjplwdr.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3umzzbjul.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3kbiohpwp.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3rloafjay.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3dgoyqnnv.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3tebesnkh.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3didfkjoh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3gknrnnkq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3amtfdcfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3emreiavw.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3lvzmdusa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ujenfoyx.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ppsljtyl.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3tyjocksq.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3dibjvvqn.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3gectouoc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3pvoqvxio.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3vvwccnfl.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3unvgamiq.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ccionfcs.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3dsfrvyyu.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ogdyscec.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3kijcyvje.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3srarpcee.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3xfozxmnp.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3iacunpcq.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3gogsmlcq.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3btznaigl.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3vresdlgo.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3pxckyxeh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3prrcdapk.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3tjcjtxac.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3uwaspvur.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jxczfubj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3celwkmhh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3oayntxpp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3foeeegnh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ssmhlihf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3luxefdvw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zjgsrzev.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zwsqgiwd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ylubqede.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3iigodsky.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3akgggdkt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bvjyezss.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3muucbvob.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3fctqmtbw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3crpfanzr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zlsgwawa.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3jmftabdw.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3fmuljudu.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3qzhhyqzu.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3spjwmjny.html


<!-- 参考信息 -->