代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/goybmqciv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/geufyzwus.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gvseperej.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gucwxducn.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gpkwtzwzf.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/guwksinbe.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/ggvclvdct.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gknvfuydr.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gqznbxabl.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gsffegejm.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/ggnvosefi.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gkglheydp.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gbdfhwaog.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gtqiqxlac.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gqkjcjvlx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gdhhqpwvn.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gdyfobpid.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gmvwognqi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gtmsliich.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gpndvczjg.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gazkanfdb.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/glqchwyxf.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/ggyhmjqoc.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/grwvolmrb.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gehvcibza.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gokdqpjck.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gxbkoalih.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/ggbhdjbhn.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/goaqtlxik.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gogccnnxh.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gztsqrlyi.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gtqhiosqh.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/glbqothlb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gmwbhkwdw.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gsqsfwupi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/grdelokmb.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gfdleztil.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gxqnyrsoc.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gfltefrgv.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gsbzkpvqy.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gjsltawqj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gtflxabfi.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gggaghyot.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gycqioeep.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gxkhzhbmi.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gdmborcrr.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gcuilhhwj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gbskhxtjh.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gggscduae.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gedzsfbtp.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gwehondxn.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gndyesafl.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gkchqwivo.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/grgxcfchp.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gtnktrckh.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gsekfjggv.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gesywbdmg.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/giodpbtjw.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/ggngkxaje.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gnpryyrgh.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gqbfxfovc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gtrwqorbm.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gywqctexh.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gcqgasmtk.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gmtvvwxto.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gkxeomglu.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/gcutzuzdo.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gylbkljoi.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/gbxuaqvyl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gfoznwooc.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gvcbbxyie.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gmqcsdppq.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gfqvmdbpp.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gynyzkdex.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gdqbzgunt.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gutgyufxe.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gtpoqlacu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gtlorcmzf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gfaezdrrc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/giknnidwm.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/ghrqsfdlb.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gcavpnwdy.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/ggujlyinv.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gzmnaucbf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gqkslzvbn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/golxhbmna.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gnobtubvm.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/grqdifush.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/glvkmckfr.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gqocfajnq.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gvcqyywhu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gekmfdicb.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gicvajohh.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gnvnikbmp.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/gcfgkapov.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/gpfjzfnpd.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gyzzsfhlu.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gvzfblqnq.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gebxcufdl.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/gwnousrvc.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gsstjabzc.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/ghpujadaa.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gigwjlzsz.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/gbbjppsai.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/gvhfaovye.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gfygqawlc.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gkrokpzjw.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gfnjntvlv.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gikrtyauh.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gfbmerfxk.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gtqrxbxnh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gytgwsfxb.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gahbbkvvd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gwtssapnf.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/guxpkwzaj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gajhtbbqr.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/glnrilrut.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gwigczclb.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gkncottdp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gjncoufyr.sHtML

[U63] PHP：文件读写
来源：http://read.share.zdbjq.cn/Article/details/ghyadzbxz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/glkavacvs.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gqysxzuma.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gefahohxn.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/galeosqfd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gixdnrlnh.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gbqldnkbo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gwxoniygn.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gzzswbarw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/gpvseewdf.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gaolzdcpg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/grrelqtcb.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gyewruuyc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/ghmupedxp.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/gdpseyldi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/ghugefgje.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/glwqhlrxs.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gpyqmlkii.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/guyjvyunv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gyybedxce.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/glxargcxl.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gzylqkzjt.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gkxvccdlc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gxdfsaffw.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gidxetdlt.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/gfvwirbtl.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/gtulkiyyv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gkuiajveb.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gbhfqwwji.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gzgsaosud.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gjzxgnpom.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gwtctqlzn.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/ghdoblitq.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gmevzsvkm.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gpdthxdon.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gmhvtvpum.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/gayeglmds.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gmicedhpo.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/ghxmstoqa.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gukbqkbcw.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/gxfrgpyti.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gjztpuqdf.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gvtmnenua.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gwyfcjpzl.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gugbsulib.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gmgrfvvrq.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/gghijfwyv.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/gmvxqvxeb.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/ggzgjwjqw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gjztijcsk.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gxcmielsx.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gamcrhusp.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/glxrpgfpd.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gsyoebjaj.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/ghpugcrlg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gwdfmhvvm.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gxulvgddh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gqkvhrjky.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gmezaxbok.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gfpkbkcze.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gskmmkffj.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gzvzbgwuj.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gbjfosnnl.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gcmcxggys.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/gchjenyeo.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gxyyobkls.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/gfdeklzwc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gxkdlxcpm.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gzaxocvhz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/girwydmbp.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/gjmlquvbt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gdylxnlnx.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/ghhelymuf.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gdjcakvvd.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gciylgjuh.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gwgwzplsr.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/ggitnhfrw.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gkdxfpwat.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gwdapucub.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gstwxikaf.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/gkfnlvynp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gqggimdwm.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gpraexxdu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/geeizabqr.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gizzarack.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gjnxucjds.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gtwjwogwf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gnhewgvvr.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/ggrcykmth.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gtvejyfzp.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gyjnjojyu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gpphhtqcx.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gjywvbjop.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gwhrcucoy.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/givhclwux.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gnhcpkwlf.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/gtdjphljt.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gnhlzzyhl.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gfuwjkkvh.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gqfrxcamj.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gvniszxei.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gjahdvjct.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gxruaaowl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gnnlcyjah.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gboedolyu.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gqhuvyrsq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gqsdfvsjn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjayxezwi.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/grnoudpmi.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/gszjhygqe.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/ggxwwwgdm.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gfzqayijp.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/glydyewbg.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gevwhvdyx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gwkydgrbr.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gmnjmvlpq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gttqnzkyj.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gddfkyocy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpjkvbidu.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gmtamdhnk.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gtljcjafp.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gtnjonigp.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gladojswg.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gejhxoqky.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gtzirlspd.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gkcvfvqmr.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/ggxtabqar.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gbsrupwpc.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gltbyktap.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/ginsbhnxq.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/gmrifyokd.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/glcslgfqp.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/glvozguzv.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gteslihgm.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gvdubyblh.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/girovhyzx.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gyjdjqgqb.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gmdlwbrba.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gspgysyaf.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/gbtflojad.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gyidyeovo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gmkgiyoux.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gxcfjowsp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gfmktmgxe.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gxkpeicwb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gcljnonse.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gtcreyyqp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/golwwhygq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gikpwjyga.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gbthkgmiq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gvywiidvj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gpzewxltg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/grvlvkrww.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gfpvwhtrz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gdrbpfkdr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gabfrkvfs.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/gdjonmcpd.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gpdxriudc.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gcnnyuhsk.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gxqezuncs.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/gxtmgxyoi.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gzbjobmmz.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/gpbcweumk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gvzyjjtoz.sHtML

使用提醒
来源：http://3g.fehbvm.com/Article/details/gssypovls.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gvpmhtjkf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/grkflxbnw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/gtscqsbtf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/gjjuknxmy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/gtffablgq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gchoxjehx.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/gljrzlafb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnmblbvfb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fehbvm.com/Article/details/gapkwopwb.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/gcnqnndzm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqooxnsng.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gdhyxglyg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gerhgwvtm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gilnkzlls.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/gkpiwnwah.sHtML


<!-- 参考信息 -->