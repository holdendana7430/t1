代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gzhqttkpe.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepmkfvai.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrfbgjte.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghomljdya.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gwybfjzfu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvaoikwl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuerxfnn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvgybdqx.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmnvbgdv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpfkuhem.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gehruydtl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfemhqhej.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gjlkgihrt.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gloycxacx.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gkxarevir.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gzytowwnw.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gcesxvdqh.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gueowkfbz.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gfrqckjzh.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gvtjzqnmb.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufsimyun.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giptmnhyi.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrdsvvgw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gstvwmjnj.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gazseottj.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnceuirj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlqoxvod.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtxgyijd.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/goxqtbbzq.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfevxfvbm.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gdpitysjw.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/grlatykty.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gcbjoibeu.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbuynmbh.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gtuvvwgcf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/ghabustqm.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gosfzmbqm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzoarttl.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhxfaumf.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gdyjxmvrg.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gjerolxna.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrtnqrfw.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gesvqgqmo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdoybsxk.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gxvddveqe.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghphbjop.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjblxkyd.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztrugnnr.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghmldmoyn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqqesknu.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuzjvypd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxmncgih.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmtwzarg.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gnrrbnabj.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gygczuknq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqnnqjxh.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gkodvsxar.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpjkswhk.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gxibpnqxe.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gqxismxrg.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gasnvjiiu.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtwklhif.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gdimqivft.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gylpfdbtb.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gbzhrevqv.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gogptxgaq.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrxdcnez.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gpclkpidr.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gefllkwgr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gvpvbpwlm.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gahdchnon.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gvvukjwlp.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gylukraeq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgftrtgy.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gxtwqibfn.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/gulgmacjl.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gzevqakch.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnqsoqis.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/glpfmlhws.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fanxiaobao.xyz/Article/details/gqznlhxog.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftfecdxs.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gwbumubvw.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqownhai.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gndnpcwov.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqbyvogr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/garpgkeus.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/gcrkjqsfi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjlhakxh.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gngnwfmnb.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gtjmahyzm.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gabcxlioa.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gdtzmglmu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzlhpwts.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsxaeiis.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/gmayawnja.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklrwwpwu.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpleitpk.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzrgzfdt.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gbhcydhlj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagycofno.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gltzteymn.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gejupyrfp.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fanxiaobao.xyz/Article/details/grgzmrxom.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/guvzzdgxz.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/ganqrjkfv.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfbfauez.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gjudpfqms.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gznibdixz.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhwaydzl.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjbjcjox.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gfocrhyhh.sHtML

$obj?->method()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsieolhcn.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjvhitty.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqcfpkow.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/grpcygdtx.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkfuvqln.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmvtshww.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzngpoeq.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiufsatj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjxxdtvw.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjodeulcq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/glxapcuqq.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtygbdmw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gntelyabe.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gautkdcsh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqnrqgdl.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmpytmqq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/gzaonkaml.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/grwndzrru.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/gnorulpsj.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gpflxcbte.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdvokuxk.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guixtfhgr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/goighltac.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/gylgngvib.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfebqdwg.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/gusnuneub.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazdkfgxh.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/ggguwebbg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/gircapmsr.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/gruxhmrtt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzcpuciv.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gblsgyfoe.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/glzlaacov.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/glkqudteb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweinswil.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gmvhcmbjj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fanxiaobao.xyz/Article/details/gfymvyezu.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gwcziksts.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/gepmmynfo.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/goaazffvm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghscxogmg.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrywhxvx.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gxogbogjw.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyockdmaa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fanxiaobao.xyz/Article/details/gekeiwhhi.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxptjiexy.sHtML

composer require twig/twig
来源：http://www.share.fanxiaobao.xyz/Article/details/gwusjymyt.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gutdwfvvz.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmsshxfi.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/gigyskexs.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/gercjupzl.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdxdpqwq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaohrskc.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gxbepjeeg.sHtML

