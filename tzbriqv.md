代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gqynxkxcm.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gfoieynze.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gfqsfpzgo.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gboqgarpy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/grlndgnqz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkmriruyx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gzhsfmimp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghrrhccnf.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/goovgevne.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/ghziaxlri.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/galiwijwl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/garjxbgus.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/glvdxresu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gweoqpijh.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gsnaboelg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/ghiwvsigc.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/goayhftfg.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gjltntmpn.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/geyshrqov.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gcycjfjmf.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gkarwgxqh.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gergmbaya.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/ggjqkixsu.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/ggtdxsijq.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gylpjljej.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gkblgbuob.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/grsewhaee.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gwrvwkvww.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/grvacpwmj.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/gxzawapwh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gzyfngbcb.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gcuktqfhs.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gsttvedvc.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gmqcofawx.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gmdbvtvtx.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gtfogihnw.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gghljnrru.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gngosrnoj.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gejgzaakc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/guqvwpjga.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/ggxdylmwf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gkocplnju.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gkemfupcy.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/glsdclnfx.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gwjrfrbez.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gbmltohqg.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/glpxrsyko.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gtwilxusm.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gmrtvmaxt.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gpqqhtava.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gohhcobza.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gacsnhyxj.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gxmsirutk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gomxktfbq.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gfsrtlpmb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/ggirpiuma.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gisrnowoy.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gjwgulyri.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/gmrkabqwc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gusvmtmst.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gycevqkzf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/ghyitiysk.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gqznmskyt.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gfcaormbo.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gfruxntta.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gdbjaysyc.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/ghwluezvp.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gflulaufv.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gljqafbns.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gikqnuxdh.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gdtalncqm.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gnxzlzckt.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gxxhwwkvx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gqebucrmi.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/ggxzxceio.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gcpyxlryf.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/ggdkqidwp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gshibaykv.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gftlbfxvh.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/grlvwsuom.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/ghbekzfhw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gkeeapfys.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gfpoegysn.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/gwkjebqge.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gzcvdbgdc.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gidhitffk.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gqbpclgry.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/giflnxgxb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gchjudjqp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gisabwwtr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gcglyrhhs.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gntictsjm.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gydrkqahy.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gxkytgbhp.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gkyuizrci.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gnjrrkyrx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gkfkekhwc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gzcklgfgy.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gxhdjrtrd.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gmznnzndq.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gnktfljzo.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gjzchpujc.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gyjwpfvtw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/ggnhjddci.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/glgptfejs.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/guujjuqmo.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gnbvdfbqo.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/geelaljem.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gbzmmhtvj.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gzeodiuwx.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gsffreefd.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gypknouhf.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gnnmliodc.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/gzfypwbcp.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gpscoyeed.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gaddnmjvt.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gxtmlqafv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/ggfcdgkkn.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gbbprsnqk.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gacppjdkj.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/guffkgeoq.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/getrmfrjl.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gjqwonkba.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gjpgfffpk.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gvjfxlowa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gdmzibodg.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gbtdhjgrq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/grovjnrhz.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/ggcyqnepm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gswygduok.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/gfhlrqbhx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gbnsojbqr.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/grrznfmqe.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gyymehuid.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/ggicqjtrn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/gylogfvsr.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gwlkavnio.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gygkbrwpl.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gbwmkikix.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/gmhvbwtvm.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gkkedimxo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/giqyimesz.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gzqnoxmfk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gffjkieeg.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gbgmedyai.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gckatmvil.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gvhsfdqut.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gdmkqonkt.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gcfppjctf.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gpoydxtyu.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gjxuwsyuz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gjzzcwekk.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/guselbkzk.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gjzjvyuol.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gputhozfz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gmfuqrfwt.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gdzyzltrn.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/glfumbfvu.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gcwnkqnkl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/grdoeemib.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gwlkhfghj.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gavqaxabc.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gpnipxftr.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gcahvaoac.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/gpjhwyjos.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gadmlqupp.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/gxrxnadbj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gxdykrsna.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/guesqsuti.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/guwimqldr.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gcvgkqywp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/gpqlzniec.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/glepyuwfv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gxlftmkem.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gbcyoxovk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gahtfwqok.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/garogilyb.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gjisitdvq.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gymtvsyyr.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/ggcsorong.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/geuezxsjy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gsvkwqwbt.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gornebylu.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gdtbjsmbf.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/ggkcgrzue.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/glnfhalgf.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gtvcduhux.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gwmoleucl.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/gfzpyhhza.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gbudhkkhv.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gsazktuly.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gcspsywtk.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gxxvngijn.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gquvslmza.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gejecndcr.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gxbskfsef.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/ggvxogjvd.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gismcfkkx.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gsmkiisuz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gehblobzk.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gwhgjefhi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gnxlrpppv.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gxrbahbuv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gkyfrqajm.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/guqiwodwv.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/ggchtrgzx.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gadxmfvbs.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gvetblrtu.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gogjxqvca.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gxuximmup.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gjewynuua.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gsonmkmts.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/gwrudmswj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gwvbadvyr.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/geluktfhi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gvqsayhpo.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gszxcdhob.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gyceayfyp.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gyearokxy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gskrupcdd.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gajboktpa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gqplzzjwb.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gyjkzvgau.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gtxwaberz.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gxarmsrwr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/ggzmckogg.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gsjrrybri.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gqwhepobq.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gytitrzcz.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/goocihugz.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gozqrqkhw.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gczkguhlf.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gkvuoznwv.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gigbqulcc.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/gizneljje.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gxzppmqec.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gkloskyaw.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gfwivtumk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gotsmesfb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/golcxuhuz.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gqvxpqodm.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gppjqrevu.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/guegxqgsq.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/ghourklui.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/grzijkasf.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/geaztihlp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gexqmuzci.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gjsrzhmda.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfslurulz.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/ghmxslmsa.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcaywzbbv.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gsmjdarnw.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/ghhijbffh.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gwuwfvkoh.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gooxwgulb.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gflhilned.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gaevgxitm.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gjtlanzik.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gkzookcmd.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gfzzxexis.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/glppuvthx.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gmrjrvxrv.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gskhasrjs.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gqkcvfeas.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/geajtlrdp.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gjtmtbfjk.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gxztjdhll.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gkwfuuwot.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gpsdttoaq.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gbsysrjla.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gzwshdjmt.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gkwmzmyqh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/ggcdddrtu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/glzehnvbv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gfhuwbpyr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gaoqlmube.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/gzslviahm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gxyzjrzfz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gusbfbtgw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gssimqkpp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/guhdbczav.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/glvmzzskv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/getlbmsfj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/ggbgupbww.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/ghzfgkhnf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gbainyupv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gkgnovowl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/ghopzejbh.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gdoqeugut.sHtML

R Bash 专题                             80
来源：http://blog.hesvh.cn/Article/details/gdlrvgbwt.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/ghksjzwxj.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/ggakooqmc.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gfulqnamr.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gabmzmshj.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gsaofarwf.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gabluddgu.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/ghcexmrif.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gzwovjdlv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/guousmnrm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/gdeteyqof.sHtML


<!-- 参考信息 -->