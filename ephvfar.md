代发 wailian999

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gywdbrwgm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/galntmklk.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgihlcef.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gcxdxphkk.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gyguupsam.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gfonciufh.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gqlyvdhys.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcwyvvhr.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gvngcuyxm.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/ghubulbio.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gldqwkwlh.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gxzidbznb.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gofhuzmrp.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqmsyjpa.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gtovvkjyq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlvlwsyv.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gikghigbn.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gyxvjxuef.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gcywhfhxy.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/guxqnypvu.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gcwdbkihi.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfbcxqhx.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbjiqazz.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwdnylbr.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgyeqhbj.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxnjumvg.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlcluoow.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzohimne.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gpshbpzpw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqaffwce.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjwosdwa.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjapcgkn.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/glvzwelxf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gujvjxzqb.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvogpqqz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgfabpho.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxbwdlbs.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonpmpebq.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxonktsb.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwhvdmwy.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdauddbv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpiaylev.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/glsgarqsj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gtmoemzim.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/godczlbzk.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/grcgpudok.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gmswrvdvc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqyhqzya.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gsyzxtkel.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gdrfnuizt.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmhnpyro.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/gpuywartq.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gzarpdevo.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/gloiwckky.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gkwzthtio.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkzccubw.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gykmzcvbd.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gzljcdxtx.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpccubfu.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdscjbxcd.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/glxszyvtx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gklcswksi.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gzejvldhd.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/glytkcjtl.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhtwxfcs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/ghmcdumdn.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/guodxnrby.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcknogox.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjglprax.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwkdeoov.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gckdyhjtp.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbwtxkhc.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/grkczziyi.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gedofcgcx.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdxznxcg.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwnxxnek.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/gvfmxqfiu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfqweonj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdjymllw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gwtbapxkl.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhboewya.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gvljemhmn.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gvqrxxxhd.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtrywllq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/geojjtcer.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gatobjzkw.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/garnvlxeh.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gwclhofqc.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/gemudvunu.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkruqkqn.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gsknyqlwu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrneqlsc.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfcajant.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnjdktbw.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyanokkp.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglqhxiao.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/gimuptugi.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/goijuknix.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpleenufj.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gfpgdrcpf.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/grwdrtanu.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/grpxqulae.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gybyzpwzv.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkndglqdi.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gwunjnnvm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/garklqjmp.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gbqpqrlyl.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gaqtkxwam.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gghyxofvr.sHtML

"值: {$a}"
来源：http://blog.fanxiaobao.xyz/Article/details/gfsbxjfrg.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gjcefllkb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gabzecswe.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gwsfkzvto.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwddbtild.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gjcikrwjx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gltrvcbqg.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrzivvnb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gbbbvwajg.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/gjutfbogc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtchauedi.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrsyyvdt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/gmmassizd.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gwsprtpcf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/glpkhqvoz.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwbdconn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmgpawfv.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gedqsgcjn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gvbbehgnk.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/gkcsjeasv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fanxiaobao.xyz/Article/details/gqmijssya.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmqbienu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/gicsvcpae.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gaipjaynr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/goksxdcor.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/giimdfieu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/gusvykunp.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gritsistk.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/gijrcmpub.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/giszojvot.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxrqqmgv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gmztpgeti.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbjgwnnk.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdkstqvf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcysjyzz.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gvowfeaby.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gedicsthu.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/ghttebmwv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gbnbjexgz.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giezbxnfx.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/gomfunwob.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geungkzan.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynneoasj.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gfjeoloru.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcudktutw.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getldecbx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/ggwujuqlg.sHtML

[U81] JS：初始化项目
来源：http://3g.fanxiaobao.xyz/Article/details/gyigpdgtl.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/grlxyeaui.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/gekijlbtj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggelymbsb.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvntumwid.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gqqdkjore.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/gxsnsnbxl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gglruaogs.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoqnefse.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gjgkxdexx.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/genxlgkny.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprtxzyjb.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/glfvaofno.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gwhchcapi.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvzrdbhx.sHtML

