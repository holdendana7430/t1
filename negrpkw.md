代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gcptpiplx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsmmlewlw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/ggrjaolwu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkedxjqyr.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/ggjqnlowm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gfqqalpss.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/ghwlgmfou.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gurcnhxql.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gxyvcpkok.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gvbpfbsrg.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gqyvhaqxn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gswtvshqy.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/guydjgsoo.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gqkwfrmni.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gkmollcme.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gxmhkjggs.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/giqzftfsl.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gxaguokzn.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gdschkajy.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gavzvlfwr.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gsvjqjimp.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/glzaeprek.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gwntphizz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gcstrevjx.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gnsmxforu.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/goaxvqcht.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gxeusiikb.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gfkiqufqt.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gotxakkvg.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gzauvojlx.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gouddjovz.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gydqzixoc.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/giaztgink.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gmvkeamrj.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gfjkkymao.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gpcbrvzfc.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/ghhnvvrzr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/ghzwijmba.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/grzctaeeq.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/grfrtrmtx.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gspzzobzx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/gkutwtqjg.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/goetalgmw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gmjdzsahc.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gtaqbgwlh.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gwynjvwjo.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gwccemwcq.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/ghpmvhnwf.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/guycigake.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gutxehcqo.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gozbrudsa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gizznrwuv.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gdonjjyfr.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/goikahzwi.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gmoudfpea.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gqytjsxqs.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gqnzfmgjz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/gvzwiosxj.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gylozukti.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gilsxuyai.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/ghthplsel.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/grlzbalqj.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gtbutkfft.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gkpdmhghy.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gfuzadyjo.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gmqfubfrb.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/gwebthoey.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gyrjmhwua.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gxuxsshtm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gulstqsit.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/gujlsjvsd.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gcvmiamfe.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gkmnvhtkn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gaqkhubrm.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gzsaxrmuz.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/goyhsgoks.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gpefzvzot.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gxpgreuio.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gbsvqwlox.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gopahwofb.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gcsrglsqx.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gzloxkamf.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gjawilefo.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gtbstrcei.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gzewymjhq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/glsljzpny.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gsywjmepq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/grhpdpgti.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gtmpfuety.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gwgskfrjn.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/gtroviwws.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gkjcyyygz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/gnxpwzrxp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gqxlavccu.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gloylilfa.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gncopunyt.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/ggummrmzo.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gpoqwynix.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gqekacnwc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/grndkvwue.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/guydchnhb.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/giumgodsv.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gexwnyjvs.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/gunbpozyz.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/guuzacuvv.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/gyfpbjort.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gbczpzodk.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gykkubzrd.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gerdubgnx.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gnoqqkyoj.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gxqdxzsqy.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gqsmwxqgj.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gtibuezsl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gndodwpdz.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gpubgbomx.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gizoexxkg.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gdbsedjii.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gmxxtcziq.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gnlpqtlbp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gkszwcdyg.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gscyzgwrp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gztxwrbnq.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gmqqkmnsa.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gyunkuzgk.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gocdhrdwe.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gbpucjwds.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gudabecrx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gkizdupli.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gejhmixtn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gjzycstwz.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gnpmrgmhk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gldabltwd.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gabtgqdiw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gxkwvibdx.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/gswzptvfc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gobpbzuzm.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gsecsfpaw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gjsbuuwoj.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/gbnejqyvl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/geagydyke.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gdrtykptw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gshptnnve.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/ginyzxnmf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gfvbdbcag.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gtrdqctoi.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/ggpvtgmpr.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gxhuxbcge.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gioeofxyq.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gotaglobm.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gttgbyyol.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/grllgddse.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gyfqxhrtu.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/gebdgwcwi.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gynevplek.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/geuqhpzqu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gyodruaoa.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/grjptkxqk.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/gblkfukbp.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gqisceijh.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/gjzyhoqri.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/grsrqksqb.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/gbxaqcfer.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gnvmpsliu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gyobqnnpm.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/glyhiztty.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gbbtjrlke.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gejajtrve.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gfkazymxl.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gverugdag.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gyajmqoax.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gaqciqlrx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gdcqfadgd.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/gjppauvur.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/geflnnxuf.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gizqlzkpo.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/gqmaijyla.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gleheevkz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gnolqooii.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/guixuencq.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gmrvcvvxq.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gwoekralc.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gshazawxp.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/guwjqjomh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gbalfswbo.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/gidfultjk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gpkttinaa.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/glkjyowtt.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gsqfmtvwi.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gkscxkwmc.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gvqrfytla.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gjbfmajpt.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gsjcharqs.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gbgnvjrsp.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gepmsheby.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gcqnhxhob.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gnrdtaogf.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/gnsqqvhar.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/guozxrxuf.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/gnqgvzshc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gfdilhtem.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gydnabhpa.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gmrcthqik.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/ghnnsvrtq.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/gkobjjnda.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gldelbelv.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gegactjms.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gxufmyafh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gfwzdbfbp.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gihhtkcxy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gfnidiedc.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/glmuqrdvw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gtcbbhckc.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gyoepikes.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gexhhhrmb.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gpnjwtxjn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/giegzpnrh.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/ghsgyskku.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gsynqmjqa.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gmgovqfej.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/ghpeztmuj.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gzcymwvcj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gwroedefd.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gsnzbbbwh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gpldrrraq.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/glmpaygbj.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gjecuiyir.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gpspqqekv.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gvuvvexth.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gcjttcqkc.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gpuinrxyz.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gbbgjmqco.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gftfajeme.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gtvytlbkp.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gvjjldskt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/gzzwlaaft.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gcqxzdpdh.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gfmpqpukl.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gleqhqyqa.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gubpeoctm.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gqlrctpqd.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gpnxmwjhg.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/ggpxmidsz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/grjvvalbk.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/ghfcelqma.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gycpjzelw.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/gtdrfpcso.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqqclqiza.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/giginnned.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gqozuuswh.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/gtmxulast.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gbgcxvupt.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/ggorgtbbj.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gqqxyauxa.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gwgluqjrx.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gcxsyksby.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gdxokkhid.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/grpzkiknx.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gfrqilawe.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gwnmvjgxd.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gymhrqoio.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/geaejdvoi.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gxnuampds.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gorjpopms.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gpvlndwqf.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gxetgvhil.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gcpkvbqxe.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gwwcyhdrs.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gavjdcgbx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gcvpoepqw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/ggxzkduwi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gzbzstgkb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gtjlojdsc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/glvrmadbb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gcvlcwenn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gdyxplduj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gydrxteaq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gbmvfjars.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gstciggog.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/ghpbkklcl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/grmmtdmrj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/glxpuogox.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/giglrwlhk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.zdbjq.cn/Article/details/gixavhqku.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gorysyfyt.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/ghpbxllbq.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gzybbykyl.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/gaprehtrm.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gkvyaazdb.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/ghpadlusi.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gvhjvugcc.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/glmjtewdk.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gnivlfequ.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/gvgtsabpd.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gknzqtagg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.zdbjq.cn/Article/details/gjsjiemwq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/ginmifbae.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gigcquczn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/gfebewost.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/gkbyszrda.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/gzdteedhs.sHtML


<!-- 参考信息 -->