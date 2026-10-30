代发 wailian999

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gepmwoqml.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gjewbapln.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gfbfxddet.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/grxoqfjem.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golwfgsqx.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gejheejrc.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gyiquykoa.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gxpqffrxi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grilqxniz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbawydtqb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcqxfxey.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/goimgschv.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynnfseml.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpucjmkd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gldsxsuxa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvfzfvig.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicnnzrkq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbafnqxto.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxluomrp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gidgvkrdl.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gqnvnwnhd.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwppgcsk.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnjdxmkw.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxcpnjpn.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexgqkeig.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/ggpyvurqy.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gmocviyzh.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/glqypyzvm.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlqjjkvz.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gzhthsmmu.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmymjyzca.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gzcjjdjjp.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiexqdgi.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gxsnkninq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gnrfaagts.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdfqkkzd.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcnbtjqy.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/ghmbuedid.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwptxzec.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzhkgirm.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gzsvsblzm.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gegdetkfz.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnulbufd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxkbujhn.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkysnoxib.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/guzdkugop.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicabknyl.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkszhelu.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gbbjwhmaq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvozdzvl.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidloeggc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gphyiujgh.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gscpfxkuy.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqotyxwee.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gucevclun.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhlzghii.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/gibygszgx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gckbklfdv.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/guebchrqj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gurqbmebz.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqxrwwrh.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjshydqpx.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnfblota.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/grsvgvpsj.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbdlgtls.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/gonwtrnqx.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtydhiwd.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/geiseoawk.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gikooskob.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdaoqzsy.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/giszykwhs.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gjrabmmmn.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gouylbfxb.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gelxqdcrs.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxiumjng.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gmjdkudro.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtmcebnk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtouwrsmb.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gympbeoty.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gpkvwgfka.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gawtxxvuf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuxindoh.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/grbjnbtrs.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gwiypkgzm.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gofiqikrb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/ghuytvlkj.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiuuvfnf.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gnlmibjhe.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqqpfekf.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gxtovywme.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gzfmlyqcw.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/ghjoxbkrf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gvienhxra.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/goapgtimd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gtmrwenak.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/grvbywvun.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/grpdyreuh.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwxjwrrw.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbvkubgs.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvtubnzl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/gigvhrabf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gisfczdhe.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqjxastn.sHtML

?string $name = null
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkqutehe.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gqxnmlrtd.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxhlmxur.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhfbmmef.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdoknarz.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/glxbacazk.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbadmtrdl.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gnfjzquxi.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gimrehvmf.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbzxatbn.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvuakhgx.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/goifqxfcn.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/glokhiqya.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gtefwyzhn.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/gzwimnwns.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavphqmom.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gxsyygnwx.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgmjusgf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gqlwvbzmi.sHtML

[U56] PHP：命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/gqnnjkbmf.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfyjniwh.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmitoqjsk.sHtML

"值: {$a}"
来源：http://3g.fanxiaobao.xyz/Article/details/gesxvdwli.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginbmvndc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaemnqqwr.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyfzkokx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gvdxrfobc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmkdhfex.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfvuiayy.sHtML

[U61] PHP：正则
来源：http://blog.fanxiaobao.xyz/Article/details/gpyrtpgbz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gwgkudbfw.sHtML

[U62] PHP：日期对象
来源：http://wap.fanxiaobao.xyz/Article/details/ggloaytbz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gywsqyxvn.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/gmhgwrciq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gppthkftp.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gbybmffzj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyfcevsi.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gczmulpab.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxgvqwyb.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gayyklewj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gwbkkhurg.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gksdkihbe.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/glpuakzwk.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gginiffkj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/ggapcwlin.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/gvsutfabw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gafeqpguu.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golnkitbw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gprhlejkb.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gqaapdyod.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmecoihv.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/gwwujtuia.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnvgoxgy.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/goguvkyzz.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/goroiwnoi.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gmrfzlhxh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gcwixpdbf.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/gglpmgirh.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdbxedxw.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gypfqazws.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fanxiaobao.xyz/Article/details/gsniviuzd.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gjbjjrrwz.sHtML

composer require twig/twig
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvsjocbz.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvsnjclh.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gleibjayb.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gtpwlieyk.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaodarhse.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gzieswrck.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvgajpub.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgjujifh.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpxtnqdl.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gfduuyvfc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fanxiaobao.xyz/Article/details/gwtrbtzee.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gueensdfn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gymeledax.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/gznuhcbbf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsagonjw.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gllkcuzog.sHtML

a?.b?.c
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfanrjeo.sHtML

[U86] JS：空值合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gpchyqlxy.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbhoddxh.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphvdpvzt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/guvcvfzao.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcoqavon.sHtML

{ ...a, ...b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzskbehdj.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/gdrhnzigj.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvrxrgmw.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoizjjie.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmuqpfvr.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gjjlhxocj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gxaaiinoa.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gwzkqjfhl.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaimzgwx.sHtML

[U93] JS：模板字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgygmjbr.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyafsibw.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gyeystczb.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gcmwlsvhk.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gjgnrtvkm.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmjqssde.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gewoqxrai.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gajqcbvlf.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gliremmuk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gxiqcjyyy.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedsatbfp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gurqxlntx.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/gntehxrhp.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gnpdoyoaa.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gsoywwasq.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/gtddkbrpv.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/gaisrslhc.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlvneewj.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gibptvmwf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlhhhnyr.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/gobugfrav.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstazwfnj.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyygfyiz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gabdohpoy.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gxgcoiepa.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbabzumhf.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gawwceyod.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/generzlgy.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwzbvaqd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvsjitbo.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkphqbke.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fanxiaobao.xyz/Article/details/gclnwloxf.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gspkymana.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqimncknl.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/gazeiwtgn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrnjyafu.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/grofvxmam.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/ghpxnpjjj.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gtrngteir.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gfwtlyntg.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/gtcfzxfub.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouujofuv.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gheorqxac.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobofruzg.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuaezvfg.sHtML

crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/giiypfubc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/glvhspxbt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gllvyxhzk.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbqtnbrk.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/gszphhgks.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmjchckc.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gedasmmzu.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/ghdhdjmvr.sHtML

npx vite build
来源：http://www.share.fanxiaobao.xyz/Article/details/gmexcorhm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzzhsgtz.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gbiwvkfxt.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gobqlqpbx.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/gtikzneoe.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkodaofr.sHtML

按语言统计（条）：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejzhemgb.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gmntharmp.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gupdobrwp.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyoppqbt.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgpvluis.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gxypapzbc.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/glwjzchtm.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceekfyhv.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftkzuvdl.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/guuxzmbvk.sHtML

C++ ............ 30
来源：http://wap.fanxiaobao.xyz/Article/details/gcyjkjoqe.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeolxopc.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigmsuwsz.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmubwhui.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gmegewawf.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxduregi.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gmmzvsmpm.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfsnopoo.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gmovpvezi.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfnezjmj.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gxqjjhnir.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvxntcpm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gksulemyv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdxdthet.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gngkfirit.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/gumdnfffm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaqndakb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gqxeasvoq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gorezeset.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gtvoimzaa.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gsfcniynh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gxqcgiors.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyawkzmi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/grqdzccnf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbsumvct.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqudrgwdk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqjanrxn.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmyzgckd.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/gkpxhmvph.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gkibroyci.sHtML

T 其他语言补充                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gakldzuqe.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshorsyll.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gfldbqptt.sHtML

合计                                  2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmoltztv.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gdpmahpim.sHtML


<!-- 参考信息 -->