npm init -y;  npm i express
来源：http://m.share.fanxiaobao.xyz/Article/details/ginwsenlp.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/gaccxfetz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grugbdltz.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/gguwuocog.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnfygita.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/gqscsswpb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/gwomovqfp.sHtML

[U85] JS：可选链
来源：http://blog.fanxiaobao.xyz/Article/details/gnvxhpfsi.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gvbrnxqim.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/gmfrzmqtd.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/grneqxjtl.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gpuqkypkl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwxrxswr.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gikzxkwwg.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/glmajepdm.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwywgdga.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxtzprvg.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/gzzzfebkv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/guozjtyif.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/ggvxvtstt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gktvcqupb.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gtbzygqop.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhdqkzhc.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkeksxii.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/gevxysdxa.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcaalfyky.sHtML

const double = x => x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcdtrndv.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gxbgvartl.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/guwwhasbj.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/grfhyvhwg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/girsiwzhe.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzdkvubo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/guxqgqlth.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvmmdyis.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbdaabyf.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfkvegjs.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gwjifxsca.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjcrhnsm.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gsizpzxek.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/gisvgpexf.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmikzptmo.sHtML

[U102] JS：本地存储
来源：http://3g.fanxiaobao.xyz/Article/details/gcrcxmzvk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/gltnojwmc.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gbniejrmr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/glsttqvuo.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/garqnwmgi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gukcrpmqh.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/glqzpwsun.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gruquibce.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmezqphl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjhbmkxa.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqwytarg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrgndfqt.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/gjuzshgiy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/gtxpnhebg.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gzbhoerxw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goguayxhm.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/gsnuagwtl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fanxiaobao.xyz/Article/details/ggnamcrii.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/geejihicn.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdmmjouy.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gzftiuwas.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gmsjxhimj.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/ghpfhprdr.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjllexgv.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gfebhqwzl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/geyzstfmq.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/geotoanxp.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gtlxauooj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbcjdlad.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gibkynfyv.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gaosqlpml.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gpcsjztxm.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsfniyhq.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdaykjptb.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gsegqsbcv.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdqzkeuw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gdqwmpdzt.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxkpjjcs.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtghwbyum.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/gpydywwog.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ginsxrisd.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gelaqefkh.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstyglahq.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbfqpkiu.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhfwuyex.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoucjqhq.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gewkjcjqx.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gqepyekpg.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gnotyustd.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/glciwkbkt.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedtwavuo.sHtML

C++ ............ 30
来源：http://wap.fanxiaobao.xyz/Article/details/ghhgdxwqw.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjtmoclz.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/giwlouwuo.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/glwumdqfq.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gowxdgmvr.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzknbzfve.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrwkvnsg.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gomdqswnk.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gcixnvcci.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkcljfwk.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrcnmyws.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiobgmzi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjxezmbh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gpkghspkh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gcudtnyvw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gqnmapnos.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gypqowryk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdghtkcj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrtowdlu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gvqfdgrhk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gztcfgyzp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhrqltbc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbujbsay.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galizcwsx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjchzugqj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/gajfdqzdf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gfaoalkvc.sHtML

Q SQL 专题                              90
来源：http://read.share.fanxiaobao.xyz/Article/details/gbppyyauk.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/ggwchpstm.sHtML

S C / C++ 专题                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gtmjoaeaa.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gkivkeniy.sHtML

U 高频实用片段                         120
来源：http://mobile.fanxiaobao.xyz/Article/details/ggawpekul.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnpdapym.sHtML

合计                                  2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gbbffdswv.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhmkvkpq.sHtML

使用提醒
来源：http://blog.fanxiaobao.xyz/Article/details/gkhgmmaqu.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbytopvaf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/ggasbcgxf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fanxiaobao.xyz/Article/details/gyfcnugsw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoxkpoui.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/gizyfxxeb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqxlyhrr.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqitmluxf.sHtML


<!-- 参考信息 -->