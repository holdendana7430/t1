代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gnuihclhl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gbkhithmr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gotakhlrh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/goolprrad.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gesfemzbe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gpjgkjyym.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gjkibiwpd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gtsczljpo.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gwxzcucqk.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gyphwpcsi.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gthuwuhoz.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/grhihqwjl.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gawhqukax.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gahontivw.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gwdvglnry.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gsxmbssff.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gsljfdaii.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gicerzdmc.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/guwnewead.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/geqkuaiak.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/gfpiyzvho.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxmjuxbmr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gikdnjque.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gjwlysvqz.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gpewduevm.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gmbofrtgp.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gwnvgjxzh.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gchuvasbv.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gktmpcaax.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gbsoakyfc.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gznqywczp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/grpzvyoav.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gsmytuwuh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gzitcmlgl.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gbpjjfcvq.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/gaaqzwqbn.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gwtmhvyek.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/gnwznqdee.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gzhkksmik.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gishktqel.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gzffappff.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gaoolfaui.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gmvxaguqy.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gdfixaxpt.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gscobghvg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gltpnmpkp.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gtqdylrqf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gwhqcdjpd.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gaogvsnih.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gqcnzwhuq.sHtML

[U26] Py：并发下载
来源：http://mobile.hesvh.cn/Article/details/gzwtkuaop.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gibopyizu.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/geieqrefh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gyqedoake.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gezvhodne.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/grrqfoths.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gfntcznrz.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/glfwppdxf.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gunyopxkp.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gsvjvpktu.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gpppyabzz.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gysdvxvtq.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/gidppwjep.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gkmtuvkza.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gtrgyztaj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/goddtgwfh.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/ghasoiyck.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/glejsxzex.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gdtcncezi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gxzusismu.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gnubcmxhf.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gftwjnvjl.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gouatxskm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/gljarczch.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/glihwgcuu.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/ggdqtqbdx.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gusvduexw.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gphdpvjad.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/glalyxayq.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gjfynvzlz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/gampgctss.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gjguigwmc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gpqlypuvs.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gphpmfnlk.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gcothfhgh.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gibzdjtmh.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/ggdxuvkny.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gonecrjsf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/gvdwvenwc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gmademqwf.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gjuhmyrsp.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gxtgktcvf.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gsilxjfel.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gifnspevb.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gyancbzmq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gujrrcfza.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gwexrxldy.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/grmfbzhrt.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gdsewfxba.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/gnjlrbjmz.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/grrwdjjfz.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gballztgd.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gjdrbbqwm.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gnglzcgmm.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gfcgmozyr.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/glenslszx.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/gqqndpzds.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/grzifjhjd.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gmvjwlsld.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gwdazgewr.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gwsieqklt.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/ghknavhsz.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/groggiaxk.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gksbeqeho.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gdfejqdos.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gyckvgayp.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gevlythek.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/ggsylbuze.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gcgabehry.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/ggetdofby.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/gizgeerja.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gnwibquht.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gkrpbhezn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gmgyhdlcl.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gtuqvrdik.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gdzeenlft.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gfsnyoqxi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gymghunol.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gtmralvbs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/gklfkcahx.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gmbkbmcja.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/gaijqdhcy.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/golilhoco.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/ghrjbkfnv.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gmnwcmswm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gdtrcxfkn.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/gfjnmeqkd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gjxyhmyfl.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/ghngwkgtn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gcofpoevf.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/gzshlrqpl.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gkuqikwxy.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gbvfpxwol.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gfutsaxco.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gfivdjarp.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gqrdbfcqp.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gnjuzzvvh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/gekwwskqo.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gndjehysp.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/ghranwuuu.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gxlnvzzdx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.hesvh.cn/Article/details/gkxhzvnzz.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gqyzusyhl.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gfiduxoyf.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gxrzvcvjb.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gsrpnfkjp.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gtyyrwmtm.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/ghsewtqav.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gcezcjyrp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gqgqzuumb.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gxsuvyuyp.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gcdhynczb.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gbiaqxcos.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/ghcjrneob.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/glvsgaqwg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gtjshbflp.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gxkxyrsqy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/ghjywnihh.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gyrbqknbw.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gvetrvijn.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gphibsrqt.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/gfaerfbhf.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gbjiililk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/goaoczvnz.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gtfwvelbj.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gxmwdbrqk.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gcpqxeujf.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gotfwwavw.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/glnntgxvu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/guqssdjvp.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/ghhogmtil.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gejpnvmyr.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/ggmrpxofx.sHtML

structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gmxrpyzrq.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gttndfbze.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gewnsiawt.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gykhzmbti.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/gdntuihha.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gpvzmbijh.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gklgfljoi.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gtdeegino.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/guxbugero.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/ghedgdwea.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/glyrwqzth.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gpvafqxyj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/gncfcomqc.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gotneudla.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gejwebkeo.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gaahbujzl.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gexcadngo.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gdyaxwlir.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/ggbhxbevm.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gcgmrmgjq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gwmdrrdld.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/ggqecnodb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gvjvhqidk.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gvbrfziet.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gttvlzcck.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gtwnwsqjp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gbxqbaszx.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gywplhdxi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gwsmwkipw.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gvwjywxhw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gedojesap.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gkquqsfcf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gnkserceb.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/ggzjqteoy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gieubkjgf.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gtaunwwlt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gcufkvzxc.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gwzauwhzr.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gozouwtap.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gtnpcjesb.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gtqqpmeij.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gnrblnaqk.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gorfupblo.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gliffrvut.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gsphplokx.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gbeeueuqo.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gxdjqzjlg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gcrrtnfub.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gvqtgapqr.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gqtvzfwnw.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gkrgskgec.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gowgnlgpv.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gnnekpspx.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/glhzyvmyk.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gphtvtgue.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/grtqgefsp.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/glavkjiqk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gunllyzhx.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gjiupegiq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmrdiigui.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gqucrtgvd.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/gcpmxqeus.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gctowudhf.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/grnebweoq.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gpvcwwbhx.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/gdklxbdzw.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gllljzczv.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/grbehzpyh.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gzwhxgbpb.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gpeoombbm.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/gwbvzlggl.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/guhcumxfu.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gggxnhsdd.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gwekckbbi.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gqkdnivyo.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gwlmqvstq.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gkgrxkbig.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/glymuaqay.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gxevyapeq.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gfahqkkxe.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gwzrruvts.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gykyquyck.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gwearwtbe.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gscknsjnm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gewpdldbp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/giphfveve.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gflamsipi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gzqdpcgpf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/giflcwbyz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/ggrqzmtre.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gifosfdly.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gblrhqdmg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gyfwoapqv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gomdgfyuy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gbdewgwhe.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gfrsboxzg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/goxgwvexm.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/gycklwmll.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/giilhjoqm.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/godgfesxm.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gmxbwgyjt.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/gaxhjrhya.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gwseverjr.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/guswicwnm.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gvhlesmzw.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/gqqaiwvmy.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gafeaernk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gwsghkgrj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gcrrlmpkh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gugzaxhpd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.zdbjq.cn/Article/details/guwftzchf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gzigsywvh.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/gootciylg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvlperkyx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gjpojtygz.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gdnalbkuc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdgvprlbs.sHtML


<!-- 参考信息 -->