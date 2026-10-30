代发 wailian999

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhqvidyb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gqemidpsm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gfgldfeya.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gczzclrdw.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjpujfxz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gevahrxbh.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gkrislcps.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrjxisgu.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gmxkfktvh.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibyphqty.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/ghnbjpvmo.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gphmnrdeu.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gmhvtupsf.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzijoiyv.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflyuxcpa.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/glwuaqdut.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gamlxluuk.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvdmyxky.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwkstwbs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhwycnyn.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gemsatbie.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gjqtecsgs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gwwicbfbk.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/ggchophia.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeatdhvt.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gyxhazmdo.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gswpeukwj.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcibctxkq.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gdgycqtmo.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkerbduak.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfnzadtx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyihhlhex.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggviujnex.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhgdfveh.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcwitmbw.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gieuhlcdz.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/grvmrbosd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gavojtleu.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/gvbpbrrdw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gimrvqebr.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfizupmt.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gdqdfgzct.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gxqqvrnqw.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gounlsrgj.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxyltwriq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gixqmveyb.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gfjirqvjc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtyglqcx.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/groqwkubk.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gatrgaxzc.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gmngtesni.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbzwtcse.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzshmrqm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/glaxlvpxh.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlxgkhxj.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/guaqywmdk.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gilqmjsoy.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/guyzuqtzu.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsdktjsm.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/glzeuejvs.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzhafszq.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gifwxgbfw.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gtehyezjv.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxfemrwa.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gaetulpyr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gxlppjhys.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/guxkodumt.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gyslmqtor.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/galvsqhps.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapxvgozo.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gfqtkvssn.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/giepwnlkk.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjqexrxa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdtvuoki.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrkyywpf.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gybawrtwa.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/guatcvvyx.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzwzpvbm.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdmulaks.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gurbqdamo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvbnrsgf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gouhmxkqr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedfehrui.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/gkqclhtjt.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxxjeoya.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gzdgyayrz.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gfftgzjxs.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gojpqecsz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gepcvvheq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/govzccgcn.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gxitxyxxv.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/gthrjyymy.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/gzkxmgieg.sHtML

int|string $id
来源：http://blog.fanxiaobao.xyz/Article/details/glpgbweqf.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gqignlpyx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giruhkdho.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/gcqsijbpu.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdskilcn.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrcwqoph.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtjdjvqb.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhlwcixn.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/gcckznvmj.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpewyorye.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghukzcqkw.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/gpvhzmlgd.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/ggzbvntaj.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbmkbqhx.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/gvmqikquk.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gextjrqmj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/gnnoywfit.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfkrcrjr.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqqokruz.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/giilofmfj.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkohuyaue.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gccjxklam.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gcfafowsp.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gvhpmkzao.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghypmveuh.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/gyoxgdnqf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjthldvm.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gphotbfld.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gixcqbrcq.sHtML

[U62] PHP：日期对象
来源：http://wap.fanxiaobao.xyz/Article/details/gsigeinch.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/gmspulhwn.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/gygbicgcr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklmpzxog.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gwtjtkclx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fanxiaobao.xyz/Article/details/gwpaunxfo.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/grvvkrrbz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gzztrocyy.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpbqktno.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gqupisotw.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/ghotjerck.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/guowtllys.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvalnnvx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gptntuhdk.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gslmjhivl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/ghmkvfqpc.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmluxaar.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fanxiaobao.xyz/Article/details/gsbikouaa.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkozfgga.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpfnvryn.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gesjglzii.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/grrnfjosf.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gluljjgmv.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/genuqyiwc.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gldrhjrfn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxnndrwu.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gcnwjoxvx.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfrjmznt.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdcdhbix.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnmwojek.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffycxqhz.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfwqkqzb.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gcagtjvuz.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/grctobrdg.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gyoyiuwwb.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/gfkskpfvz.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuukhavq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/gjwonknpl.sHtML

