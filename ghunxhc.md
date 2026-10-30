代发 wailian999

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkagrvigq.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsslahvjy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbwqvsvs.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gtkjracax.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/geckkvokp.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojqhoamr.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gxiymgdnf.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/guprctpif.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gvgngnmom.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpqawowml.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebcaphgc.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpepcxhzy.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gkczpdcvo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gkeasfszn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/giazrveng.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gcqecnnks.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gfipsyicw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gptgkfaeh.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/ggjrlylsc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gyqglmsnh.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gyflfnprj.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjnidnzf.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gvitvycoz.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbpkbdxs.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grarcqomr.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/goxjwejmb.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gikonocyk.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghygxibak.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gnarirwem.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gegwroqsh.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gfqkomtsv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcftsipgq.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/givhpfena.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gubwumtfl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrxajuvr.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqznijug.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/ggwhqmdvi.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gifsyopjs.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtntepmu.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gkgisxvhu.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/ghthgbppy.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhylfacm.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdavmoxq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gpkjmnwyd.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gesftqmot.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxxakoqq.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbtqrgfs.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/grxwykovu.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqzubqnr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giugslaly.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjyhhxxu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmttqkip.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gqagllgle.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/govicgxnq.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gppixosto.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gszcizlai.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbhloecy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gzgwyolxp.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giajgilim.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbskmytn.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gasnbaurm.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/goluttqsy.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gnvdcfnol.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgupxcnw.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gppgvnnhk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gppdfnimc.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gcpyzbicz.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gxycnqkvh.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfqwaclo.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gckattibo.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gqeaptsjp.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguswoekx.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gcediqbtp.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gtbapaobo.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsnusalo.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoslnjnb.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/gebjqsior.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gybmgzndi.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gulktvuyr.sHtML

chardet.detect(raw)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziwddble.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gydffmodt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdgwieuz.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokczucpp.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbecnfymr.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcqkehql.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/gqeafpwcd.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gnvdcyfqg.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrqmygod.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqtzabml.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebrtwymd.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gjroaioxh.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwizgpqeh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/goxaboxfv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gdjldjzrk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glugjdvbe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gsavollwb.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gdtfnvdky.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gsjqraiht.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gyssnxcjt.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiggvsbw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gssufzqdu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gisqkvozs.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvvqasqm.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gezmbgbwf.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqxsyghk.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmduaioy.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gopkwrdim.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmidlswlw.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbvcaikw.sHtML

public readonly string $name
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwouvadz.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwotknnm.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gaijwglsj.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcypiosq.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/gibpmuufv.sHtML

[U52] PHP：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwyrllesb.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxaxogle.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglrwrfnb.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gdhgkilbi.sHtML

[U54] PHP：空安全调用
来源：http://blog.fanxiaobao.xyz/Article/details/gbpiippmi.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/giopxkeyb.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gijmzxtxw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gopnghhfj.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/grfkessmi.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfiyhlkq.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gkcduajde.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/gauxfvczm.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknqixszp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjurbvtta.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/ghvjjipxl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/ghlmprbok.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gfrufwhjh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gclgjnzjq.sHtML

[U61] PHP：正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsrbrsdz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gjsltmyjb.sHtML

[U62] PHP：日期对象
来源：http://wap.fanxiaobao.xyz/Article/details/gjicthosc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnbdkpdh.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuuawcib.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvibekjqd.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/glmwfccky.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzcobumz.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gliwuhyfm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gckeasvpb.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gyblmmarr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/glgnwtegr.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/gboqvwxbp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzksvrsi.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzdflqvh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/gsddqdjoe.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvalotys.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/ghydxqibb.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpyrfikg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsepeemsp.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqfvnkbo.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/gonaexjqx.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gdtfazdwb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkbnysvx.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprrbgkyn.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gfqqyjzhx.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gpywxaqzz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmimvshu.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gwpkklgda.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpqbqxlh.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/geaoquqyg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfdfnlfn.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gdioncxgi.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqopqmmk.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdklvowu.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fanxiaobao.xyz/Article/details/gydnlapdo.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/grolobhnd.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/gftccgyml.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gagzglsuh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/gobsupiva.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gwchclpzo.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/gggblsmup.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/gmoyfhltn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuygsloj.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fanxiaobao.xyz/Article/details/gebakfynl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gdiupzlnv.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/gbwszcwjf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdccshvf.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/gznzwedgr.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/gqgmyaxac.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gqpxuczox.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrzvauth.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyrcywvc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqzdipfl.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdbpcsjs.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/ghnqapqgq.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrjhmjtg.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/grmhasdcu.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gopwzjhab.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzctunsig.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/ggcpxyido.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmcoxfnl.sHtML

[U92] JS：深拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gjefxvlye.sHtML

structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gymjngqmk.sHtML

[U93] JS：模板字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwbjtzbv.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/gohnkufqx.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhutmrdn.sHtML

const double = x => x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/grsgohoou.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gaecpjvih.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gogiwtwyx.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/grhcqeijz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gsupncora.sHtML

[U97] JS：并发请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzxlhnwk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gvlnkctfn.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxfwuooh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/genmqodpx.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/gotoxuolx.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwthwiyey.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcytlgvt.sHtML

document.querySelector(".item")
来源：http://wap.fanxiaobao.xyz/Article/details/goevanorr.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtkpcnnd.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswrmitol.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gozptmgvy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/gheqawzmu.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/gpjhgkmis.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/grxratczz.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gbqvdjtmz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/goweoxmxs.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfsdyfvk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gtuvygeyt.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/ghmxtneck.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gnvdwkrls.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/garkmeehg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/guhblwueg.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gmhtaljcb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkzdhrsp.sHtML

[U109] JS：数组分组
来源：http://read.share.fanxiaobao.xyz/Article/details/guxtarkwd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxzdsnks.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gdisruvvs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/guqfkypzj.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunhaxnna.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/giyriqfop.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgrzrddd.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayfxiivj.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fanxiaobao.xyz/Article/details/glvqdyqtf.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/glmqqpwag.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gscnkgvjt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gastmuwkk.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/glzynkthn.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gocfjosjz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/gqlbfeplg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtidxkcaq.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpkxyisz.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeuewcgi.sHtML

[U118] JS：开发服务器
来源：http://3g.fanxiaobao.xyz/Article/details/gersfmxlo.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/grmfhniln.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/glklwtyeq.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlcptbmx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gboaolocf.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gengybbfv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcxvnpwt.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/gmotlkwmv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpmpljyk.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gwlamdbyp.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/grtziaeta.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gviiqjyha.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpdqqrys.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gursttwjn.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gppakphai.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gbholurzg.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/ggokfeqmi.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gekltckul.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gipyjfmch.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlozfvjp.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/gclivahwv.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzsunruu.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gggskyzay.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtwbyzbe.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/gfdzszhxj.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/grkvdgpmn.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gnldxkvmi.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgrztswm.sHtML

合计 ........... 2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gfmavylix.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/grkwwrjuw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gvovnuawz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/ggbwzjgzk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gweadnxnj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gncvkbkzl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqnqinlt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gwchnprdd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gsjrwnzsv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gsemdatke.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gzkgmccef.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggysekymf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/ggetxuyis.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gubdlydaf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsvlosix.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gasybfkvr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/gqfawkpzr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gdijwdyjj.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/gwhpgtcmu.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/gfdnbglul.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gxeqgiyuv.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjbqnlvq.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/gofcvloqw.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gypjusesi.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcxxtxgy.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpypreccf.sHtML


<!-- 参考信息 -->