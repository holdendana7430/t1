代发 wailian999

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gybfmcnaa.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gogydwhiz.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gnppuyjtx.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gzqhhykpc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/ggbgmvbst.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/ggsuakxgf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gssvicrbh.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/ggixxwacr.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gipalgqlj.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gytzhpkjt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gaptdrbbf.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gatkiivcd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gidovgock.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gbijpsjpn.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gyuuowfab.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gcxlxuhta.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/ghpmggftk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdfohridx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gzjrlznwc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghvojlltg.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gyzyjdmmu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/guwdugamq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gjkwtqjjo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/ghsshktev.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gsimwicox.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gtbdfmfqh.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/ghvcwhnzo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gmaodqapc.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gvxovnsdg.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gikcnnmuz.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/grxyvestq.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gyeepfuvm.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gfuexczpa.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/gwcecvuoz.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gnankuvda.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/ghojjpmfg.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gfqxiyguc.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gcocrtgcy.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gvwjiycjb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gyzfyxrso.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gavujmbsm.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gemzkjzbq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gbkahlewx.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/grqafmtgq.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gfpagfbeo.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gwhtbnpxf.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gkrltwfdl.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gswqmpmyo.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gjzioituh.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/grcyxjtus.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gtektivfq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/giumyuega.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gkircsjta.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gxwppmcek.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/ggvsfoxoh.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gpibastkh.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/ggpbdcjbt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gdhfpddjn.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gwyaalmjf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gpavoqvud.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/genzygfoz.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gpwzxfpzs.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gzhofccbu.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gfrgnifta.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gfxcmjkhf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gnlzfkirp.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gotvfrwul.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gkrnoqxzh.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gfzuxxzpp.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gakwkzesx.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gprflnavl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/ghsjtxhqh.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gizfaufhn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gkhvbqreh.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gzykqkamt.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/gljmovqfu.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gcbhjjeuk.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gqyujiuyw.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gidhpqbxa.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gqivbsiok.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/ganbovhhy.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gtlemfwsk.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gmovnenzr.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/gzfidfnne.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gteaaglzo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gtedvifmv.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/glinloyjn.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gtqtqvsqm.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gtcvdfcol.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gtzrqdfvy.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/glpjaftcg.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gueiositg.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gnuhsbyny.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gakawzhbm.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/gqiqhlhha.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gamegkrhx.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gyirggfoh.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/gpliiordi.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gzculjkhn.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/giishfvzt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/gtdtnwauv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gjoinbwgl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gnftngatf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gmzyugwkv.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gsdnlcpve.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gbmstqryb.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gdkmexxzs.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/guprycrgh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/geczmmojf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gemsjixlt.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gasbwlwpn.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/gfatxelib.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gfhjarian.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gsytpymjj.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/grdodrzmn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gmprfyxxk.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gllglivsu.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gddfmszrg.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/gvwdtevdw.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gfmboxnmq.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gdwbonmdd.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/glbyrxkwj.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gothfqzma.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gdldqjofy.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gdijjzbcu.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/ghwdybuup.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/geouqiqsb.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/ghrmtmbgc.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gzbjqgeje.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gpqfjsnty.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gwmwkmmia.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gbacqwdqj.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gomjxbdwh.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gamsmkakf.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gjpgfdwuj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gkntuspae.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/gjdakibfk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/ghqsycxft.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gvcegcsqd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/ggrfaytgl.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gcyhlhvpc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gfbexetgb.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gsupkpygy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gzmsvmopr.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/gxlfcsgth.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gggdonfek.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gxmspnskd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/ggpnghryi.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gswgalnwj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/grdslvgwc.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gmesccvzm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gbbmvgnzf.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/gimtuhmow.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gaoinuyzc.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gsqhqckco.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/goeowwjcn.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gcdwpxilm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gnygwchhl.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gtqmncrjz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/grhkdvwxs.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/geuzdipau.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/goeumaavo.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gcynebpix.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/goheiabbv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gmcfoxqwq.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gersnxwdl.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gtgftapzk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/gqqywlnuo.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gxmhekxyt.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gfmsfqtha.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gzcbmdnmd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gojucdbaj.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gdczmfpoi.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/goiarqvkt.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gspxxhygu.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/gszalibyg.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gdyjwcbpm.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gyejrjwoj.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/gnxagsdvh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gkkeilcou.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/gfmurfaoq.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gngytcvpf.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gpryjdvom.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/ghtnrdapt.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gnedkbxsf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gbsdfoamb.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/grpfikopj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/guqtwxnnx.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/gycltmloz.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/ghpamodru.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gykdhztmt.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gnmmxzfky.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gcubaearv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/gnwagmcue.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gojuqoqmb.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gqbyyynxh.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gewgndogh.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gqwsmyhcc.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gjccilqqt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gvotieiis.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gegfhqxjh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.zdbjq.cn/Article/details/gwpkyolpk.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/glppoekzx.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/goxjmucno.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gexfjjidz.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gleyulifm.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/grmanlkuk.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gvvtjkjho.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gfrlylczx.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gtjzhzyrq.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/gpnzqiymp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gulxjsrvu.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gykkkdgof.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gpsqbsmwb.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gglbeyuls.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/gcstlnmul.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/ghutydxdu.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gqryzgozz.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gvroykfvy.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gxaiwojpk.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gpznkhxir.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/ggaytgtxw.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gmupbasso.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gryakdyvv.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gczzwgcjq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gwkbxfmfx.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/ghgrbkvyt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/glidutunp.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gfkceetwx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/guiribnht.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gbkogusbk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gcmsuaywf.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gadrmhxss.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/grbmmdowk.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gglrtnnnh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/glljkzdjl.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/goyjkstbt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gdwqhxkqm.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/gdktncagk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gngkgwlwc.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gstfydoqv.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gyfvmbqyb.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gwniocgay.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/glibjrdoy.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gfjdbmybl.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gtxweyhlx.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gbkwqvlpc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gaosftvjn.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gnbqlftzg.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gxlogsfbx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/gqtqwrxgu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gbkadmzwq.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gdnddygsl.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gdvhxbpfh.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/gspzyzwve.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gkcdffvud.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gpljoeaul.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gjkiwjfax.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/gpcqgftqw.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/guhzxmupx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtesdkmxi.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/geijnivob.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gibirgtvu.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gsprggiwb.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gleeoswoq.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gmvyahgmh.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/gjhjztitw.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/gqcmeflqu.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gzhknfvdf.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gbirhqjmy.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gymtcnqwk.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gnscszjcq.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gmgnvzfnn.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/ghezhykuv.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/grbniaicm.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gyxzvljxg.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gzjkfgytc.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gppczxtzz.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gvwgcxhou.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gbprdjtyf.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/galcasmpm.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gicvvczfz.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gmiaoosnr.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gvuuvwete.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gasiawwuc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/girswfopw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gwxbvsyxa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/garenqasf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.zdbjq.cn/Article/details/gvwfayzmt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/graemdhqg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gknsirhit.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/graeqfkwa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gviosohjj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gjdwoovgc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/ghcxczenz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gjuflwzcc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gdmiymkwu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gwqjynjxo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gquwgsial.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gojytuxdq.sHtML


<!-- 参考信息 -->