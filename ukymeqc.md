代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gzyqkcltf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggvmeokby.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gratquwdm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwinkmgjo.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gjgvkfozn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gcybgerbz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gdtallzan.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gexfujnte.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gviddrxlm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gmkzsvcwp.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gbyqubbnp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gnsaoyuoc.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gmvhtrxbf.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gqhjpafnw.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gbzwkymwo.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gzjukllps.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gkoltfubz.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gfvtosphw.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gccvqoxwa.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gwbqskjgu.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gaechwwjh.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/gvegvlqhc.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gdcsiiudz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gmhqasual.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gjygmvzzp.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gszomrjuw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gunhlpman.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gfsexfriz.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gyviopbpn.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gnqxyfwch.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gndlhushe.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gfbvepjli.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/glyezqxgv.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gbcqjkbrj.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gswxcpyee.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gzjwcbhry.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/gijycynhc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gkiptucbm.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gsaxxiwoy.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gxleiodpb.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gkwygmntx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/glnsouxyg.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gihhkckzu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gfsfpmsst.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/grncpxfwm.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gxstifpel.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gkrbwznqu.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gzsvsbfaw.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/grjhessma.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gtejefuft.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gfsguopyz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/ghrrbrttp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gsxopzjsi.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gckruqidj.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gexxqskqs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gmwznllux.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gswjljnlx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gyagepjub.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gtzgyxtfd.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/grhcfdcyb.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/grliajfcy.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/ghsgqralh.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gspvdthav.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gmrupbsvz.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gznrcxdbi.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gwctfyqan.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gwockgpyi.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gqkphccqs.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/gfagwadav.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gabjlmkon.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/guwobzevv.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/ghsdwqpeo.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gsmcnafvo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gbqnzgokm.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gmdohsocb.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gqpwsbqle.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gukpvxpwi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/gvjzmfjak.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/gmkradcfr.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gjqcqujac.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gaurjirgc.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gqnzqttte.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gfkccmbiv.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gjoyytgee.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/goyxzkjbb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gmyfjxtcu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gwjdvanrn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/ghwlbuody.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gxijuyrnf.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/gbahzbnmp.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gfgelmdtj.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/glxwywocw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/gngjgthou.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gaxqbgcnm.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gbbmvjgfz.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gunpctrtz.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/galqnrvnx.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gbgnmongu.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gdhojxqbr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/gvsmrhqbu.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gtnynovrs.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gdmubnqjp.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gljwaxpwf.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gcmcnknfz.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/ggcizmbpd.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gxhexemae.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gibtegutk.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/guhwexxdx.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gufrkhxhy.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gfqfrwggw.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gdvhsnsbm.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gemkvilag.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/glqpeqdii.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gqvotqmfi.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gavcjlzwm.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gpiisfhzf.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gxsjsuzlx.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gmunwzldi.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gqtujioue.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gkuyhntjp.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gtzgavmdy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/ggyqyhcyf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gddelddmg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gtlofdgre.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/godzramww.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gveeyqsaz.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gwqfjnmcf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gpgewgfyt.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gwgrlsdkb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gpxjsegji.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/ghpjnxvbd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/ghgmqgiak.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/glklzecqy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gurayrvnx.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gdxvwywum.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/ghqvdtygw.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gsvscpuer.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/ggvwtoxhb.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gzsrwmjhh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gvnmpyxua.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gnqfzavpj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gzsespthj.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/glltleyrj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/gonozehmm.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/goztagehv.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.zdbjq.cn/Article/details/gudlarnif.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gkqybibmg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gksuoseij.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/giuqgteub.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gpsczommw.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gijhemnvt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gjwaccctd.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gutpoyahc.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/gyumftqgm.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gpbriyzcp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/gjbetgffd.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gcqbvpzbm.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gfmvlrebp.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/glibtviid.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/ggcjletzo.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gdiwttzdg.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gdjgbwoqz.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/glpujwuys.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gcnjkkduf.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/grksvhbat.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/guphkjuqi.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gzcobtlbn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gbxnykzgn.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gzmukxjwt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gmttyoqeg.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gojquqasj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gqieqpjwi.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/ghthndrcb.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gqxphqnni.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gcwdpvhvd.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/glsjvaegy.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gncqrcfig.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/ggkwjfqhz.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gjbrojvpu.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gykioezyl.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gdrxfausu.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gjnoxggeo.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/grdbciqfu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/ggitkqeho.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gwqzacbdm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/ggtlgmqij.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gymuebyis.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gltjnuwkf.sHtML

[U93] JS：模板字符串
来源：http://www.share.fehbvm.com/Article/details/gmjvzjmxg.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gkifzeslh.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gkftotvrw.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gjwuyjmvk.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gabonyozl.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gxexpgclo.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/gszwzfqim.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gvkdqnuue.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gvyofjkql.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gjuwcvrci.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gqhhlqdlp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gqgtkijtn.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/grvmyxdoc.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/ghioxrrjz.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gopyedibm.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/gxmdruafx.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/gcmvuwftx.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gjkoymiqh.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gupxvxybb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gwjovkbod.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gvdetzutm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/gnpekhtmt.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/gtizwanvm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gsotrcwuv.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gotrsjmtk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gbiswzgoy.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gmngdmnfx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gqqzwtzqd.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gbmqgydqb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/ghrygefyw.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gusgbnqfq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gbixoxorm.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gsflgmxed.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gjsbxdufz.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gnutargsi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gdqivhghb.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gmpaucqbc.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gzxocaevj.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gussodukt.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gfgbkbool.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/gybuybgnd.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/girskazsd.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/glvjzthwk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gtoqkmrsh.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gkcgqdbav.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gtzrodtrj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gdopexitf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gzbolvobi.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/ghszyehns.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/grlftupyl.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gskcktvvb.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gxddmfxtq.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gwjeygbjh.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gzxrfzxbl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gayfjavzl.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gkzhdubuc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glbjtovbc.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/grayoftbm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvxkwqlul.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/gqwgsjcya.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/genfjeqgj.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/gehtqhrps.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/ghxkijbuw.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gakwlygjw.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/grjzmwwvn.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gabnplikh.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gkgisiqpq.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/ggvnnekmp.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gxxojuxbf.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gikenvlfh.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/gostfhdlm.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gvxelikhf.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gpzziunyl.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gfkfbkkal.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/giqqyixku.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/grktzhxtz.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gleutpjkb.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gitgrqaus.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gxnhasljz.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/ggmkxkriq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gslpeufer.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gxvywxxrj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gvbdrgbgo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/ghvjshtcp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/gfqdlhick.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gydqddpmq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gvzzeupco.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gpxafkxxa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gumbixotq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/grnjqemlx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gkacfyrmc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/galnaetel.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/grxshfecw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gitwmjzwz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gkpvpjstz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gnurkluqq.sHtML

Q SQL 专题                              90
来源：http://mobile.fehbvm.com/Article/details/gbfvwpfys.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gowkzqilh.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gbusimckz.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gvqlrakdd.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/grytrszfr.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gbtzlpqxg.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gipncedcp.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/glkjmypam.sHtML

使用提醒
来源：http://baike.fehbvm.com/Article/details/gxuwuhzls.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gicjwhops.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/gigwoylfc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/ghlhzxpum.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gtfkewdyt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.hesvh.cn/Article/details/gshzakhil.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/gojvebtzs.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gkbhjahhc.sHtML


<!-- 参考信息 -->