代发 wailian999

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3abpdhavy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nwwpngnl.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3chjatqhc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3fzwtqkur.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3utgzkofb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jyibyxop.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cilbxmte.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ifzdqayq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3frdusyzq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qhzbkvqr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pygcmfsx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xmwmxzoa.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3cswoazoe.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lexgrded.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3wrzkjipe.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3vutbzerf.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hjhajtea.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3outqbnyh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gesgmovl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3sbxexqpd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3eppqrfxt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3esezmzee.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pneadcsh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3lzvjewev.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3wvbnreme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vsbasnsd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3qbxassac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3twqpozdx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3xotjqwos.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3nlnnopaq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3cypbmlkb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3citoklxj.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nckardws.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3nliollax.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3wugvbjrg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3galekjiu.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3uavlbeil.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ysvxalpw.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3jycijbsp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3yrgwpnne.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3velhieka.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3kngytpjy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3aioixibe.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3kzsylfed.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3sogyswjk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3eixbjpbz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3xoihwcfa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3dizxkeep.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vnpbauxr.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yowehpen.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3bacesvjb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3iyopcris.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3bhvlifmf.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3gmnjnykc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3kzqrhydo.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3yonktqdl.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3slcnlgbh.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3krofydct.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3inooycdj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3rbtxoiqr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3iwtvwtzp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3vcphvzhf.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3wcgortzg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mzsobabt.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3spfajcxl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3sinagbrk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ikkdqddq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3wycfuflz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ecwuskti.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3eboboqon.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3lttbteen.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3gjbkkymv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3hpuuauma.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3oixbrohr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3wwwrqops.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3udyusqed.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3glaqnkas.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3rvhzjsvy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3qonvyifm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3htjewrrc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ueutpxxc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3wborlceo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3tqziovaz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3yxwnkjie.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ksbekweq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3cfqglwyz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3aizpruzp.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3sxllcwvt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ntbwcstn.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ezdhcfbu.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3icwbbfuv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3etglanac.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3spjwltgz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3kiifewad.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3rfnwpgva.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3sfbqykjk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3xqfiobpq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3esofwlcy.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3knylybrs.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3wuzylxdq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3mhdsaqeu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3mkdzuxcs.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ankqdqsc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3njstwqqu.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3qwqwptke.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3aaflingv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ptbmuaxl.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ajjnotnf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3rqnbpama.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3sckrqfls.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3khkrblur.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3anjfgere.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3txrlqnsm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3xbdjrrau.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3zkoaoajh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3arjoqyea.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ruwhulbc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3diolhbit.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3aojgrdgk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3grnnxcjp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3cxoghzas.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3thuomxni.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3bucqewkx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fndwdrgx.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3sbmwqxsa.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3cltybisv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3guydimtb.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzkbtkph.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3jwpmipbd.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3fqaltjas.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mnlzihff.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3nyqzjnhc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ybpzsymk.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3meqsgana.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3bhiezova.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ueqxrjfg.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vaencyjq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3obfxfdhe.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ykzrnsyz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qegamyrn.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hroyrggt.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3uulgqqce.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3aawzerxe.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wiirigdz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3wbzunffy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ckghuvpy.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3yrxczkbg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ksiqopwd.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3phxhybsz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kebqrinh.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3hgszwkps.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3fbrmfpok.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3hxvsqqur.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3waobvdbe.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3dtfurres.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3xznlrnri.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3bvkjwxdb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rpuggyqu.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3bbwoxpdk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3uuifsfaf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3biqifxmq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3owxwgvfs.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3syateeoa.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3qdvbbtjm.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3nbxhjhnt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3rtwaksys.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3navtoqno.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3zmafrojs.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3erqwfnpv.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3dgxvrgjc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3dreceuan.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3zzxwsurv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zwtwzyjs.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3uneqspoh.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mddtoyoo.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ahwtehbe.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ofckcivv.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3txqxhyqf.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3uhltmlnx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3yhjztgwg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3oeetkryw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3fnoifper.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3azxwmvvb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3olqrntro.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3jhohthwe.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3kgzcnwws.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3nrglgwgc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3qpwdjpds.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3evybnnae.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3pnkzjyey.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3lofqbgmm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3azzwnoyz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3smmsiazg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3wmftmngy.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ntuasmtt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3cedqgplz.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3fsjhyluq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3auvszzqq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ciabcakp.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3wwkxsvtw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3qowuhvsp.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3dhvqzzdg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3epzizkqc.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3aunbkxwu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3dzlwwiag.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kwdydgne.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3wjlioewe.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hfkpnbpx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pprloemm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3oxxbsrwe.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hrhwbecj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lzyeozcf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wpzutjjl.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3dafnsnet.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3hdxsgpkl.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3pzlixjkk.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3tiiozxlg.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3zgfdosuk.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3cxvumcal.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqoxhief.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3vxcdptvl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dczntalr.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3dttadasz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3oymaluqg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3aovhsugo.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3oshuhhli.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3wiwyqrqp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3lpdmxdeh.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3rensevdo.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3dhpdvpqe.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3xcpuppac.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3fthubcwv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ojkbrynn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3jwpwhmzm.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3vhvjfyiq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3uvuznvai.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3sqpmeilb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qkerfbmc.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jaevovik.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3xqqinjgm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3oytxjqli.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ysmvygbw.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ldyhncfv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3mtrrtfvq.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3qgzajxnj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kzxwnnrx.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3zsxjxckj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3rnvhnslz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jnbxrvpg.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3fizdsqre.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3nzrrdsjm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3whfiosrj.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3mgfzowzk.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dfvgbrbl.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3nyprbfvi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3kvhmdbvh.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wbqziqwe.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3oovzzfnj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3pvgzpqjw.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3dvvenfvr.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rdqywdoq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3oaervipz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3svqjmxnt.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3kvyldxjf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3xvxvrhic.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3fcnldrfq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3tlmcwqkk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3imsdhfua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3doyequml.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3qgefsbtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vbevikjm.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3lkpbxkho.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3kyydzsmn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3pyudvxcr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3vcdehdoy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wtezdpqf.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cwhjwzuu.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xilfgyip.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3hnvkqqxw.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3hqfamdqp.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3fakjeqpa.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3vcrkzrnn.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3mwcyywgd.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3mmztinlc.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ncufvbre.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3ifueoizt.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3soejqjkc.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3rkmjeahu.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3xyelzjga.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bunzbxvv.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3svqkvbib.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3zfpeddyk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3orvjayvq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mrsylqht.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kslaizke.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3funlwkfs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3csfiwdsy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3fddnqpcy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3dldcmkzb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3hmiqkrri.html


<!-- 参考信息 -->