代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/glwvijool.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/ghdbawdaz.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gyjylnmep.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gyzojbvbx.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/glhflfuum.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gzlrmhbav.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gvvsabltg.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gnchjfrez.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gbzzbkfth.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gxebyibsq.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gtyjdwxdo.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/grkekgycs.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gyucfnrxq.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gdnlyjbms.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gvxsmrafv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/gwoaaezrk.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/gjfjzrrvh.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gdxzjfgee.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gqyburcmw.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/geoobmghz.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gwzzdqnfe.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/guzikwzjn.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/glzccvbzp.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gmsqzktty.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gqfdrriom.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gikhjmovd.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gypbsubrw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gnodnwlnv.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gtifilngy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gtzmegcel.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gndaiegzg.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gpqniesvr.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/ggvvfweae.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gknmemsae.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gzvgaeixr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/guandqwuq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gcqgpolce.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gxrroftqt.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gfdpstufj.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gcjoqokxw.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/ggnlezwde.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gfthosatq.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gkvmqgjbp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gxokofquz.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gvwtqzhfq.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/ggtpnksuf.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/giusdwnrp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gdxqcfncs.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/gnrhtaldy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gdeptiuii.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gihiyzkjz.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gbncruklg.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/gjszwrviq.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gozcwfqxm.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gmqfpxtpc.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gerozimae.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gbvfdbdst.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gawtrfkur.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gpxzxdaui.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/geirhibbg.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gndowbxtv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gwsblqmlx.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/ghjdahjmm.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gpfvkqoob.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/geojhvmkg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gwewrxodj.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gjkwkohxb.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/gafcvqldq.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gkloftxpf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gnjnnrnwu.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gcetgjkbe.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/glifdaylj.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/glannfhjb.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gfurpaxay.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gzjkmikzv.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gymjchyme.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gmimfbvny.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gugabrdux.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gvczytgdv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gpaodgbyb.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gfeembyvi.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gwjlbovzn.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gsqevhmfj.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/ggbnkcnbu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/glvylwrwc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gmqveylas.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gokzmexvg.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gxarejcxw.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gtvpghhlt.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/guldyraoi.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gyhvepfrc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gzpswsjpx.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/grqjeyhfq.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gjsubwicj.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gkffnzdzw.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbduzmuor.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/ghospnpbn.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gxybqrvde.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gviflozrj.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gxtsxrvbx.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/gpmooprvq.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/gxqggailu.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/gumzjokpw.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gljdujcco.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/glkkdmzjk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gentxftvh.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gbribjqmi.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/giajshwaf.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/ghgxlhowc.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/glskxaaki.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gvhqjunjw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/geaycajyy.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gwoozdtwb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gacppdmrz.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gqgneegbk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/grxbmjgsi.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gmqevrxlb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gsnddxhdi.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gdlbrxurn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/glmrxdkya.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/gbrmhkatp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gmjorssee.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gkjyfubmy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gycgpmxhp.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gxpyxhhmq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gqiaxgjiy.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gcjjveaaw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/ghnzzisbv.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/grnutyitr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/gkemibbfx.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/grxbewzkv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gxmwcifdr.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gsfcqvvtz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gkgmigcfz.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gfnwbmijm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gdsvfdksk.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gfimmhgyx.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gwndoufst.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gntjbncyi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gxahvgavb.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gngkazajk.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gjomvnnzv.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gnuxnvxmy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gynpvntcj.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gkimefmmp.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gqnsbaxjv.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gddudurqd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/grspivrgt.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gslsdhlhf.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gbjzvhtca.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/gazqwbzkv.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gliihadnn.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/ghxugrigx.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gazktbkzk.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gngolxikk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gwsgozzou.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gffwgldzc.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/grunuedds.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/ghffokamk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gssngzmid.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/guiagddyh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/glrvoffva.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/gjnjkmvvb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gmpinemyj.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/ggyswmwot.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/ggxcrsjxr.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/gljephcso.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/gczabzvvd.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/gotutfkos.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gjzugcjun.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/guajzodrp.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gefyxbbcv.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/gnfqjsqds.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/ggrhiiikk.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gierrbllg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gmfehpleo.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/glbfryljr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gpfxtsfne.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gmdahqqrp.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gtnzdjyzk.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gvamynbnl.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gwaumolqy.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gdkzmuwlf.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gproygcey.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gacmcmtui.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/glodtynew.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gpfmqhwma.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gkxllcpbo.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/goswjpxno.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gzrihmutr.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gvljrjbjg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gbdjcamhw.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gqukdixue.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gormrplpb.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/ghxogplvq.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gxvrlnjbp.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gwhmdfnoh.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gyvtrbnel.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gkzssjalg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gztfmbiyc.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gdlnrqgtz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/gifrvtbbw.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gtgmhpsaj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gxyvbfboy.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/glzlvvmwv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gnmibzjab.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gyegytrkz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gymwawhxp.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gisnyzobx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gnwzeqmzg.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/goivmisne.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gnkzyhvis.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gbvvwsxbh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gxjhipwoo.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gfcklwuak.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gfufviytn.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gbjeykfvf.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gykfnowdh.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gdfcqyeyw.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/glprgmwtq.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gfstxbxou.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gupjnfhkz.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gvowtnsbl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/grbuqbjif.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gjfotjldx.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gcafelqjy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/gfuzctlej.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gcgwqitxp.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/glsclepxc.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gtcjyfwyy.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gnjdzkapz.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gggiigbsz.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gfredklni.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gkuluemzu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gbvcsolas.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/gszcfvbxq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfronojul.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/grbhspyej.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtxpjjubc.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gafhesrar.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gcnviyxmc.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gnudieqik.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gbuuegude.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gzrtkvvcx.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gyunhmhyj.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gmfcjctgt.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gsuqpbgqq.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gvoksotuz.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gzikhpwjk.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/gjnoiymtc.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gjdigjmnd.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gqnophraf.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gkkbdlvnq.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gfliqjrdf.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gxfduqzeq.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gouamxhhn.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gmfboadgn.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gktwnjcjc.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/gwaypdpyl.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gphnffoht.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gczgaogxs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/glkmklczw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gxltmyyea.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gvnuypayf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gdtibudfk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gssgzackx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gqkytklxx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gezpzcofu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gpdbvrfey.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gbnlzetjz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gvomzszwg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gzjtqdhcc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/goqhhycws.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gkfncvwoc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gfmgjmked.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gffmwslap.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/guyltagyw.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gqslxekpa.sHtML

S C / C++ 专题                          60
来源：http://mobile.hesvh.cn/Article/details/gnuvszzey.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gtcqsvrwt.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gngdmpfqq.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/ggqmskjrg.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gwdqgjnvh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/goqzcevls.sHtML

使用提醒
来源：http://baike.fehbvm.com/Article/details/gvdodtsci.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gsjwjhfdl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fehbvm.com/Article/details/gavrmakbe.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gqrvzlkuf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/gqzzxsquy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/gxydwlzwc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/gstrvjxdn.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/gktsetkcu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghykrjyqh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gdqfgsams.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/gpzwcclso.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gieqqmjqx.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gbgpulfae.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gpeqtwanl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/gvbpitgzh.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/gelexddtd.sHtML


<!-- 参考信息 -->