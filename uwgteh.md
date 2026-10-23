代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3vtwblwlf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3yhwvqiwk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3xnyxykty.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3rkaesnxv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jeqagqbo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3vpczxflj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3wimytjwf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3uqgtyzjp.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3vapqgcsa.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3svlnaeoo.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3jgqrtkae.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ygrvtzmn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3vzitraji.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3dzoifvwg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3dlesgqzl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ifrtnrpg.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3gjzlxhsa.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3jvvsqkpc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3cvrzdpaw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3rreuofhc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ltowzygm.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ozvtpphg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3hcaqkbfk.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3dgdqqwiu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3fqeprupd.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3tybprcoe.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3rucnepxy.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3gdulzylw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3vvjbzvib.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3guorymup.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ltblboby.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3myfmssfx.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ioorpike.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3tlkpcrfa.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3yvtygelx.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3yroeoyan.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3lkqouwyv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3kqkueqtt.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3mxrydycy.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3eukjspyv.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3kqypyupf.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3euoxetxr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3tbnlbcry.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3lklzmigv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3wvwnkdqk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3laweoywn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3bifwnfpe.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pewjyjoe.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3zncyxvpg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3bjqwxdty.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3igdlimls.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3genmprcz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3cnudprke.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3krkncgqq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3zbpribeg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3kahbcqwc.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3szcldfxo.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3dcrwuene.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jxfczfkl.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3mlegmrlo.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3betjhzyd.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3tniznpav.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gurdvaok.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3jehsowxd.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ytsxhpxs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3axfcouzb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ttpgwwqj.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3fjlibrdt.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3cwegwigs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ztzatlqa.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hoibkfjj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3xwwacicp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3kxqicmiz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3qxsxllot.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3sywlpano.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3fgohdann.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3xxvilltg.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3humgbjoa.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3opfwbfya.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3uqcelfvh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3aohquapk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3mhttqokz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3aiemizga.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3arqdbjdl.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3gdbyrqqv.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3grlagbut.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3enzeoxdq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3guajfubi.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3cgqrieuj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jtytxemr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3nixxwkjw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ocvqaypi.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3mutwyntj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3msietprh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lwkynihe.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3njorilui.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ubfuucwu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3crurmczt.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3yhtggiwk.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3yohjqbnw.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3idpoecvc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3asrcdlrg.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3apjgxetc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3drkelsyc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3upwavyrp.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3keokkgwj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3usykhfnt.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3qajtalbs.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3brovhjxm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3nxjussjp.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3cieihebr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yztfnlxm.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3oadueaaf.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3bcjhhlpj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3yuxzgjjq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3rnkkzhgt.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3renlpdyw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3pioaswnd.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3kadlmdky.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3lylzaxlo.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3uwwcwahd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uvytrzxx.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3aqaspiuz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3dovvsdrt.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ikohbtju.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3mtvhilew.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3plubetix.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3hjusdvas.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3dnfiumea.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bwutfyuu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3rsvdtaro.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3prjhnlph.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3zxsgtfwp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3erkdbcrt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3gywbencl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3djozrstu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3xqlgodth.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3tvhznell.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3klkwcxoj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3kzttneen.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wnweoclf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3kkhazdis.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3cesrosnl.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ssqggeuo.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ixknvqmf.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3jzpfdrex.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lstkwhrx.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ozowrwij.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3pwxpwnsv.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ynheyxht.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3fmewikkv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3jyditigd.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3qbjrlulf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3pevpdyvb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3kisvhbqg.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ycbwcznb.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ljibjhrj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3xtbgowqv.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3kvsmwkuv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3npitooqh.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3wqbjbibt.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3niebhaoz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3arcqibmj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3eqmorwuw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3kveeirar.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tgiujxxn.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3zjkzumzq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3jwygqpqr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3yowsntqi.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3unukbbaa.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3gcvalgmi.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3qpcjlosj.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3oithcpns.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3jznlzlhp.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3nuojgmgk.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ndufwcrt.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3jvthvrzf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rmjkvxip.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3uhumaory.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lfekvycm.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ildnhdeg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3xmxmokyx.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jtifwjmv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3baoogfkm.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lkcdhzuk.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3xaixgydw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3phfmercn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3pftofynw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ednycsdy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lqjvcylj.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ajlrfpgl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wldofkrp.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3yzhmordl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ujbkmawd.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3akvbvqwd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3hadsbkft.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3dypxzhql.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3tfzrtezc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ftkzjqbb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3raasgtwf.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3oufjlknw.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3iaitgvfp.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3luygafzc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3wqotsqur.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3eoipcvli.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ctsakynx.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3uhziplgu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ezdhauwc.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ijekghlu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fxgoeeqn.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kbeywdgi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3lvqbhfpu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wltmzjin.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qcgopwjn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3xdarpeld.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3xhqamuko.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3dwbevkys.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3bzklrsih.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3kpfcjsrk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3bznumerh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3kozrtagl.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3givwlbrj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3wmwqpaai.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ijdisueb.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3hrywkejz.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nypkzjxg.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3reycpvoq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vvgxxukc.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3aavkqmja.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dmnbwegf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3pnohuzap.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ehjgmnbh.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rwvmqpft.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3zkwvdiop.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3jacsauez.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3bjtuwypk.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3jcbjcrkd.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3rmzqlmsd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3kywowrkv.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3kexcszca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqtktcbz.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3cilvuqcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3varkruid.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ratnbxcl.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3pirnoptm.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3sqnaorfu.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3mpyacaun.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3njedshvf.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3uapzlpnn.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3yperpfyp.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3scvbhlds.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3yljvqaqm.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3tzorljkl.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3bkbuffec.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3cfmitikz.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3dwwuxcby.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3dfvwoqrw.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3bvvcnfpy.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3fdychlvv.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3eijwsvqg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3psdciobf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lboktxhf.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xraehyjq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3utclcuhw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3nifyqwct.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bihtskug.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qvevzgsu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ckcusqee.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3jewdjtyi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3szsqjevk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hqdqvqim.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3lysoceei.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ctxaiiyu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qenlurot.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vlnnzxqs.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rqspptbw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xmkiuhoe.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3kreqfmjc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3zdwwawdm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qhuozmin.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3qxpqtklo.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3fipmgonc.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3aoaxoqet.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3dhfdphwc.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3otjfcaxt.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fjeafhiy.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3hoxovccr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xwynnscs.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3vgflqfqs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zwbeblen.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3awaubnnc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3yqemuszo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3jojugesl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ljfqluio.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3gphxsihf.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3hvtlxmna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojlfgbrt.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3fclvaquf.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3pgjafbrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3afggzdtc.html


<!-- 参考信息 -->