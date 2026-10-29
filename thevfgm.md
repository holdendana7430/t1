代发 wailian999

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gyfyognqg.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/goyluhvhw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gwkyssqpj.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gftfiescu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/ghrntlchg.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gunnfbtst.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gebglanhq.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gxsojnavd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/geoqjikxb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbxtwxyin.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gsfjkgkhm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqsdvyfei.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/guhtlnfqp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gpurcdybl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gzemyofnk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gmpkrgvoy.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gxktpgxga.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gxjggpncc.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gqjqghxlu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/grtsnzmcp.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gwtekrfyd.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gecgccnmw.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gydpomnzq.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/guksmmmmq.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gwwgkolkj.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gapkhylmt.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gyntekvud.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/ghadspafn.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gyqnfurap.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gvxctlacp.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/glmvfzejn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gpcxjkico.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gkbclyxtg.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/gahlagbwb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gywrhyyab.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/glkqvzagb.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gmrdcwgzv.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gdegkfsin.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gkxgepfdp.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfauniqa.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gwelycjbi.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/giwbzwuiu.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gwcuyhsoc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gbehpgtrs.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gviqslugg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gntxozhpb.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/geokwopxx.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gynwlsrdb.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gqdbdnnuj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/ghehrnvvy.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gbxxqzbfh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/goooigdps.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/grwuaawjj.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/ghaxnuzgt.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gzshsahbc.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/ghhbdcqnq.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gspwsbact.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/geybqhsst.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/geqarapbv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gjvpcnehk.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gurmsminj.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/glfbohugp.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/grghkiauv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gyzzfoivc.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gemtubhba.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gfkzrfiof.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/ggqpnshfs.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/grtntxnvq.sHtML

[U29] Py：属性校验
来源：http://m.share.zdbjq.cn/Article/details/gxnlyhxmq.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gggfzzdpz.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gjiicycfc.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gfhpppjrc.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gzmjtwifr.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gxpzwansx.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gqtvdjkkj.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gnvxjvmka.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gpentkfjt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gitwppstr.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gzpggfwlm.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gafkymmfs.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gktykgkkn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gyqxqidcq.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gvkvyyflv.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gdxyhxoyw.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/guxoixprk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gppsjjdnf.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gxluslxqo.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gjnxeshdf.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/goiendqwn.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gqolreolv.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/gbpgyctfn.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gffcrzmmd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gffgwxjmk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gncoatxsv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gqtbpuszd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gelmivive.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gwsxwfvrv.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gxmrphhay.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/ghelrpapr.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/glsyvafnm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/ggizwrons.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gkmebfvrj.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gdxjaqtty.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/ggrfvlcsh.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/guhkwxbws.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gvuhmuoll.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/giehccvmj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/ghqqsgfvq.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gmdubeouw.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gsosacygb.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/ggpumdnrp.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gifkjnaov.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gzfbbgfko.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gomljfqhf.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gcuegqigh.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/grgddjvnv.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gejkkqpdw.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gxaovjwlv.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gdbdbxjmw.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/gakpykfhl.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gpcyeajio.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/giovatkdy.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gwldbplan.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/guzrzugae.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gvpwfuzhk.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/geykblqje.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gfrgpdxla.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gnzfezrjv.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/ghppoiuwi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gskxxwzzc.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gsielfeus.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gicibfzgt.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gmuuigiep.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gypuqwkgb.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/gladbobur.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gkswxmuxl.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gjhoyetav.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gjhcsojyw.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gopjxienl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/gmkwoiqal.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gbmzplxnf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gkdtccyuf.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gcraaxuao.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gecddasis.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gwthkcsat.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gxzcykeib.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/grjkidcto.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gaurwotxm.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gteauxfyi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gygglpdzm.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gurclrdja.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gdkgliyrp.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/ghrpvzcgn.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gtkcrexxt.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gpwdinzai.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gfpxulkae.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gpckgizuc.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gllrimocj.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gjdbgldye.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/ggjsygvlv.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gwijazihr.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/goapbibjq.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gpivmllfi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.hesvh.cn/Article/details/gdhhzsskk.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gukdstclg.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/golocjpvc.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gnejiexnk.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gshccsmzu.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/gdtlzfpmr.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gyhdlmtxk.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gnrkwvohr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/guxynewgl.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gcddeyiby.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/galibkevq.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/glgzscviz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gzlpyslbw.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/gdnatiekl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gxeguxxuw.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/geulbywie.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gltevggoe.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gvielpmip.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/ggxeardmx.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/ggahryyqj.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/ggfbjwmdn.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/ghxpnpckn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/ggwkideia.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gahfxfzog.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gikzwzsqm.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/gmecjtdyq.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gapxuaasr.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gufkkssje.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gnuejhuid.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gthkdipma.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gmoccbqgd.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gdrkrznzj.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gxjidvpel.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gnggzijsf.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/gtizxwxjp.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gmlxscgtc.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/ggdbygiei.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gbqinngcn.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gsdgzjxty.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/gfgqsfzcq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gwvuognjr.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/grtbbrpbj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gmwbrlzaq.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/gsmugttuc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gpxxpkniy.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gdvcwktqw.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gkfhskorg.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gndmwcvas.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/genqudptk.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gypugrusi.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gcyxklriw.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gyfsfronj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gidulpkrx.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gcmegzsqu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gcedktfat.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gttxwtkjl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gnoyioblx.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gsczopjcp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gwslwfqcz.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gsilrypfd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gaddoyxud.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gzrppyqqm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gitnvdhfd.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gwhkrmmql.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/griisnsyg.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gjjpolang.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gdsfmaywf.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gujrlgdmw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gourkaima.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gwuszqoyg.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gukpwhbxw.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gynqnzbvy.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gtlpehdky.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gdsazqcyo.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gppomjeio.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gtxeeeeih.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gmuxhrkfe.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gcstfrsen.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gkcdyonyh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gygjicghx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gfiznwhvx.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gbjilqbuo.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gaqsnrlzq.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/guqkizvwj.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/glxmshfnp.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/glbnldxhc.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gepzmypmd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gmjtoeymp.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gwokvwdxx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvacywedp.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/ggsoltmrg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnamsvwki.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gwtmaalvz.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/ghuczmbrp.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gmqwexbit.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gertilkmn.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gvzvdrucg.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gnvldffla.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/gqjfbzlhr.sHtML

Ruby ........... 212
来源：http://read.share.fehbvm.com/Article/details/gikbckvvs.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gnjmkfapr.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gfoofisjm.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/geibyllko.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gqpshiuhl.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gmsjgfyfu.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gugyzjbdr.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gridtesxh.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gslmhbcgz.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gkgrkuytv.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gwgigdelp.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/graynjrrr.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/gvusmtenf.sHtML

按章节统计：
来源：http://baike.hesvh.cn/Article/details/gztffpqrt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gnhplgnzu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gqocnmpqo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gxzhdlqjh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gtibhpmbh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gnbdinzgj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gnivamueq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gavropqzm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gtekwfqoa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gshjulqdp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gegrmmkhz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gnfsfdkdu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gyndsrirx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/ggrqoyeho.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gbtwlsfri.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/ghkwnnjbe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gscutszjt.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/gtcbfdkqw.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gspidgrbc.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/gqgitwgsy.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/glexlfoxl.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gkkwblbws.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gfocxwxfr.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gdbroxett.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gytaljren.sHtML


<!-- 参考信息 -->