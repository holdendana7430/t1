代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3nmzdoiki.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oodtypbf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ouwqrdfr.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3bjaftrei.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vzgkmhsm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uvwvpuuh.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ymptsqob.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lqatollk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qyitxcvj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ruxfaokb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kxzgigyu.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3oabbxocs.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ascdnflt.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xkbytiil.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3dxuipfhy.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3pdlzcuwn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3xtumhnqk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3lidvpgaf.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3gejnloyf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3mdgjukxj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3wnxpwlle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udodyiju.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ezcwptbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vixahrmf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3komauuey.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3zdofqiqr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3aklirgnt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cuwmepmv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3avriguim.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3wrsyoaza.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3hcqykmoz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3gfmjqpbd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3pwhvviik.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cgqmbido.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3qhwrwvyr.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3cebbweop.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3nidcvfxa.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3yrrkgahj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3plvkoobf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3asinofyc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3kmlnklne.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3bywgtgsl.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ttdrfyad.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3wijvgcfy.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3mxinstxr.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3olhoknaj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ckpoeugs.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dnyfbdoh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3rokpcuez.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3slayyiwo.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3zfegalop.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3etvskarm.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3whojmmes.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3pbvgxlul.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3xwzuoshx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3jbynvwnr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3saiirten.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3zlmqlucv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3rdvccnoj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lqhqgpom.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3npmzmggr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3hawteakw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3crbdbqbr.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3uzdpwxdi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3kfmztrrb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3nyqlzzcp.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3fmtagjfr.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3lcngymie.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3hcwqrmlw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3iqwqibhj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3amcavdut.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gygtthtz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3sellgvyq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3mdfbsphy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3zfbzxwov.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ocnpprxd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3rqceahxc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ohgmqnqh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3yjrnytby.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ihkpjymr.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3bzgmmkwg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3vlpbsyuq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3efwvgwjd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3jfdnxtfj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ticgdotu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3plmujfqh.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kxafkyyl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3altcezdb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3wkmfowcx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3xnsxmmiv.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3xwageoyz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ofngqyuk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3vumnkavq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3aggjvmeu.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hgbumxpf.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3fmhpdcfm.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3xnaeagcr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3qywwagni.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3fjhywybn.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3tanffdwd.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ozjteqts.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3derpqruw.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ryxkfidq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fwnfqirm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3opspdbun.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3gatbsmxh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3flirlqsf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3cuspvogv.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3yymdnnfz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3hphxwhsn.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3dtmaetcw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3wzzqasbx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3qcqfrnzm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hswarbwm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ebyffrav.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3byysqkum.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3mmftxctc.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3hdpfwqjy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iwzollob.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gntfkodt.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ipvcjnzn.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3bwsbfuux.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3udpycgkh.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3foetwxyz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3rifciefx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3pywwujrx.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3yqylmrub.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3kwqwbwxe.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3qzpilnpg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3fmrpttmx.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ipfyigby.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3wiybfuay.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3lxflmrzo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3bwnlhvpl.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xswvnapu.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qstvisld.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kavanllb.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3tsxipcwu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3gpbrffyz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3jjhloxrh.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3yxyzccye.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nvasmbxo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3tpereooo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3huozfwop.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3slifkltr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3fhwmavgo.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3xwicvrby.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3igymgcsi.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3adwcdgfx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3mxojjril.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sesdkawl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3zbodivwl.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3yidpbpid.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zyuwsbsg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ewbcseec.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pkbrdhod.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3jinjqsyh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3htcppbaw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3hbuniwal.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3qtsrvtjp.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3narjgqfp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3bhkfcfmn.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3hgdqiblb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3hpxnptwc.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3vncbepcw.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3jxmezjht.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3vpmbqokj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ziezzevj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3toxfyfjs.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3marxwuxy.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jqtrwbym.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3pefqzsfl.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3wgcazrcb.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3gtaoyunq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3quurfmwh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ivdcmgnv.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3isnkelze.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3rxfexcjb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3tfqwsanx.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3idxtlhxk.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ulmptkfz.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3xndmublf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3iwdqsqxv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3lujqxjrc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3yypivsmk.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ytkmeivb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ljwxxjee.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ndippwxh.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3tonxslpa.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kmpkqxrv.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3dsyzkhxk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3tvcmfnjt.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ohyvwpxs.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3wbslqyep.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3alhnbfqc.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3abderhgs.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ywrsyhdn.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ixucqyui.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3numbbfvb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3gkcyquww.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3fmnsgbre.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zpydcedj.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3tjlwgewn.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rpoboigf.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3jidnuwgl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3rwxwzojf.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3odrsjcqb.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qairyeox.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nwjloxik.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3vgotaszl.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3hyhplbvt.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3rwerdwry.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3kmiajdxk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3onyopidi.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3zqykeofu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3amknhiek.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3mdamxyyf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3aqipnngj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ytrkkuhb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ajtnxaaz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ieghmnbt.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3wuokoylb.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3xnaboaao.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3zdczsxlk.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3rsdcgeop.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3nxtpljuq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3broqduqp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3lkpwokyl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3covgvbam.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3jlphscsd.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ricqyxdp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hvsexted.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3asewlwme.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pypszgvw.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fsnuykng.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3zmdojmbn.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ohtstdgr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dnbpddgm.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3rtsrhqbo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3mzzarted.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3kxljruyj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3subumcpv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3devhjvzk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3jlwmolsq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3tpkkknnr.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3kusnsogq.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3hickrzha.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3eyxisscb.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3hwmnfwxv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bryxsecy.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ppbvavuz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3fufodjbg.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xtgtsqem.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3icrtctuo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3qencvsds.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3zckquqnf.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3jilydrgq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3coamldwx.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3pbwioqyg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3smlkmeke.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3gumurqdb.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3rfwrvhtc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3wanthuyc.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ustzvdpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ebyoqyus.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3iokulwrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ipvjbezs.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3tmawqbos.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3kcogoibs.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3rnaerbtf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3piewdeuh.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xgdixtsd.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3wiwqrjqd.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3euunwvvj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cvfhmlip.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3gaimauyv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3vsdefgtd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ugzdopfa.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3vvphmyte.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3korgjgnc.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3nixrxckh.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3sktolwxq.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3foeanqtd.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3gxagpczu.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3gpdakxmz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ylpojdxm.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ysgindjg.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3dakppztc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3yvblrzyp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3akgdszgn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ttffalfo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3dbvwgcps.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3vkxftaoi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3lpmfuafv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dzrdxvde.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3yajxrhle.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kztfgpxg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ejejysau.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rwprjkrf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3uaufpsks.html


<!-- 参考信息 -->