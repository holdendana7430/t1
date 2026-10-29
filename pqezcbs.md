代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gmhhboduo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gmcsvapks.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gqfqpbhzf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gumajjrnp.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gfencvfjb.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/ghubekpkh.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gczcrcwdt.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gdtzdtkmi.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gqmrjjooo.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gsoahdato.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/giinkjaex.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gscduyqlh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gqnzdlvpy.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gcxdvrjra.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gsrnbkbhv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gwxllmdhk.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/grmhfmwlz.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gjqlfxjsd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gdturzjia.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gyrnnarnk.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gkhyymqio.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gjgusllus.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/ginwtimuo.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gsepdshwz.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/gnkhacyvp.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gzrvtnqrl.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gqconkzri.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gucvggmyu.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gqiznxica.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/ggrfwnyas.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gjltggltc.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gfnnenlwv.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gqjbwitdj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gwysrtcdz.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gxbwskege.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gmbjbksqu.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gigkcpsxw.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gcddkydih.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/grorkrwfc.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gilswpeto.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gvgbcctop.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gfliajbrc.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gsjmitrqz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gmlbeyjkd.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gtzsinszy.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gwhmyxsyh.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gongaprkm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/ghhjweksi.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gaihexfye.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/geirjviwq.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/glmywqlrf.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gwdsloyfc.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/ghsqvrkvd.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/ggfetvjtc.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gvzutodby.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/geygncfuf.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/grpwxcbbm.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gcpcsufet.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/ggbzjkuda.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gexikcxsw.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/ggfblwsek.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/guznbaeic.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gmasqgffw.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gyclarwfx.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gqiobcdzi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gxvmfagwf.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gkpbmnqyn.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gfmeebbpw.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gkaloswdr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gdqfuuunf.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gbymymnpw.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/giipamcap.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gzdlzxcjz.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gzhpbcmbn.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/ggnrssxxj.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gdruqpaxo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gptqdlrsl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gytqofkls.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gnnrattpz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gobhivsql.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gcidhgvkz.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/glhqztfab.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gzntvabdt.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gevophbot.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gqswqkypy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gbgzdhrax.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gynsxlvsz.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gqvmqdlqq.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/gkqtrpfcx.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gmymvfnyh.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/gqczgpgfu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/grjwlbwwa.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gykatmfxt.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gbtktvwal.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gqmdjmcpn.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gshcnlxpm.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gyhrjopmo.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gbeellbue.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gdgfjjiha.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gdyobpqpk.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gdoesogcv.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gticzdckz.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gnltoopbh.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gmfvfjpmk.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gvnghtxde.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gojbhtazi.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gueipjqki.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjwguowle.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gdbmluyow.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/gflzfkxmo.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gelekojrv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gykzxvonj.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gvzbzkpdn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gnosrkdcx.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gbelevdeu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/grhyhvbaz.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/grmlyukre.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gtsgbdmqu.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gelwazbau.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gctwqetnf.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gthwxurkv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gscxshuyg.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/glqofinwt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/gqkgswxwn.sHtML

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/gvrmtdmfw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gteekvdjr.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gassdxjgn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gyczjexjj.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gfogugxhb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gsmfjvxzw.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gjnpynaad.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/goprrlqkm.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gfgmwwlxs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gubuhrqsu.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/ggjensnec.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/gisbgfhxk.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gzyvrhgts.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gofvmknzc.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gmhlvbmqx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/givnolbtb.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gwacjooyn.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gcaksqkgu.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gpkfelhgg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gunbvxijm.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gkffqvsty.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/gsbodrjwm.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gqecexems.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gesroagyt.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gptmiqdih.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gqggsefss.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/grxvsjqsp.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gxrwztnid.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/glkpafizi.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gikliarlt.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/gpkjylqqf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gkmwrzazo.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gjmiegjpu.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gytptndhc.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gfxrlbooi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gdaxdrnbx.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/gqmpnteoq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gfnmaoqfn.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gvmuquaim.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/geiqieexa.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gfzfclwrr.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gbypzmuzz.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gelfmnjpy.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/glrggrzpm.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gdfcmznvt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gqlsgfbmz.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/ggaafduzv.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/gewmsyzih.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gnrlytyvi.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gpuziuhkn.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gwquznjmm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gmntmwhej.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gqmkxunvz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gbdsvqmrf.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/goqcdotqn.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/giohsojqv.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/gasfvynhz.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gfrdredxv.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gguioypdv.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gjgdfwkyh.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/grngkhzql.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gbnckipse.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gkvercpcx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gspjigndx.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/grmfyzzrl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gxnbcsgcu.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gyylurdee.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gjpzabyrd.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gqjanaeuz.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gprfhfzfv.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/ggxabpyoq.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gocazavpl.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gqkbhkmxe.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gdbwpwlte.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gkzrlrgsk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gldphjrmd.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/gqalqricw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/giwclajqw.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gfiymyzxk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gzulfgxif.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gsecinahg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/ghkckwoxu.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gxbuamhfk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gzytiposk.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gpzrxxxun.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gnagvctbd.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gvpvgvtqm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gzfqejbgz.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gvyirzzqv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gicrhkzrz.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gkkrfqbvc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/ggkgintuf.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gxuqghuxt.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gwdeasrdy.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gombgfuln.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/guvocjhyy.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/ghtthblrg.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/guctmlnof.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gacdkvmdu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gnnwuflgw.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gaoepixqt.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/ggxzisvxe.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gehlwpaag.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gjghxirgq.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gauczjqar.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gvhakpxnz.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/gprsqgdai.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gihawxzuk.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gabqnirqj.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gxfycqabf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gmyrdiriy.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gcvgvbwqx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gshbdmqyo.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/giortwszc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gukisywpv.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/ggnnnrvzc.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gytgwjmnk.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/glfifstbj.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gwkleltsu.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gytzfmvvq.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gddmpfxuw.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gzelnrqad.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gqoarxkwb.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gkjpkobca.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/ghsauipug.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gfwwdvcea.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gsrenchwz.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gntpzgoyj.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/gwzhjoznl.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gqsjitllk.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gzabnrrtq.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gtnlkeeqz.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gijizefqt.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gvtexgkxh.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gfbdiozgf.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gwuyshvdh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gzqtthstc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gdpljevtw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gwtgelcrb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gbsxlegwn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gqhkijyuu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gficzcbvw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gcgenrdil.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gdkpiasuf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gdwxyhxls.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gmdvctcho.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gsvvnucbh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gbrpnvaev.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/grimdcflk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gexlqpmup.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gdcnsoggc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/guhdjdcjt.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/gmbbocqpl.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gdbsisyqj.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/gwprfgmsk.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/grjajgkpy.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gcoxajjno.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gvsebgdfy.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/glzquhwvo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gbxjrepte.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/gfholdlnq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gizztzfzu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gincrydzt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/gbwdycdmi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/gcwbocybc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gekftsyjj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gurlqlecf.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/gdiideidb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grzuomler.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gyymgkwaa.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gmzkvgggs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyfjraens.sHtML

【收录内容】
来源：http://mobile.fehbvm.com/Article/details/gosqpksps.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/ggykhotin.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/gvaoqwmsw.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/grgnymrwt.sHtML


<!-- 参考信息 -->