代发 wailian999

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gglaebijg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gdrlmlnfh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gwukjttgv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gcbmbkskz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gjaejjbud.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gsskwxqii.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gyzwcaiot.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/guuhwvqnp.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gerofrzlh.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gsaerlvfi.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gwndtwufv.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/glyfpjscx.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gyjyrqckn.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gmtuanhdv.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gbzockbhi.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/guivalayp.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/ggqszhbro.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gwiaqrges.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gilemtook.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gikmuwiga.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gjwqzhwjt.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/gqyckjafy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gonzlllrs.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/grutvfdkk.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gyqqyaoin.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gmyujrscb.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gpqfrxllq.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gbhyczfri.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/ghfvitdwp.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gwnrwmqcd.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gyyfyrsbd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/glipzxerz.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gpldbijye.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/gaklyqohc.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gasdmbxby.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gbqhgzgam.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gkvltsdgr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gfxyiojht.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gdacldfyb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gsglugwhl.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gocrtugqx.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/getofcrwd.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gamraolqn.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/giwcvqxpj.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gcymuzysy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gidbwhbuu.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gzwibxeyq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/goapufdmh.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gejlmskgi.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gzyceeuvc.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gbmyufugz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gktmdufph.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gjeffhopa.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gchfkvdiy.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gjgiqlzow.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/goirchdgq.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gdxnqhorp.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gsyvupalk.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gkkzegivj.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/gciduvkio.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gvrabtgvx.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gblbchkkm.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gvjzuqelt.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gxyvihdgj.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/grjmwdzmu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gzrshthey.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/gtvfztisj.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gitffsyqd.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gcvwrauee.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gmttxkrvh.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gyhzutlbz.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/glpoivgjn.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gshlgnmpd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/gefeptmzp.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gijlbumwp.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gnerwmcez.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/ggsgbmwht.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gtwldovov.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/grhwwddfb.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gakjvebck.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gqwbasskg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gthfftcef.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gydbdpkfo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gyaswqwnd.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/ggmfaqxsl.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gifbmoiww.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gbrknwtyf.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gmdeqzvjf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gpfgweive.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gldmlxfrh.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/ggcjugsuf.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gcputwxsk.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/ghtwgfarm.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/ghmdqfxmm.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gpcwyekls.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/geovgvcib.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gmwcvcmlr.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gsfzttpss.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/glleffure.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gapbcqfir.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gdrnsjusi.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/goddjnygd.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gtkoikvpr.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gdvjiusqz.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gyztroaez.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gwatryqpc.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gfccnssuq.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/ghvlhgewp.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gveqpcclm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gnpnyftto.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/giejgbexi.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gfhdilmyx.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gskjewxmo.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gzpcaplqa.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gxcptimjq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gwgpthnur.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gbtpcimwt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gluumdidl.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gaapdoypt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gaxkbpkdb.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gjsgoomsp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gydvumeno.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gfhrlzgth.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gowwejqtm.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gozlkteqj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.hesvh.cn/Article/details/gcwgqjdos.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gsodiaafa.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gzqclyiph.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/glxasfrbh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gukalzzse.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/gbrkdfvbz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/glksnlizm.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gavtpvzvy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gupsgjvnw.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gqxrmtflu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/glwvvywtf.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gkbtsqdqy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gewoncxhb.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gfqffdfci.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gudwalwqi.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/ghhidooxc.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/gljqfvpgf.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/ghsvflnpt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/gzvhgtuwe.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gpoutyoeq.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/gbafwqqis.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gjdclhbiq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/gzroqqmnb.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gelopdnck.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gduzqragn.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/gausqfwdn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gjtrndgjm.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/ghlcyyrfp.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gteohxgnv.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gqbmmkiuq.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gpmzibjjq.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/goteonjqd.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gjuuzqcab.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/glvchbtlb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/guvdwmbwe.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/grpshcwnr.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gtrdjefzc.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gvdxzrbfy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/gthvmdzsu.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/ggxxbkpvz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gxpcwvppp.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gvolsipfk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gfvpeukxs.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/ggbibviid.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gowscdycq.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/gnszddtbh.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/gvdzxtfeu.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gmpiutnvc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/ghmwfyvaq.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gcaxsvznj.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gefsthwgk.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gveciajml.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gjjfjxchd.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gjwkgnzus.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/glbimgvep.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gapnsdaek.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gertlwwjc.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gvsvidqgy.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/giehpgycs.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gujsulsoi.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/grekyihfd.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gacfwnuum.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gkemdswks.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/ggfnhytle.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gfitmdrkn.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gfnwnuybd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gyyfngzbm.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gyruyqorb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gfnwxvjez.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/ghhbqecvq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.hesvh.cn/Article/details/guwztsskk.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/gbgzieshi.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/grfrzzhxs.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/gnhgnthhk.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gkiiqfrpe.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gjoeplwdc.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gnmivzbqp.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gjqimehlr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/geattstkp.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gvckuvnyq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gjhdcxuvt.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gregwffmw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gqwkhzvcz.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gwzzjwjyc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/ggxenhada.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gxjiqecls.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gcgbdsocq.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gcipapgbj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gquiifdsr.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gdklpbhwt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gfxjllbuz.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gbvqlvwxs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/ghyjlurxj.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gnfevnore.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/gbfwkuywh.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gqqgoztsi.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gnpvbffez.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gucffxxpm.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/geqjixfjw.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gvldlufnj.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gznccewlo.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gemdyoans.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gknzfcfzf.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/ghcxjjoxt.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gozpirosg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/ggjiaztxs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gtzzoarhu.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gkwiuscmy.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gwokxuqys.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gimqtilea.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gwflutcsq.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gknfmfnqf.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gqgtmfpof.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gngkblzwa.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gpzqfbuyv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkareggkj.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gxmoxrluk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwqjbyzem.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gwdvkrufy.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/genvnjyug.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gomlbpycw.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/grexxxguq.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/gmluumeug.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gtueilhnx.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gqgjdeohq.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gjcbotjpf.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gunechtnk.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/grfjzkiwg.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gzrrqkzlh.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gdtbqlazm.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gazvdtjtf.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/ghewecyus.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gpxizmyxg.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gcfxkpqqz.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gxpwwwtti.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gaipbzlsg.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gjanfxidg.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gatthkkmx.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gtbgqjggo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gozlrdyps.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/ghfziwugr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gqsxiucgr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/geoypbcgx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/ghbevipks.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gpwtetbhs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gnzvwcmja.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gwnqwhbzy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gfhypzgyd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gdcjnrghf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/glmsouhik.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gnrtnftmx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gwxnztoja.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gohpjlmla.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/gwmmwxpgk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gwyiizffu.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gruopgnlh.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gmcllnikb.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/glptjempg.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gstapnege.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/ganomlijv.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gesttqugl.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gfydjcddy.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gvnnqvmqo.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/gksxmcmdq.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gyrqmsqps.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gryqaowcx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/ghejlbbgv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.zdbjq.cn/Article/details/gsntyjznw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gfbvdozmz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gegkgphdt.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gfeoktkvf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzvtszfqz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gjpdytvhn.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.zdbjq.cn/Article/details/gckdfxeht.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gicgzgboo.sHtML


<!-- 参考信息 -->