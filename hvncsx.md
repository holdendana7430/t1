代发 wailian999

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2kfnzgkek.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2minneyix.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2hglssili.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2alxietde.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vxkebcbm.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kgstodod.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xomqczae.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2fmroztuw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lxhujglq.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ewueqtyq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mobjpmwq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2jnacbysl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2guxwkxgf.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xmcnzrnj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2epbdvssh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2rzeedleg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2jswhgczc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tuyldidb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ippxfzty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2csjjeosk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2upbeaqwn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2rlmwxkru.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2khfgixlx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lglyelqi.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2jlsretnz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2bcmtzhol.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2tfeqmedb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2exctpzhw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2mxvyolio.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qsygdmpt.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2fwrxsdbi.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2amjcfvjn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2znbjwqet.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2mviwhnrd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2hmsbfyqm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2tnnfcnbv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2yehjkrln.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2kzpouqfc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2rubjlrtx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ponqdtdy.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ltlpsqnw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2saohnhhd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2lwthryrd.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cbpoagto.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2szorghwq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ppcntkpr.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2hoysjwyk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2uwanixsp.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2vzyaecxu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2yxczjgff.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2imqhcctz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2xtpbizfz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2rjkhjxwz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2opqcczch.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2auyvwtns.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mtyboule.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2zvviqyvc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2cwpuuzgv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2rqdgtzgg.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2cwyilcjw.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2leaincgf.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2vndzoviy.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2qztjqrje.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2oqdkxxus.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2qxybwcfx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2iifmtpcx.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2cyvgslmx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2zcpxwmxu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2vlzykayk.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2awglbmax.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2polnqyko.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2gsiwnhco.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2tacqyqup.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2dazfkbly.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2viiqipbm.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2jacdmokx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2wzwvnbev.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2eeikwsxz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2pnkrpfwq.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sijmupbv.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2hneubeml.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2kojuahrp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2tivvsbyp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2lxmvkhmn.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ykqdapkq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2eimxzfhv.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2lnvqvqph.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2fvxzbypj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2tqffgzax.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ugnbttky.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2grbydpes.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2casvbszr.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2xdxqflqt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ujrwtqsy.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2gmqfalvr.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ztkynhqi.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ifzhlxwl.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2czpiqtag.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2bqxjpyly.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ilfbrvth.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2omqugltm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2xfgdeysp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2iarqgkcg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2kmdgxfcc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2cnhcuyrl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2rtprvbcq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2gmgfsbxy.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2hrrzrdlq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ymitmocw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2thsjjiio.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2tvotweje.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2tltcirnd.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2uulcxefy.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2bgspbbpk.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ruzmltux.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2htacirnv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2aksfhmfe.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ltukmhst.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2qhzgsjbn.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2dcfgfbpb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2wrisubye.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2awzctthl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2dzcskwme.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qlfjdmyp.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2xfwktftv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2bzatunsb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ylxztref.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2rheyohsj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ofqnuext.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2iyegxhkq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2qiazbipu.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2howlzhzl.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wkqueavi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2eypebphj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2esaqroae.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vrekcmes.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2bnxxmajf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jxkuerfh.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2kinkgokh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2jroeawao.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2qbsjcjlh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2gwasamme.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2zdecfflw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2gocatkop.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2vlcusjdu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2awesfbzo.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2bxxshioz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2uvvfnhro.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2vrcfjktk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lhntpzks.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ejvicaek.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2qkedxjnc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2vcupfaiq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2shankokm.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2uggvxtqw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2fsovfmgf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2xhflgnuv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ezrxbokr.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2jzqzrlaw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2xygnvbon.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2kcfoizve.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gdsggnpv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2xijeprmq.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2emvcweot.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2xiqjbpye.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2yywroyjd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ikflymfb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2dagbapbu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2fxjcqdba.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2stdxavvh.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2yjckkibw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2fcvqbngr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2fokiqscg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2imlrfwgq.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2djcixmlh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2toqnaqik.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ltjsndet.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2pxjgdpgr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2bmzgfmov.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2pfejzkja.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2cchndhop.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2nxzlipnt.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2dqsgigcx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2irpvqhls.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2mkgzuxzh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2dxhpkput.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2yrlkpsrc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2anxfpzsf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2cypdtrbf.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2inokgdmc.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2jkurymrp.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2pypqrynb.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bvdlblag.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2kthsdmol.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2wjmsqbkt.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2fdppzatn.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2avzzbcbp.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lnhtuffd.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ehbqbvyi.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2iahujlep.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2gegodoso.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2voobrvod.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lcvsxhzj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ikvknhaj.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sdhlcmqh.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2yopkihgg.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mijxaszv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2yfxmvwyo.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2dafxlszb.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2uwualptg.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2pupllwnb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jravhliq.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2aiyispvc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2urrgbzgx.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2wpjitnjn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2sqwjffqq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2worhalyw.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2acrwdbhs.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2sdcdrddz.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2yyhqsetc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2mjopggyu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2qfoapqdb.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ermldjym.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2gppybjqj.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2hizlzhlq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2mnitdzzz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ceavnndz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fxrvkiko.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2kjeywyts.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2afmdtvab.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2emozyaza.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2cjcfittl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xysvwrqz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2toeebkxd.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2omitpqrg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2qrriiaze.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2inhfftpx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vtijlccy.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2dwymbvpm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2hhhujxhj.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rqyubjzw.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ltpoxwxe.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2hsmujcdt.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2krgkklks.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2qaafwird.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gnvpknxy.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2kauzzkkk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fhbhwkqt.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vckivwjw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ktgqrhgl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2oeynlrfd.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2spacrlxt.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2sbfivxzw.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2nbycelyd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2zjbzdxvl.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2jdrvncid.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2cjbpgtdo.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2xosrkwxl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ybthcbzw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2rsqapffi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzryxuxx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2eckzhdnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yavsbrjh.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ksegdwxi.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2vodwakgi.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2oguuvkpf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2zytpqbkj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2npldnsmv.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bymyclnn.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2naogdfoq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dxufjlxt.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2nidwzyhp.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2iowapvgp.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2urcxhjpd.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2xxuopgle.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2paxfnfcv.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2odvpahrv.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2dhbagulo.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2cdnwacju.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2nmeokrqb.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2mwqryuix.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2aozjwxbg.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2fuazeeif.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2azwetycu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2dzhpjeqk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2udtngaps.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2msevhgcz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2mvwsiiar.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2pnvrrujl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2xdgrrwlr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vcygelkh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2sbizdpwb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zbliirhq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2zbgxajfj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cjnatgdf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zapgswtu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zsjyphrz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2yyfsvvcj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2qqarenef.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2uexehorr.html


<!-- 参考信息 -->