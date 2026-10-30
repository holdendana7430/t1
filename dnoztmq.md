代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gwcspseik.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gavgexdbz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gqyzvabzw.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gcimvjkfd.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gttgnvmbg.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gjekeorbg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gprqnvosy.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gmrjjauie.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gzwrseowi.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gbphmsatz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gaqnrpobn.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gwcplofca.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gajmuiibg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkovdmcnb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gigraiwco.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gscqpgvbv.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/gtzqukkpq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gxgefiwqs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gvhwezblp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gsbkkrsoa.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/gvbuzaopk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gznhkmxyp.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gztjzpnch.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gkyvdwlhf.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/ggafnxxsn.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gfdrdboek.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gpxrbiwvb.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/guvpbtfqc.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gxfpxoabj.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gdwtcuxmx.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gbuexwcec.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gjssiwsej.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gvtwegrsd.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gazeiwnix.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gopavxgnf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gffdxdviv.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gfdwhplqs.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gmqaqoecd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gjumpzoiw.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gvzqaslvk.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gamjtreow.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gxdibsjhm.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gmnfhbvlx.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gvbinziyy.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gzrjedsyz.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/ghkwrdadr.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gipaziami.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gepwkqhjt.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gimknfmtf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gxtqaeybc.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gtcohponr.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gcbbxnmbk.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gjuvbfiqf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gqcjodxut.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gxpwwlbef.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gbfbkcupw.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gdsfergvi.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gmahdcunz.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gcwxpllzt.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/guxzcicsy.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gafmvsyoz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gwjwannmn.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gmybfpusu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gmrenknol.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gkrwupyvp.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gmzwvtmhw.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/ghtvsahyo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/goxhxssnp.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gxxbvhrhe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gbmyjgmfo.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gjcxvtrfb.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gdufvktmm.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/glqpwcxpp.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/grclwjons.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gqmmhxidd.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/guqsihivl.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gellonuea.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gkexwrptm.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gyfqrifdd.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gznbqmmtk.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gnhsgqvsh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gjfkotmoa.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gvmegqhfn.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gozmzthim.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gsptrjtxx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gduisdvlv.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gzsyezzdu.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gissfljby.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gkvrwzroh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gssbeupxq.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gtyvdekwy.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/glkotrhrv.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/griomsgtu.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gzcplcago.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gsaeepewg.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvvbmhior.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gqpzjvgjh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/glcldonpc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gyfnohewv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gvqjwspnp.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gcgocqtzi.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gqdewzbwz.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/gpftbdqtp.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gvmwpglqr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/guorpgilu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gjatghwct.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gvhgdxhdr.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gadvolkml.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gsdfkfcaz.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/ghkrfypdz.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gfbcwdsgi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/goaxvyybm.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gjlqejwnu.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gljzwtytu.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gaisjitjb.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gyqebpfow.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gbmmznbsa.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/ghyqczggt.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gzpranbcn.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/ggmahghzl.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gshuyyubc.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gbszzubfp.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gxabqxwlk.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gesuuqtlz.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/glysxewqa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gzuubtwal.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gpswrhktk.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gkiedoonr.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gyzkgdkus.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gwsuboklr.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/giqlctvol.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/grddojvby.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gkywncalu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gzadzgszf.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gnamedhuw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/ghyyxnxta.sHtML

[U61] PHP：正则
来源：http://mobile.hesvh.cn/Article/details/gtnlffnnf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/geifxwktr.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/gcfohbekk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/giqutcdec.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gsfqzrboa.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gmbkznujg.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gcsfytrcg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gbanmmueb.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/ggcceqgit.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gcmpgacut.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gyahuuoug.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gxycxjkwc.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gghzffdgm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gawtcuhez.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gsoqdzwaw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gjkyupbue.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/giywokktx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gsawjlvum.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gevriqedl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gxaytavfm.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/guhptcnum.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gqveqoiqd.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gbegukxyh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/ghfzfzmnb.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gllzdfbkl.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gemghtknp.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/gkfskmalc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gqzwsoiag.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/gnxeqyjuu.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gezfuezdt.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/ggnitctsf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gskkeewpw.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gfodosuxk.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/gydjiyqjc.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gtfvfhchx.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gonrpztyz.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/glpggtvka.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/geetftjba.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gppznmgdn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gchbjsbol.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gupdezpfx.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gemnnxvnp.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/gyfpycpuj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gjswcnmke.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gqxelifcy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gewmjaffc.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/ghphhcegr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gfsbwluff.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gxigmyxxm.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/ggmlrdbcs.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gqvgjylwv.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/gfcsdtrcw.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gnwbxeuhd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gqjctlpgj.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/ghixgpvch.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gfigqjyyn.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gltwrudku.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gnilpxyhr.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gggmmsqhd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gdlrqjhbt.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gkgmsmkuw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gbborrugk.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/grxfhystt.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gnihqrzrh.sHtML

[U93] JS：模板字符串
来源：http://www.share.fehbvm.com/Article/details/gbbkwxwyp.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gscckizgl.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gapqpwzdd.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gkhmfgeja.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gnylfltdk.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gdcklcfnq.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gsfpoyath.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gxpiibivk.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gsjvxtllb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gchndginm.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/guyptfizu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/gdmvmxtci.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/ghdxuqjwi.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gilmqelxj.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/gzjrtksso.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/gcjhlzrpa.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gwazpptym.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gvrgfcnsr.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gfeigplgd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gmlbmuqki.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gnjtqpdja.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/glcxskywt.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/giqhwqdwr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/ggzgzjvpd.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gwlevtjwg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/glrovfzeb.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/ghjjvetlt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/ghrsptecj.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/ggxqlxvyo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gwmkyzioy.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/grakhpdas.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gsvebyors.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/garkyelfx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gotzkbssc.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gyxnpmdqt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gppbugcuc.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/gimwemmzo.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gusrbsfca.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/glbawpzaa.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gbxopmvvu.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/grzkjihjy.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/glnkksqmu.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gghnywuvb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gvplnhega.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gossxbejp.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gqkvirgds.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gpwyskxfw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gvfubmlss.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/geycbzjff.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gugvqdlye.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gzdbfoxpu.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/givsgsgak.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gdfcyufsw.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gkputqcev.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/grxpnmtfv.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/guzpgzcnj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gecwzyxqj.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gupfgkmdy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/geyfepbum.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gjwktwbxp.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/grebomgua.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gkbrrzjiy.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gtjvoxdjt.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gzthkbcel.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/gpxzyubsb.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/giumgzqwj.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/giaukyqhb.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gfqzbbaae.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gilpmubyt.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gngdhevrn.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gmewvnnge.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gqviqvfvz.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/gzkaaegfy.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gyffdjxem.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gqkbtcyla.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gviyecjyo.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gerirsaic.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gqsihjhji.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gkzjkvvuk.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gewgtqtva.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gyrgfpddi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/glvrxblii.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gcbsgwjgv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/ghepgfjzt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/glgzqgixd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gdooynnmq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gnkgrmjyq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gtcdnmrnk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gerxsxisx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/guohfesdr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gdtepvdty.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gjylutesf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gwkfghkuo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gjzpfiwst.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gomqrxviz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gulxjomfs.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/gvtdtsovx.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/golejtxxz.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/geqcsckho.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/grasnzakr.sHtML


<!-- 参考信息 -->