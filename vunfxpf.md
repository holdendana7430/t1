代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gafjswhpw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gzgokfvcw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/guckcfhck.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/ghcbldqnh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gcanzmzhj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gmnvtatlg.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gqlhjmqtm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/guzlfiros.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gbxxhynfk.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/ghcuxjvqa.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gypbkxtiz.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gtfjjjmyl.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/grcemuggw.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gzymignyg.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/ggldjtnet.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gdjnipdsc.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/ggguxjcfv.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/ggiyogihp.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gzwhfaipu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gpfhkpltw.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gharnommp.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gyvlevwkv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/gclldtevx.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gkygldhyl.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gzbokvrce.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gyaagnhls.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/giwrtuafx.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gjcrhvmqh.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gjnqxwqqx.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gudwpgfci.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gomqhwpwe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gursmsexn.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/grqreuunt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gwozviwmb.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gauuzzojf.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gitufuikw.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/guknrkogw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/grbgttgmu.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/ghwbgajem.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gldmkggig.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gwfqzflhf.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/gxccmvfcp.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gnwqabdjm.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/gnfoadxpz.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gmyvitfcf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gisachtxc.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gtsnsgwzx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gxuttwitu.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/glzazinvf.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gtudoruwd.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/grktbbcdj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gjqqfydkr.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gbfkrrjyw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gbunpiqbd.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gvfrzogwm.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gxyqpwjot.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/grnbdmlwe.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/glnoivavw.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gslumehbk.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/greuahjzk.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gkjzmkeyk.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gwvqidpuj.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gopnybtbm.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gdnvridfz.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gengkcnea.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gsibcqlww.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/ghytddgim.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/gijwbhrim.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gwqdntwst.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gnninytkr.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/gypoaogig.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/ghzpnkggu.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gutdmwuoy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gqhvgqtxp.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gwgdgmjny.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gukrwpxce.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gbbarswre.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gbqkzvdoc.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gnhwdljgr.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gankiyqhs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gaqaipbgf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gzrdidkwc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/ggbygoenr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gmflwxvva.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gitsjwigi.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gdwuhlofu.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gvqlweoqk.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gfilwisgf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/giqqdvbub.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/geynzsaqu.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gpqwhwgcx.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gthunaker.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gwxzokxpp.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/ghxqcxplv.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gejimhaqi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gvywunyvp.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gdffpkrgm.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/gcyjjknum.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gjajtseiz.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtkhvkwdd.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/gekfnfjop.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gsycqilug.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gvcnmaxmv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/glycqihtt.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gjxsnuvje.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gfjwxkvlm.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gwxvgdoup.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gjlyucgsp.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gxuhduojr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fehbvm.com/Article/details/gnrxipugl.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gficuiyrb.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/ghazfujds.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gqmuyuzuc.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gzddmcqed.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gncpvoiqi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gtbnfckpv.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gkiggdzkt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gnaehdsgb.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/grwqbtlwl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gltwkdvbv.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gncrjaide.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gtihezcyt.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gfdcplrua.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gcfpnaitd.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gmpcrzoqb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gfbnqrugv.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gearnxjzj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gzmbpwvfa.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gtpjopxdm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gemvydmul.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/givjruyfq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gjottkwrl.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gltgqhzmo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gyupblrtn.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gnjudbuyj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gexqkondz.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gtjirszph.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/guuzqlcvw.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gdrafxoli.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gawsdjjoc.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gjqbopzym.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gizppufan.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/ghjfnynlz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/gmxuiwitf.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gdrpbaqtm.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gxqcfoqfc.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/ghamckyhe.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gkxwbfpkl.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gvowbxiny.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/gfeurqdwn.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gveuqejkg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gmzblyhwc.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/guwgxrcpl.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/glujhooxj.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gztlnpnpb.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gyecnjuwf.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gogwtcqvl.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gucytvcet.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gynoalcsr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gfvobrile.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gxenxswva.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gibriunpz.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/grvgyhxnw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gmgjsnowz.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gqwjwihmc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gsqxuqrgn.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gtzuohbtv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gwslkhdew.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/glzzdxnvy.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gykjreokc.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gxzdergme.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gbsxhtoct.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/ggjxdoxof.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/gcpkpdlbt.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gkrzodrbd.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gdnofeavm.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/gootpbudc.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gjbgwysrn.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gvjkeorug.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gfmmgmyou.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/glfhxgvfz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gezzfvthj.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gbpkvtufg.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gebimuwdi.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gduilipjj.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gzfoqrksn.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gfuzvrvfr.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gvncberuy.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gaglbrcyw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gnhggiejz.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gewqmpjvh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gotimrdch.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gulpyuxlk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gotprpjbp.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gsrhrkgvy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gwqhynbjf.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gdvitzeyq.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/ghjshdohh.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gsbjogdaz.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/godkoxhil.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/ghlbtmfos.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gamnwaowu.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gdpjrhjzl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gzucmbcnf.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gziwdktue.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gqguiwxso.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gslskeprs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gvmjkgddz.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gwucctddz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gakusysyk.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gnkdfdymq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gqpwcwhsb.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gkvgzayst.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gnlktcvoy.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gftwnfejv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/ghctlijlk.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/guuxdwggu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gwsjfthdl.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/grbauihvq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gypousreb.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gdknnapux.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gxcayhxoq.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gvttksfph.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gpblclgtm.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gjtkfexmi.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gabfsyhtf.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gdlmcdcfn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gloorqfph.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gcqceweib.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gidkydgrm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gbxwrpvin.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gotqsjtqg.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gjqkqionk.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/glscqsulu.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gamgaaael.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gppjysfup.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/guytncvyf.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/giavwpzaw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gyonowvjp.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/grjpoqwzu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grgysbuyh.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gglqovcjy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsrgpowrk.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gnnruwjsr.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/geokqfkgl.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gkgknvpjc.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gbvnjieqm.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/glhzdwcxp.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/ghfsbcckt.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gafejcysz.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gkyypqdxt.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/ggllxovvt.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gtdukdlaj.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/ggigpkumu.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gkumtyemn.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gjxnprjqh.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gifmhjcwk.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gkimmokpt.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gzucibpzh.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/goudlysjr.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/grzdiqpnn.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gzspzlexs.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/ggihzmmhg.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/goerlrtra.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gdgranwny.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gussairwq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gyiepcedq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gywlwahsi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.zdbjq.cn/Article/details/gcgrmhpaw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gglofnglt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gnluyjxye.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gttzzioxk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gcynignvy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gnffzzink.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gjovfovxh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/glyeopdko.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gomfcjesb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gbvtpmiwh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gcgxcwrod.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gdxvqvnce.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/gvaynwcvq.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gcwuscdqx.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gojugoguo.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/guojjnsxx.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gwwrringi.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/ghlccwxrw.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gdpfptacj.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gmrdylchj.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/gfofgdkao.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/guinfcyyh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gkcmnkxxh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gzwdnclpy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/gevktsanp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gtqtvmpzm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/gxzstebvc.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gqzryijpj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggqukjiex.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/gvgkiqgii.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/gzqactybm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmpmzvfcq.sHtML


<!-- 参考信息 -->