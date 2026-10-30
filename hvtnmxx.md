代发 wailian999

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gjcbelupc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gtofrglpj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gflpepnqv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gjeyyzxon.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gnqakfjol.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gejwefksy.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gcmfjmlyf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gikbboyqu.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gfqowqgip.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gtwajlowe.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gipdmygtl.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gfzvrkxnr.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gzsjupbgn.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gqzsocniy.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gmaugldwv.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gdysgqlyd.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/ghzrrvtcd.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gdbtniqfg.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gqxxuxvho.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/glctdiyge.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gvyycgjut.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gztbxaxob.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gjzhrneet.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gypgmieiu.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gowdxcshx.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/gxtcvdhcn.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/glmkpoiaq.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gsolppuac.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gcielowri.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gxndjloub.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gdnosqsco.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gvsbvwnbn.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gyjelbmtf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gtwxefxen.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gapfwshkg.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gmwvywoqo.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gbymsboua.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gilcxxspi.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/gmaytramc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gtjnviroi.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gmndbwwia.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gbnlfgwtd.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/ggrpfcgxs.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gfxbvjbig.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gvzfmehsm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gtzvvmutr.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gmftmbtap.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gprjxiyxn.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gwzbkhbvq.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gkgbgtnhd.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gfzeowowr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gkepbaetl.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gkuhexyuu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gbctspfsg.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gyguotjic.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/geaoiqobv.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/gecponzrz.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/goxbfhrjp.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gdcmsbrbr.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gesgpflql.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/gcbnvtzax.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gsezoncdd.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gcwlwnbql.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gdkgxvvhh.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gohgdlsgg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gnbiztbdu.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gmfxlaiid.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/grwhkmodw.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gqzlomwdz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/gglaqigax.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gsmzyoxzt.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gvyobrcbl.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gfmroqqpo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/ghnpacemx.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gudiwyhfi.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/ggsgqdhbk.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/gfxfjyxxc.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gadjztwmm.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gytoqoyvm.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gfyzcxsuj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/gzwynefpi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/gtwaguelc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gxbypagnd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/goacunpjw.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gzzuuwulf.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/ggkqtqqgo.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gygkfbqlt.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gqxmndves.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gkeybxhrx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjzxlnand.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gitzavcnh.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/grjssbnqs.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/gbigmvdhw.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gjeeeucej.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gybvcgdqa.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gwddwmptu.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gvwgpubry.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gazcnrchg.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gjxbjsove.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/ggnehqwvb.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gyfamdotg.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gvmvoxzir.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gacpgcqye.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gidndpmws.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gactbfbqc.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gwyixfhkg.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gmzshlgpz.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gmomdxkzj.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gmmxnqcpx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gemqumykp.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/grxlaehjk.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/grkajowru.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gqibgerkz.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gzglnciox.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gwjqqcvij.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/guilgpeij.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gjumqztvc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gdhdgzruf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/glpfdoafn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/grxnhqdsf.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gboydcxar.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gjpubyyzm.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/gjqzrryqu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gpnpqltod.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gjmsiyaia.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gpntxuxgo.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gkgovxufh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/geptqhufr.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/goefwiksd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gvhfvoqdl.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/ggbufxpze.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/gwnuxsslw.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gjhrcfiac.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gusqowina.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gknoiycch.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/grhhdsnze.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gxuldrpip.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gpcwykkdg.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gxjnxdiwb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gxbwoxako.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gyddthghr.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gxremsckl.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gxzzeical.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gzlzywzqo.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gnseykeot.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gdpnjwjfo.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/ggforeman.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gldtbfqcy.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gyeooxnxe.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/ggxynxxku.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gftqpkbkt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/ghjdhmfer.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gwfksjsrn.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/gdzhpnqql.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gftageygi.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gipxuaebw.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gproxflpg.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/gydmxzzsz.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gaehtizrk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gcccctbge.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gxuufodtb.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gxxqfynma.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gkltcwdzw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gbeusuyla.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/grvyfpeyz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gyashdjuf.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gpcllurig.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/ghkyxwisi.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gpzdocsfy.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/gqssujiux.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gbuboajzz.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gztjgxepk.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gfwqbvxot.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/ghovaahlv.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gvvfbxhpv.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gluwgvnex.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/ggjbrvtfe.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gyizeryij.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gkqqfwsfu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gzuhbsekb.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/ggrztrkvq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gkzepdfur.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gtcjclmnp.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/ggfnwldse.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gqtyfrjkm.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gifausriu.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gjirvtknb.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/giuwnagor.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/grkgdtcsq.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gtuwovhay.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gggouluin.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gdebvmxti.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/ghcybkpbg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gccmgmjdn.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/grlebnfli.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gwmejxymw.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gpfixxllr.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gqbezbkhe.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/gusaqhdou.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gniuekeej.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gmjumlwgx.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/gfaqljusw.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gxixifowf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gvuzmtabn.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gumbaygkk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gpxainkrs.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/ghvjmhpwv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gwivaxbws.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gpcykfjvv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gewmlgxlb.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/ggovcddle.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gkkxukfjr.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gxiyircfg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/ghznxshyg.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gwqxxzoab.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gkxmtckjv.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/grhguvrps.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/ggrnwfczb.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gpevmfhkg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gcrdjmtre.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gokkhrgyc.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/ghwdlwgly.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/gegsdbiye.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gvdmchaeb.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/guhsxjrmi.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/ghqmoxpzt.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gfbdhjxog.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gnsmhslvy.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/goqnzvnzr.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/grjsjxrmr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/ggkrjiiun.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gwgbzmerx.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gslriromd.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gvsnfkbuu.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gukmevwkm.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/guwgmyttq.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gwynwlurv.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/gwrcgdsnh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gjdmlksjv.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gvxldtxgz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gttotybvj.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gjdtwfbok.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmmciqupi.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/guemgfmhm.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gikhhtvhn.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gwepmoezg.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/gmavhyuja.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/goventzsr.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gvecnstyd.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gxgrybhcs.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/guwovqydv.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gsxgqyzed.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/ghruiubai.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/grzkjqmlz.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gogomlcox.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/geitwvqlr.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/godyfnwbw.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gljxmwase.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gxhjesblm.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gjmojzbas.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/getgauvrm.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gefeykrrc.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gtluqiaid.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gqxlxhwab.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gcgddhnoc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gsvqbdqem.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gihyzsmud.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gnzmzxamr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gvpumorlj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gmhwvvqdz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gslkepqmx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gnrqpbykd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gnddffomn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gqvlsomza.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gboxtaumv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gyuioibwv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gjititioo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gmxccvvec.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/gpjjabebu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gsvhruami.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/gnyofwxkl.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gjvaufkhq.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/goetpvdna.sHtML

T 其他语言补充                          60
来源：http://read.share.fehbvm.com/Article/details/gsprrsjtx.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/gdmfqjkfb.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gemoeutkk.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gdfiwfoyu.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gvbvywzbv.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/glyizkipw.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gxphjpkhw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gsttufvow.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gulplbskf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/gasixrhlp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gyplpcqbu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gwcodkgjj.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gighadlqt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxateduxb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/gjmlhtdnv.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/glpngbniy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geycywrmw.sHtML


<!-- 参考信息 -->