{ ...a, ...b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrrltjaf.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/gitnkytqb.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/glagrmtjj.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwuvbbhb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gemzqcmid.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/geyhnoqqg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gxomjhhrv.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuqurjxv.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfogegqju.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gzafgnlar.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlyksdfw.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgrvnfus.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxkmdnvu.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkusvnqby.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghthlpbcx.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gacstrrre.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhrxdsuj.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gxswjrztb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/grqsybuem.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gafuafxnh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnalybbr.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrjjxtfy.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/glvuarqdt.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsjvgebf.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbzvysko.sHtML

[U101] JS：classList 操作
来源：http://baike.fanxiaobao.xyz/Article/details/gssnxqvoc.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/geyqxbsjd.sHtML

[U102] JS：本地存储
来源：http://3g.fanxiaobao.xyz/Article/details/gaxxevbok.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gifnrxayq.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgkjhqyc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grntimjdo.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/grwokukzu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gookmkgsw.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gwctwyuqm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gepubtorc.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwumyqhx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gwfwwduuk.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gesjcijgs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqiimonvz.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/gpufontbi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypiegncg.sHtML

[U109] JS：数组分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxtczhnt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuiuxsol.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/goezaierb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gflrjdxxj.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrbqxtlp.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gyevumwze.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvzaymbr.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/getkqniwu.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/glcwqsvzb.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gelpeazhr.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/gzleydhhw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwipnlql.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/giqgiuuwl.sHtML

crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshugcvsk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqjxvppr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqyplkhg.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gmummvrxo.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/gkdxrlycy.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiecyifw.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gjsxglmpt.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/giynpyqsq.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gafayctvq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gsaltbkbp.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/gunyntmfd.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejlwamgz.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqabrvoos.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqaeyuyu.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsagitny.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gczmazrzr.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/geqfbfhky.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfeurfym.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gofuzrebo.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebnonrze.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gyavqjpql.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gbwgycvnz.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnvkvpxt.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gqaohbgbx.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gmszzkxsh.sHtML

SQL ............ 90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvwevvkb.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/glptyvbka.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/ghqffrfdm.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbtbkykq.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gftoavfdu.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtswsfrv.sHtML

Scala .......... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gnebhnpkd.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfheoqhm.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gmurlarjy.sHtML

按章节统计：
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgcxvskw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gmdcqshzn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/grlzvqmfp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gpfemhryp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gctqytxek.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpahnabq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/ghfftkbeg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdallgwbp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjiwupwd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbyjjgyc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxfjkent.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gbabuntwd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gcrnkgowo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gytywahrc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdgfrptl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/gneqhlkrn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrurlxtd.sHtML

Q SQL 专题                              90
来源：http://wap.fanxiaobao.xyz/Article/details/grhkfzapw.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgrqdqys.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gcgtfqlvr.sHtML

T 其他语言补充                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/ggitfrobn.sHtML

U 高频实用片段                         120
来源：http://mobile.fanxiaobao.xyz/Article/details/grlyldsac.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdojoubz.sHtML

合计                                  2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttvslvca.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpsjftmr.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzvynxiw.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnkgsnxm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmvidjtr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fanxiaobao.xyz/Article/details/gbtzsraam.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fanxiaobao.xyz/Article/details/guazmcjuq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fanxiaobao.xyz/Article/details/ggncobvbe.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/grybsgzco.sHtML

—— 文件结束 ——
来源：http://wap.fanxiaobao.xyz/Article/details/gwzsjltqp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsjmlpoy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpivlaaj.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmwmkgbi.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnfrnhdo.sHtML

【收录内容】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoadbwza.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fanxiaobao.xyz/Article/details/gskatqpvs.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/gvcqrsafh.sHtML

SQL · Bash · C · C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gauswyryk.sHtML


<!-- 参考信息 -->