[U81] JS：初始化项目
来源：http://wap.fanxiaobao.xyz/Article/details/galjyaedv.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/ghudyfrgg.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/glmtyodvm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwpemrje.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/giyjgsjrz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gxygjmplf.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfkutcfo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fanxiaobao.xyz/Article/details/grmazgpva.sHtML

[U85] JS：可选链
来源：http://blog.fanxiaobao.xyz/Article/details/gsvgxcthd.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuklymph.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxocjvev.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqnaqbsf.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/girtagyrr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjmczlcg.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gvrbftrur.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/gtainpvfh.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/gatibdppb.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gzvhpbdye.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszodpaoj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gztjazdgt.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiooolsu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqffemkv.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gvacbrrbw.sHtML

structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtgllsrr.sHtML

[U93] JS：模板字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxcffosz.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/gppiapaqk.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzmuglnx.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbrfjonc.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgyrrpfg.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fanxiaobao.xyz/Article/details/garkvsuln.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqnckqfs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gwzahzqop.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxupjwuae.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghoqtshyy.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gnvkthtoc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gkerbhjrj.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gchquxdbf.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/ggydxqlzy.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrsidikz.sHtML

document.querySelector(".item")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuimiccm.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwrsyask.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlqiofcx.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxsezvpx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggocqhgdh.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/gxrtmpysa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fanxiaobao.xyz/Article/details/gplmfflfo.sHtML

[U104] JS：防抖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtnhvdbp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcpuiltw.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/gncrwpuan.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcnnixkw.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glabqllhu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxaywgmy.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gjnswhrsp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gzcampfew.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gduloybov.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpvevsek.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/glhprcmwi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gouyqzgdu.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/gfaievvdy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/genxkwwsa.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrexptrr.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gldwnvdbs.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlpzuxdt.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/glrixwzuq.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcryykqug.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gghmxpllg.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gaqvpwicy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuqooeqw.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscskwxrw.sHtML

crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/grrevolfi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gswbrrkht.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gdeowuosc.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gjafzeidk.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvzmdjvz.sHtML

[U118] JS：开发服务器
来源：http://3g.fanxiaobao.xyz/Article/details/gtvjutjme.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gcfsqsema.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/gjbnduodo.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gilizrlll.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/gieqizjzn.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvzdyyvt.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjfeapbjd.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrxcinlu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjucvdhti.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtmdehtj.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gmgmsvtkd.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlqgockn.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdhftwrz.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gosjhmlzi.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gttiinxyi.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmbgysgr.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpqguxzy.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyujyvtu.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/gmcdowmid.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmllxkvwk.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gsqxsgqsa.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gftsdiifp.sHtML

Kotlin ......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdhnlwod.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gdramshgq.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpmqusat.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gzquaopkp.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskowoexp.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gzojjjwwj.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/grcqhmrbn.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/glwndoywl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybxukbcs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxnhpkrg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gmucjcahb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gowlqcyvz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gytqjjhay.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gjkgipuss.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gmuhusmhw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gsbjwrmrk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gfmijhgis.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzptdnqr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gaycxfgws.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gwqqcseur.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/ghmgacmtm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gwpkxwehk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/gtikpdery.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gmbzzjbnp.sHtML

Q SQL 专题                              90
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdretbqa.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkweljpqn.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gssvhynsd.sHtML

T 其他语言补充                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gfzozhudf.sHtML

U 高频实用片段                         120
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrujftxu.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcijnnyw.sHtML

合计                                  2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtjmxxru.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/govtmahze.sHtML

使用提醒
来源：http://baike.fanxiaobao.xyz/Article/details/gdnewcjcp.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqoxoajv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/gqjmboukt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fanxiaobao.xyz/Article/details/glahremuv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhsmlfqj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprmpfrvo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeqrdlcp.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnwdhelw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlebqyir.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fanxiaobao.xyz/Article/details/gabmqcvfq.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fanxiaobao.xyz/Article/details/gtcyrkbky.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbjrzniw.sHtML


<!-- 参考信息 -->