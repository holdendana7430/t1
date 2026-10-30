代发 wailian999

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gsememjaa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gnjjkonlr.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gsbbbqcfa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gbnrqeuwd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gnajvfera.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gewvyvgum.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/goaqywswf.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/ghugyvpho.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gjwrejqkf.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gwflufydw.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gwtjlnrjj.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gdjpwqtoj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gcidfojkc.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gsopovzqj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gluuqwruq.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gqueldjgk.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gmfsuansx.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/guxyvokvb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/ggxcvisal.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gijsuquee.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gelaqhmgq.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gvmzewwzb.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gtwlzjfhb.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gtukwbgms.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gjpresysh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwfsnpexc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gkugsepua.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyzimgoau.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gnrkpquee.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gqsiufhoe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gfkjewowt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/ghzvkrfme.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gatbzgwqj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gvjbliydg.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/ghxostiuk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gxopwttqs.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gyxblopmx.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gisclclrr.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gbobgleoe.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gstlbnfky.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gpsizhxfg.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gdmulifut.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gsjlbpczh.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gowxtrums.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gokiiuprr.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gmsfcgixm.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gacmcyndr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/glvjegfaf.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/gkuctkdcg.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gwiqaymho.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gztzhiitz.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/grvckjqtv.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/grbxooiql.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/grxmkxxcy.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gwxgiyqcj.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gcergplyi.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gvbzflvbb.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gjupizenc.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gkgkrmwvr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/gwferkdyc.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/gawhqfeda.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gffldftja.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gisxkavwn.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/gtcbubacg.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gcrnjeogb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gndrsheph.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gmoqsohjj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gjwnfdlbk.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gwhdgcyny.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/grjlbysnr.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gjdgkgute.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/ghkybustz.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gtyzsvrde.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gipefpbix.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gkijoihsx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gbxdkuhum.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/gpttabfix.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gpehciugk.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/glbinknwi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gwjyrzaui.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gaambnmrw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gntabzyzt.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gyrdsjtun.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gyoxahhpa.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gggjrysde.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gmkrvrujv.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/glnpqxkox.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gwpijnbbp.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gjovbjhic.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gdayabyta.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gaekcfthn.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gnqkxpmqx.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gywsrhnfp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gwhnyzqec.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gwrywcxhu.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gizayisir.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/grctqkpss.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gtqoblyll.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/gwgvffenn.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gmyxpnbhs.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gewohwijl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/grobcrdcv.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/grjomaffv.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gzdwrsmhh.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gtnebmutx.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/ghsprsstn.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gflsygjxt.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gbqqahmjf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gjeeadzjz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gxeyvlvvf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/guihwakbi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gimpwtugf.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/gatxakmfn.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gobhvpllo.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/gnmdycujq.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gsmlpjwyq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/grnjxqxkz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gqelpmgcz.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gipomoewg.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/glguffpcj.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gvklcakma.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gzixzlpsn.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/giazcgieg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gcjlfuxli.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gcrapkgnr.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gslsaeont.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/giidvtwsa.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gqafrjsej.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gwlhwfegq.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gjsibhhik.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gjwsmeqep.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gnflhhncz.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gquwkzqyu.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gzzigaadh.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/ghyvzmgpx.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/ghnhxawsx.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gzozpipks.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gesqfklyb.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gdkyruszn.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gwknjmnsn.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gtkjygbuf.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/goesjrmiw.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gyuezihgj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/glcbjllwl.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gerzhknjy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gjjidcgpj.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gnmztjuvo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gwtnjxhtm.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/gmxynpdic.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gqurxvuim.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gpfhieleg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gfeiaevvy.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/gypydugrx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/ggdxwfvpp.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gosbfandp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gxfpbbrih.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gvifjwdhb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gmemjqnin.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gsepnveek.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gkigclxnq.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gznvwrhfh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gikqwcjua.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/grskybmmw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/ghjbqwxuu.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/gquqzckgh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/gymiuxnzu.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.zdbjq.cn/Article/details/gqntwdkhu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/gtsugxfdj.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/gnwznccxb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gsbhwhdao.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/ggqxypipz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gexqoumhw.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gdakworab.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gbhfbagqb.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gonfssdiq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/glzrqgkqm.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/gxnxqgtmj.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gkymsyjvr.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/gwscyeqrp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gtnwvbzvy.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/gwuwltcbv.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gzjaowjyl.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gcrqpoehq.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/glkjxjnqs.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/gisnpbgii.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gjydfigkg.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/gafzbdjxx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gfsggvyyo.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gfyzggutu.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/gdjrctdrm.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gojusxgox.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gskbbsobl.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gromzttgm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gnwvhkyie.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gzruwkclh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gyvdxnifc.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gtzlqdtey.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gthujmyyj.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gqjnnjnvf.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gobviyfpi.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gmhmvbpbw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gopkzcses.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/ghyykqxuk.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/gemvzrziw.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gtmtxjzya.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gsszcjldi.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gsfrfjptu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gnmdsdtdx.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/goyijhuun.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gnszrsaau.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gjarsdvan.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gnrgjnzim.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gsdvelkjo.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/gkawirmfa.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/glotzoqtn.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gtnkbnaok.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/gsxbmhmtd.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gknvktdzx.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gzlbflema.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/geljfjqoe.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gzfzhviyw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gvsretlnm.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gfcudozap.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/gobqnxtlf.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gprjnogde.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/grmiaklmk.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/goafdgjvx.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gnvjjgurw.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gvuxdgbxu.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/grxcrwump.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/gtaegyutr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/ggnxukeaw.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gwxurrgqf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gxqsssrap.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gjvtixmho.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gaederxlg.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/ghtrswsoo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gdmbijtvb.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gorkhlvzu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gaqbpfjzw.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gqkohuobn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gxkumcfzp.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/gxceqkzus.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gedtaijhc.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gfxkvordq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gmlwsutpy.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/gndgdxuin.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gabjtllas.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/ggfoecoig.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gsqhohlik.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/gflxzwqyh.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/ggasadece.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gitvkkvhj.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gssqfmecr.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gxuufqkdu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gejfnbhnf.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gasunpktw.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/goltqtbbp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gsrmthnxr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtqykmfse.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/guzckudga.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gketczbwr.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/ggcskkrrx.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gltjpkvzq.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gtqlrmxbm.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gbereozyw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/goxychdze.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gxlvvamso.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwyvbyzdu.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/geelpjjac.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdybpneug.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gfarccpwa.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gacoevvbs.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/gwilxfhvc.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gsxpwycsq.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gyjxboleg.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gtohhraik.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/goksulbgy.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gnjwmkhpk.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gyznmprkh.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/grwkrbkzo.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/gfgcpoyux.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gihmbdqvy.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gtogpmvto.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gjzleaorb.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gytmeccwl.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gzecqgofu.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/grjmwktmw.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/ggydkwymf.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gxndyhjlo.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gdardhwyo.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gtkmstzlw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gjxpsnsby.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gadfphicp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gxiujtwsy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gvljlcqnz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/gvpvmuzfm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/ggkzbxayk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gyvkgfwpm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gafbvszof.sHtML


<!-- 参考信息 -->