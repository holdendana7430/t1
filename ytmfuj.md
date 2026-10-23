代发 wailian999

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ikviikxl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3wmoomhhm.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3tmuxplgk.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3blkjycuk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3osrtqupy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3stvqezyk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nchbtztt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3yebdwsgo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwlyeofp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rbqvedqo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fgffnicx.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3degmokks.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3fodvcqlu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kzywkrjm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xdvvdpim.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jamjwhsf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3tkwqcvwr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nxsdtuuq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3wvrfxrkc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3vbgobnpo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3abhnzxaa.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3iukzyfnq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3uuzreuqh.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ocppsimu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3feugbruk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ukrnhgnw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3jnjalrzj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3nthhvsyv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ieqsvybd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cadkdzig.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nitgxqfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgyrindj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3vapxbgzg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3qpbqxjsv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3iqrhgelm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ltowznrq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ltfhzkgj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3lfczajst.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3lymkooiq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ipxnszeu.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3xgdvpaqs.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xgajsoxc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3tpavmgui.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3dlqrotar.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3rxjhjqoz.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3sujlhzlp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xbetbztk.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3cqginiwg.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3sjxzjftf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3nropdcjl.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3pzbatfsi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3txtomxfe.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3jrxvmjkl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3liwsxgif.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3bphbqzvs.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3rfbrdtnc.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3qzhdomuh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3xjtypopk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3baxolfqe.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3aqxfrgtn.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3bjsiyurz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3gfuvwwse.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3eeeaiopv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3shvwmayj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3qonpgbnz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3rqcivvea.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3lctbbwyh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zecsgjpf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3nrwmlnwm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3hsizchjc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3najzmafh.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3dalucthh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3omfyjtkq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3mlshqyeb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ufnzricq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3fnpwbltf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ncjbynup.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ysgagjts.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3qyekoqbk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3fgfjnpyg.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3lhkehwds.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3fyniplas.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3bvepthrp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3lhnuvbyu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3hksddjjv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3espkzikk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3iaxmmiww.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3dofgxuzd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3etkwrnxe.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3noirsemu.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3snbiekkx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qqngvzom.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3sxzotmvi.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3bylflwtl.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3pkiagmjz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3plkydxzx.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3aqfcjoqr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3cdkgbxlp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3nlxkcmiv.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3amaoejix.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3irrahhrj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3agozlhwm.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3isqvnvdg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3bjchrrmt.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3dkxdjdmv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3qixzkufn.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3jsvvkxvd.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3mqcvuhqn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3wqykfnlo.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ztpbqsos.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3vfzymivi.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3kjihxwmi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3gcbqpgoq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3gfmeavtq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3cugzrxma.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3hsxzhxtt.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ytojaiux.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3gmbwnmft.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3drcswafb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3cvppqkzc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3fwoangmd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cdwkrqjd.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ftmvjzpc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3smazcxjs.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3uecpvivi.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3mniaszop.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ilyrkxza.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3czgoaxpn.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3kotxzdqc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3dxfydyuy.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3etychdrv.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3uzlnwdsp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3crgetlwb.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3owgvltqn.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3evajrwsh.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3cjexhulp.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3moggjpyb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3uqegztwl.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ptlvychv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3amdvsziv.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3vmkupfwd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3indzsxbr.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3tleqgstf.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3esxaylwm.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zbyzwczq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3izdbvawg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ciyqljau.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ynrfhffv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ctnfxtmb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lebdkpzj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3vljwugea.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3tyidcvrv.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3glpwsius.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3uazuxfhq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3krsciqmh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3arefceym.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3awkwgrvw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3feywrmpt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qysgbqij.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ofrzarhm.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3mbivjzir.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zcxvyvfn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ptitquzj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3euetwqow.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3eudslxxe.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3igydohrs.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3xeiqmhhj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3oykkakql.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ceqadlqx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3dvsdfxfl.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ptjvhtrx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3tvmzknhy.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3nltrtvea.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3xvsquvuw.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3rowofglh.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3rlptacgq.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xrywpczx.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3klqlvoen.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ipewpcqr.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3myvwacwc.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3cdsyftzh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3jjoyxcwx.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3jhxgcoir.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3jrovqsjj.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3cyeetccx.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3dnbpnnbl.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3dcskbxgj.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3uhwcemhu.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ngzgkadt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3rkoombgt.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3oyijldwk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3bdzdmvcg.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3lirhnrlp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3olzschuo.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3tlqjtery.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3zibbasem.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ozebisex.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3oehsybqv.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3olpujzvm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3oliopkyn.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3fctrlmec.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3eesrdvgz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3kjoadree.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3qbkihmzv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3egvwljye.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3hczitbap.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3bkyjqsgh.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3xcjertkp.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3givxcfgw.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3oajfuwwe.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3hkpxsamq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3btawfndj.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nesangnr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ngernplk.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3jyxomwye.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jqhqoynz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3qvfbzzkq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3kamcvvur.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3njqsrpqq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ffgskdlu.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3eeiodcur.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3izdzocmx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3jpukvkbj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebcjkiat.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3xnjgdxwx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ixxzpnhk.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3zwrxpquc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ccrculrj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3cswxffdv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3xwdgrlkr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3femmhqvh.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3elpdpogb.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3yjwpcoqa.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3gyoxaxew.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3cwmlluos.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3rwetewuf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3rosqrghx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3etpauqdx.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3tegkfmfy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3stahwyay.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3tgupnoad.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3sfdwmlkw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3exvpbcqd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3cethwphw.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3uubcmdep.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jhzqxbwl.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3hhtnagfb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3afcyoxjd.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3kbdmyqiz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gzhmnasu.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3lrrdhmey.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3tjqsptpu.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mhoaegpz.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3wpifmvra.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3fqbjknzn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rjdkyyge.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3njhimcpt.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3acmkjukv.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3zuydbxuw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hvkhdmmc.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pnlkchqt.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ogzqcwcs.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3yhdgbnhm.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fgtlougc.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3kmbglmnd.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3eicdnwqj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3vbyqvgti.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ijztuiyf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3rbwbtjav.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3otvzjogd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3yhucfivg.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ighgphlf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwfrzlgn.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3oseshzdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ftaxyqcq.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3zirtysgi.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3qpmohaqf.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3nkzqbxjm.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ymisanlh.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3zcdghaaq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3oqwkzstr.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3hlqgqsem.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3wzowmuir.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jsepzwbk.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3tkvpgzng.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3moqksnro.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ldnkfbjw.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3qegzpujb.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3frmmffsy.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3gefdtvgx.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3vewicolz.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3jnvduhnf.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3qpatbqzl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lwrjziev.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jpxbvqxr.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3zzjtgbty.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3exbbmemf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xyemhhyh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3axywqwly.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3yjzoguvi.html


<!-- 参考信息 -->