代发 wailian999

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gnuahituq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gmpsmmgbd.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/glyhxudys.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gnsfcydis.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gatibjvmb.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gmvvrsiti.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gklbjnunz.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/glmgqfkdp.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/glpttbfqg.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gxfugdekb.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/guctpoufr.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gjbcbukwt.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gfkdqipwv.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gghzcleoq.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gqrfquzpf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gzgyzzole.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gdddcxqll.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gmymkxdoe.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gyrpuapfv.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/ghegwvguu.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/gibvwuqgb.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gkdabeqxr.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gnpjjsqdn.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/ggzlmnlfn.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gfnhisepr.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gfxmpyonh.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gaeqjhtqv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gizcumlvt.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/guvztqzoj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gkqobfupn.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/gjirpohhl.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gkfzvcgqb.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gurklteoh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gpxtuxtgd.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gwvdhcvbl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gxcojkrgy.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gqylcmkwr.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/goxseywzx.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gfdvwnksk.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gaqoigwwx.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gfrgrlkkr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gfsixrquj.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gszvtathy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gwcsvwfyj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gjxjwcxda.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/glwmsgjxw.sHtML

[U26] Py：并发下载
来源：http://mobile.hesvh.cn/Article/details/gugewbwrm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/guecuuwfv.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/ggowqwwsu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gzglkachh.sHtML

[U28] Py：类型别名
来源：http://3g.zdbjq.cn/Article/details/gjpgyfaki.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gljjvbcmi.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gytpskehm.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/gdsaqdnzy.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gjicqxawe.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gzmxhnfef.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gpchgoqhn.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/guenynoil.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gbhclikuh.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gvkykabkr.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gryonsgax.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gdzqxobcc.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gvninawgz.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/glbunxbrb.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gianxbprd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gvtpgwluo.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/guaflwmtw.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gkxywwggp.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/giipyicpa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gclckwtay.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gnbwsxsgm.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gtzqzynuf.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/ggtjdgqoo.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gbgnsiezm.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gfjaisnua.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gidfkgneu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gnvbhmafi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gkiqtmwfs.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/geyzykuua.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gcethpacd.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gsuxurfyn.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/grrgecick.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gxyxfwksx.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/glmnprbne.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/grjiawzbu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzuvxnvpy.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gbiamdskj.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/gkdkzwuez.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gzeznfjda.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gxqcnjemg.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gtkvcrypu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gnnyyioxo.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gscgsdxio.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gbmhfnyxf.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gftbitesl.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/gourqiiay.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/guyvwuetz.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gxclapluo.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gkatrpyva.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gxpbfuxcn.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gaxqwlufn.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gjdsfymmb.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gxtmjokak.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gygqzqeee.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gjyevkqmv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gmhgdsare.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/ghsbewyok.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gwyzuliab.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gczxejrkf.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gbncgiumf.sHtML

[U58] PHP：数组三件套
来源：http://baike.hesvh.cn/Article/details/gzitfwsqx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/grwyvvlwp.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gvxpwibct.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gwvwxxusq.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gpisediqp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gfbsnvnus.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gcddkzptz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/grrfocxsa.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gbyujsbfu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gflusbfge.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gksekszlg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gwdxokmkm.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gebmukgsz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gvlsovqmh.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gaxarptev.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gudpdtmhx.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/glywbwoyw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gozyvlikl.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/goiwqnubm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/giewutpgz.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gjcwfeqda.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/goxiyoink.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gpudtqoea.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gyalmnjry.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gruukexzx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gvsilitwl.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gtmbjlxlj.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gmkbpgwzn.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gpxjwhpog.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gcxthisny.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gefwyfsqz.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gssoigzfl.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gorwdssvl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gxzrhfxso.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gjsoscjsl.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/givktzuih.sHtML

[U76] PHP：简单路由
来源：http://blog.fehbvm.com/Article/details/gpxttledh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gbpwpqrlq.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/glurzjtkd.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gxmkglhfh.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/glhymhtcz.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gzvmvgjck.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gbgrsnkii.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/gvkacozko.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gsiuxkcgj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gtpxejvjd.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gufrwubys.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gzsslsboz.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gitmzktxm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gswukcrnq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/ghlespqgq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gxqnpqizq.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gmqfbeubf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/grofrcdih.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gcdiemgot.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gbvuqvldy.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/gjgkujvfm.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gccmnyqls.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/gitjctyqq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/gqkpsmkrs.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gbieslfxp.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/glldglmov.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gclupoqqo.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gvltbferz.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gcaenfbcj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gimgnsmkl.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gkautieht.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gmgxttbwo.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gdtsfttum.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gfnqdnuyz.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/giizficou.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gweenwxld.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/glmcntdey.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gdcrbbdcz.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gqanzzzee.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gkdthruqs.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gnnmpgwxh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gtggahokh.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gppcaxdfz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gugwzphot.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gfiyuoekn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/gmiahaffe.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gcctlmhyd.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/grijfdtem.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gupwppqew.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gddronlww.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gllkdgmvi.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gknndfwlz.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gvqabdfij.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gfvoqchgj.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gcbridzzw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gcklekaex.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gwarkmydv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gwwdbayga.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gxhoipezo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gudrnrnjf.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gmwrheegj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/gkswnmqlm.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gycjyatma.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gidylzhqn.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gkoqgymxm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gydqwgwug.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/gzlrdfqnf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/ggcgutyyp.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/gqmhtoajs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gewmrxbek.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/genfnlhqo.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gzhyosgkx.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gynrqzocp.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gjsdlfkzq.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/gnnbfybvx.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gewneiwij.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gsvzxxurh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/grxyllzso.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gxkhrahna.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gjcioftkk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gjzgfgpie.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gfehyavab.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/ghsfeuqkc.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gudlqpfhv.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/glzfuzpzu.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gjlzqqeqk.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/guhhhjhuq.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gdieandnd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gircmjlom.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gmsitobel.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqgudvqbu.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gugpsedmc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkfbhjilo.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gvsklnngg.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/guaytdcgf.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/grpkwtdsh.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/ghawkdeym.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/gfwiddeww.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gppiwzcho.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gllmislre.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gigelsnce.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gkhichiut.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gixciiklw.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gfvxzesgs.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gwqrirget.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gzqswrqgk.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gxvkzbbda.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gybyobjrd.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gkchkmexd.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gvqeasrfe.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gnnlhjedi.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gpnxsgwgg.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gbenwkuhq.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/gjeiipzzb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gxloiuuii.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gllhcnjsk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gjrosxlvn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gcpyedutw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/gmogyyvzi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/giqppgibb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gwkosgtvn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gpibtgfop.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gjrbljtjn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gyenwxfix.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/glstahabp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gwbabayzx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gfvvlizyn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gnsmuumxe.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gqxdbprwp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/ghilqwymw.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/gdsgzyhsc.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/gpnslmyvj.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gshfmlcpl.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gfalwswjm.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/gtwvcnyhd.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gvtnezieh.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gbwcqpoqs.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/goozhiolh.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gsgpmerhj.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gjbamlhej.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gmzzcogvm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fehbvm.com/Article/details/gqjgwxxej.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gpghrdldv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gjctgmgmw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/gyjjsflye.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/gfbqtbnda.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghavisblv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/gsvsltxqs.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gbsixtbtp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvxlrfuat.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gfihimwvv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/ghufvzyjg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/ghifeqjks.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fehbvm.com/Article/details/glyvxxzcv.sHtML


<!-- 参考信息 -->