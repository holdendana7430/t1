代发 wailian999

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3idnvmoud.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dxkgvjod.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3oidnkjah.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3igxzdksd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3lgwgoxho.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3yclngtal.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3efqvkzzq.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ehadiiaz.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wprqepcd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gsscxdpy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hjhvbwjc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3seigdnxm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jywrucku.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qpbvevnr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lvyqjipr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3adinqquv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3bemhosfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmyzzsjs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gkmizggm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3usvabnug.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3xovwdpqj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3cwsdntnq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3bwohnxkm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dnfxgxvv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3kwgkxlop.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3kfbnqcqh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3giucrfga.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ondocvkb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3garzkfog.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gskcubzf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3vbfjzbzx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3icaechyg.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3vmkxoixx.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3zgbycmkv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3kuroagge.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3wmedjxbv.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3qrmzryhl.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3gycwjaac.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3azzegnke.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3pryurezx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3tpywojno.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ijamecrw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qdlesbvq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mmmkurgx.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3yveitvtp.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3iodebtlr.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3kmessiea.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3pqofnjog.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3bggeksqe.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3zhhmoong.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ubmobklu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3rbaqaltt.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ffsvppra.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3rvzgvcsa.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3vrliwznn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3hfwsaohm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3wehnlwvm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3rpihnmrk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3wynpnvva.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3cpjasuyp.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3leuzlltu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3vuvjuuog.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3fmlwelrc.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3vwauqcsy.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3khcijwry.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3zjwyxgyh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3wokaxqdv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nqgpioad.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3rywerwus.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3nsomxyvq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3kseqfatq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3gybkxmyv.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3otrmyrhg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3rlyghgfz.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3zozqwnns.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ojqupjhk.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ispvnton.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3pchucsyf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3fqozzazj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ebfyrfcl.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3wvyvyyea.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3czqlefoy.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3csksadvy.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3kisuwdbm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3owhhfwmx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3nxxgssal.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3fqundmpo.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3gumxlpwu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3moalztob.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3igqleelt.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3xstwvzgr.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3opvnhbew.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3bmhviadh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ptjdgrpy.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3togxpyhk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3znjwfviu.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3jewcwyrv.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3gpoaynsb.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ebjjgmfy.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3kntbbnjn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3vonlppgy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ohqexvey.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3slsuiykk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3bkbqsuiw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3meysjnhw.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3rurgkxql.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3douzgbmj.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3edkiuhij.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3esqwdlab.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nbsczede.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3hqmpxmdd.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3hdaqmgjj.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3iqyvlrjx.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3izymbfui.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3mkbwphyu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3bgrdbvbn.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3wzlmfpqw.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3mfoflzpk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3qzovwcpb.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gowbceds.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3tmlymgqk.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3cdgbkvvc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rfxeygjv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3yceojjev.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3mgbpvycc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3hhgianrl.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3bnhrbwdo.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3erbcoymd.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wfltpcvw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fmiqbygt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3irpwljlj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cifetsrk.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rkaiezhi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3xxmfqbhc.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3lazapudq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3irwqskdn.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3irsitqsj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xgbayikh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3zjhinckg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3akqzyiqh.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3yhlpyybb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gozurljj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3dtyvqaan.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3epkzupeq.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3brhtavkc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ndxxxnrm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3amtjxxlu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3njzbbwqy.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3lmhahvuc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qcbgwscc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3xpwzhwhb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3igjaznjr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3belwdhxr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3idimgssp.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3zmskoyyq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3lfutmgux.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3scthahtx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3uokanueb.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3gypmykec.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ybhhulmj.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3cywqdqdu.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3hhvvrrlu.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3bkbzcqqo.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3hzkrbyce.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3lvoaedvo.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3gfmhuung.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3usnwkgrv.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3zejkuygx.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3vpbpvebt.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ftbkfvgc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3nnooipqi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3pzikcnbj.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3xokazwjw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3hiaokasm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ktoiokcd.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3xffefeyg.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3zwazlfzb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3dlhfjcll.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3trrbyzof.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3chtfrimi.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3jmxvtdju.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3kxdjfguu.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3oofyfcqd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3vgxdqcit.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3lglklkat.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3jlvicnoo.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3okwodywj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3iigtxnhh.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3reecdlvp.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3mnljyecw.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3hihvfzrj.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3fbvyiiiu.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mszighxd.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3jvbdxqkl.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3sldhrhdv.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3czacqwnz.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3yiofbtsq.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3piitxgxe.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3ksqdunnd.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tmjslhrt.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3xwctarrt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3uimhvqmy.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3jkjvkcqq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xjcozxzc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3gdmgynfc.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3vpfkwndd.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qbmyeteu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3njomvhbk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3dzfqxppx.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3dcbyyjhi.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ykhhomxd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ieukadqs.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3rpedlldw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ubuvjqsf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3aurrpiqs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3lecrghjh.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3jfymfsat.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3suprxkbp.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3qtjobuws.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3xvufqmed.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3awrfggoh.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3rfnuhtvp.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3tjidbfps.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3dwafhjtr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3zqewqzyp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3tpsnicdm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3sxnreggi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3birfmjnd.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3sjkpuepj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qmklbuds.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nutkpwpe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3wbypsbmr.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3acxesvqh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3kmingykq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3caoszpyn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3acwffbnm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3oymfvgwk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3tbcrhsvw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3xdappmig.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3qalvlozp.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3bryhzknt.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3nwowqvim.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3lyjjtepq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aphbdqqj.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3yfgezwes.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ugvctkzm.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3wmecsjja.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tqeftxqi.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3layxodsw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hboefbty.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3kwktfjgq.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwipdjgq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3kbdcpxni.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3iusqkelr.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3vrffnuwz.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3fnynqonj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3qoljlsyv.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3erwdvdjz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3jcwlnuvq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3nkinhjno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mdaldblp.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3xsgzkpub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzgotelx.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3giaoebtv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3azynesjs.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3vwdfjgaw.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3cuxeimzs.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ttwzfdwu.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3oyssgmrl.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3yefnrfiv.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hzpnbclp.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ddduulbt.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3vffpovkp.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3xyuapzni.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3wnaecmru.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3xkkjbzyk.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3nuyadapm.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3qlrqgdtu.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3wqbiquqn.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3vfupfjtd.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3awfeojbk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rxatnrfx.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3iuwhbsqk.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3zwgplxhd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3yxbrhvds.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3etvdcbjd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3svxlmxdv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3nyyytgly.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3fziladic.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3hybpeppm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3iqbijfzh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3oanjldlu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3thxygokw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ghvcojji.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3eirtdwzl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cddwqhiu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3aebmmjbg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3fqgwvyzr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3kekizinn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rjkkwxqo.html


<!-- 参考信息 -->