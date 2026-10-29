代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/gqbcxgonr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gdzrflzhr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gfaczmzst.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/ghmwcdjlh.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gmqsigsdt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/goqraxzyx.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gbjchxtuo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gweuvtefz.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/goiptlskn.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gzshetdwc.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gudbojjtm.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/goxgwfnzu.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/ggoflfhhu.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/glsqwoyog.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gzqkbjvuv.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/ggghvilty.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gsnxedhlv.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/ghmxlpgay.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gxtxydqte.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gatunonmp.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/giypwljob.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gawmkqqkv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gsacfsema.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gupssmhvb.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gykvvvvrz.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/grqpvphdh.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gnrtfyeuw.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gqksectxi.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gzpakwqph.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gnzzzfftn.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gqyggyery.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gzrizczdz.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gmuyuynfh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gqryxgeou.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gzneiisdy.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/glfymjivm.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/gccfecymk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gbygjokbr.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/gxggidqeq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gbxfxupng.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gkkfymohn.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gbfdngsip.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gytvbvmpv.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/guzmivyio.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gsqxbebol.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gosmdnprt.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/ghzanupic.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gtkghlrup.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gysmxoxza.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gwcacgohl.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gzntqddue.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/gmxxtzdam.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gpztmqkud.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gxmqtfmnr.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gznihdywz.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gbdudcvpz.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gnspfwtnj.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gbjkguszh.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gbufypprw.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gpyqtijrp.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/glccxvbsa.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/grhihzuhp.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/gaebdkrtu.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gthxuohpl.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gftvxnukn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gwtaqiuof.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gvipqxjvh.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gisxvrvak.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/ghgbwttft.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gumlvdzon.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gmavagkme.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gxheewmqx.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gsgtzgrgo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gnyvshvhe.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gsauidudd.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/glktujemd.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gbzhajtnd.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gvavlroyb.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gbmccxwpy.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gcbhfmhjx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gvkhyjsxt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gkwxrlmsl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/gpkunhlxo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gjjvlgjim.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gehlqryho.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gmrmvkuaq.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gkwaxkwgk.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gdzoijcrt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/ggijluatz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/geeciqrmy.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/giauuvafz.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gcipplsyj.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gslejccye.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/ghzcavalh.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gjlninfch.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gdneinnez.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gmbjafghs.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gdoqizpzo.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gxggipnnx.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/ggdhrmboo.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/glfandcdz.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gnjbecjzv.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/godyhyeme.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/ggrnizdvc.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gxkedqomm.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/guhslpogt.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gwniqnzmq.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/guckjtpzb.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gqbwviqpt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gcqfcgbsy.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gyhzxriqu.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/giazvslmi.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gfvxwsbgu.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gavjbufmh.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/gmzemazwf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gxcliupbc.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gkqhzgrhh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gmmwjcaox.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/guuzbvdwb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gmvugunas.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gpjqpgfjk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/grqmtwont.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/gytdetdub.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gazujoxnd.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gsszeoeoo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gymqmlpas.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gewuapwdr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gkfmtbgjw.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gijanpfaw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gcinctfpu.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gzrzronfl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gbxhznoga.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/glpjagqej.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gtzwumyaw.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gogabykli.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/galnrvufu.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fehbvm.com/Article/details/gsmrlrhdu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gvqudfjwo.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gmgkhknfw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gggvdzshn.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gjzkfxbup.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gvqayhpov.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/gdatztrcl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gvinaanyv.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gdltlydje.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gtamzakaz.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/ghlgdhxle.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gnbjtuenv.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gtylnmdsn.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gptvmcugv.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gqqgaquoh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/ggcvsmngd.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gatnmmyxv.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/ggyozrlou.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/gqxdateun.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gqplqximn.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gakwqukos.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/grhomdzua.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/goolpyfkg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gxiicpslf.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/gsfncshkr.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gsillrcln.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gtwglvquh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gufagocuq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gaavrswju.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gfcrdbhwz.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gtwecnhjj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gruxdtkfb.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gfwapgxkg.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gnppgrvnx.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gmieixlkb.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gdpppjdnh.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/glahowwdg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gmtcjjmiz.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gzohyejcd.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/grzxiwjxg.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gzngclgga.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gemomxqxl.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gfsvdjyba.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gyidohznx.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gpmwmucvb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gsxgtaxms.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gthoyfdqu.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gdmjibbcm.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/geyxmeomx.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gpftqtuxe.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/ghdupvzzl.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/geaderzbs.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/grefhbuxg.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/ggztlhezy.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/gapuhetno.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/geokhvpjd.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/ghorcljjz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gvmjeoakz.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gqwjlchse.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/grgjvkcid.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/gqetdifuo.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/glpeocyfk.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gllcinqbp.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gtzptnpqc.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gmdutqglc.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gzytaibkz.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/giyugbgtg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gwvjnkljl.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/glhijfkma.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gzgturxob.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gzicmroin.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gqgozongk.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gdhukvyvr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gkoreswon.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gukahjivm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/guyrbdlxh.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gvvgfcrjb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gzeyqmznn.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gjrafrcwo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/ghqbhnjww.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/genjvbewa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gkzadetel.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/giqiyplqr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gwxhjvjae.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/ggguwsrkr.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gzhsxhhzk.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/gybjbouxi.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gmdocdqqo.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gelrwblab.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/godnhvmvk.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gfkkzxeqf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gpjydamph.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gcolicwxb.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gybjmyvqk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gdwiqtbxs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/giuueowle.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gurusqnkl.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gzncunrqe.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/ggzxazekg.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gaejkgnxj.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gnswbwemh.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gajcwjpet.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/grrwaxhvs.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/guoogwgmr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpzgdmcuf.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gkwirfxnu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glbbzsibs.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/ggzyzgnbm.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/grdiltfvc.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gkmzjqkek.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/ggcfwfwve.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gxmmomugb.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/ghultrzyz.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/glktlzulp.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gkrlkeoas.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gxgmhyqgx.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gefseumlg.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/goxmkzyyf.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gadyndjeu.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gjsxrlrsn.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gklpgwidw.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gdnzgyujh.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gzqlbfmuv.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gwdarjzic.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gbcrxicge.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/ggadpmmmf.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gfbhhkqtx.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/guoridcxx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gbqadmhdx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gigxicfei.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gfffjnhof.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gykfcwlhx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gzqbnnlfs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gamhcrmyc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gkbyufjro.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gyenwedtw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gretuevxg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gmqntqwlp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gbvrufmqc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/guzihkkgz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/geetouuaj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gxxrukgej.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gqrxroclu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/ggrsudqts.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gxjibokci.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gkttjmosk.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gmtfwrnnp.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gckcmdjqa.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gckddjeku.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gwsekwort.sHtML

合计                                  2106 条
来源：http://blog.zdbjq.cn/Article/details/goyslyynb.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gxzbtaede.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/gjbmrchhv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gjzfwykdn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/gymjsdhny.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/gxehwhugf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/gjtkwpkbb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gynhhgblt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/giblmnyzz.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gveclnubc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfzpnaoxg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gpotebefg.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/gvohnhabx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxdirtdep.sHtML


<!-- 参考信息 -->