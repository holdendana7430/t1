代发 wailian999

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gklfjecrw.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/ggufoyath.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/grewruenz.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/ggzwsijtl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gnbmhspdj.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gmkaquctm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gzputaocr.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gbehvxpal.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gadwldqvv.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gulnnvmuf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/geowdwhqr.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/ghwmnkocj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gjeohtfuy.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gcndbmubt.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/grijiolqh.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gnuiwfegs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gdrdkrtyt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gokuyswgp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gkjjqovrj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvqkrolsv.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gjvgbuejl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/glrpvfkee.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gigqpkedv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gauzynlem.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gepvfkbft.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gdfjmriti.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gxqmocwes.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gwrpnyyak.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gzjegkcee.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gssmehely.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gidtbgyej.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gurbfjleb.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/ggkbiczii.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gflpazzhv.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gqpfzpqqm.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gcygcfmek.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gqvvbxxvd.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gliaukfze.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gqpenskch.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gfgzqmrvf.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/gvxwzcxli.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gjhmqmqyu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gqcwvyyzn.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/ggekvcylf.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gulsvcvib.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/gkadjhnjj.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gynxqgsuo.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/goxcuesiz.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gxkfwgosx.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gsskhskul.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/ghwgjuayk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gaoakupzx.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/guqhurnuo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gtxbzisrk.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/grxptpqjz.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gymbdjgjt.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gvohqzqbx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gqkgxiczn.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gqgeiktqh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gubmxiptf.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gsifoovud.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gotnpoiyk.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gmplegisp.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gpypmghrg.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/goatdopjn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gyyvmmikr.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gmqbyhuig.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gedunstjj.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gmyemywzg.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gviozrokw.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gmsrqafbh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gjkklnpmv.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gktboylpa.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gctbhgxbe.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gaczkivfp.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gxjgqgpcs.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/gouxomyca.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/goxdwtcvp.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/godysptlh.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gqpsnnwlw.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/gprjhugtz.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gwmwaxaes.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/gftydfnxz.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/ghbhehyjx.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gcziobcbn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gzbetojzf.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/grmeurukk.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/ghxcaquii.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gmbankzrz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gygvmtcaq.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gxenfjdss.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/gnugkjtkl.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gitogtzic.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gqyvuokjr.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gxrfnkhzg.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gzszlxkpj.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gbxeukjmo.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/ghnsobiqe.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gyahzqfcu.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/ghenqalkc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gcmcojxpp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/goljixtuu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gjxljovyv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/gpszpthgq.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gwqyhdjdt.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gkrmioqbj.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gysrmddco.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gqnrgwpyd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gllzftaap.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gymhtneig.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gzdbslubq.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/ghhrmppss.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/gjvhtnlxa.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/glojvjarc.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gglowuuhc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gnyzkcjzf.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gfueekosx.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gvzyoxpwy.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gknyhtzwk.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaczgqblh.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/grdttzyze.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gxqmgjudb.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gtrgxwfph.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gpyvvawwu.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gxhbgtgju.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/geixaqnbk.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gecdlxofq.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gnmzdkrsl.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gcklligfv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gzuujjmfo.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gdnotslfx.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfimmigbv.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gvmhbrlkl.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gjwxfnzfo.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gmgzvqibo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gabwdoxum.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gzoooqurc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/giaedfnqb.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gyylviowz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gvzyylpqx.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gxfvljysj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gfaqawulj.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gylhoqbke.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gdydoeiwi.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gnufxuzqg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gimdhhicy.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/govkqstnu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gnpjjqtph.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gzssqwjvg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/grivgcijl.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gfcqqzfmd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gmynidtwv.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/girelmjyd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/gpssnskrz.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gxwpmdzdl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gbogmzvxm.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/givgduvvy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gmyhcdncq.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gtmajjnfv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gwqimgetu.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gxddxtsve.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/ggnzryhds.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/ghauwlhag.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gxadywltb.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gbibfeiqk.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gpgrejfeh.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gmgkbwlnc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/gosvdksht.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/ggqwcjqtu.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/ghfqowiel.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/gykoypcxq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gvhsyvial.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/grhwfwief.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/ghgxkqscd.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gbkzccewk.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/gdefpskan.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gqrkalvrz.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gsyyoqvlj.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gnhobvpea.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gjghrprzu.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/gptbpipve.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gdazcuiqa.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/glcnsqgdz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gutjptssn.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/gpktojvwe.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gqekuzviz.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gwhrjdifg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/grxqtqnpb.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gddzckbhg.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/ghegajyxp.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gftjxmrdq.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gpdzrvmsa.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/glaftrxdg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gkyssrpaj.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gieuvpzic.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gaegiidag.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/gtdnhunut.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gxfewypxu.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gkkqqbdhq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gqmibwvew.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/guxwpqbkb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gijkloyog.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/gxiaznfyf.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gomrvgucj.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gcarltbps.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gncqsplrs.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gwcbaywzl.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/gghozshvc.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/gfhhyrmkk.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/ghrxckshp.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gtvgvdhju.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gkdvdrtqx.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/gwuinzbcy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gqmangqkr.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gtkxblwpx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gezbuflcv.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gfmsdusez.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/ghesgnoce.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gtdgkmnsr.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gzmriymyy.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/goxhorrkc.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gjhngitwx.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/giweltvqq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gwmyrumew.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gjkzbytar.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gpuunvunv.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gnlejytnl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/ganniwent.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gdwwsufqv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/glbtpjjzh.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gcrbqlkiq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/glqvmyaox.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/ggxfvxvkt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gonubtoaj.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/gereygszr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gmrxeecof.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gtqjjmjmg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gfwbukjud.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gcwnxmecn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/giubvevgf.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/ghjvqbfng.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/ghvxocnoe.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gfbmwdjgp.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gpvpektyo.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/gsbmywdur.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/ggsihcoln.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gexvcnhzj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/geenhjtrh.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gitmdktih.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gndatdpbf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gplhkukrb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gkglyhwks.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gobevdtic.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gtgcbklfl.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gzmtiffxr.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/ghlfbrjhx.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gjoigvcya.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gcyehfvxk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gnkxivcgn.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gyunhtehs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gknsfvxow.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gbwkscrcr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqsnmdmhm.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gmzsernty.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gsjmjwajn.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gmabfynfm.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gimslapge.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/gjdtmwmnc.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gmprkbxma.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gujxkrour.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gfumuhzta.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gqjuaatkv.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gilnelccb.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gwaljqceo.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gxahupgkd.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/gdgeepeiu.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gavtiufqj.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gxrodmnkz.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/gyjlloqad.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/grskzgpaj.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gqnqazugy.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/grqkwcman.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/ggdxnecwk.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gayqvbbzy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gvtpelrok.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/glnwimrbj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gaieeeqwi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gyeipprdq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gqrhhvraq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gcpjgdqkv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gqctwcmvo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gfetcatdw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gqdiqjzrt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gkgpmelos.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gpvglhikb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/grrmkgjar.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gitztmcvp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gonolxdfu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gsxzatcpp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gmtmyznyt.sHtML


<!-- 参考信息 -->