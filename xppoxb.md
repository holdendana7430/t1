代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2wpigirzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2trnlvjkq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cmkpbyhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2edxjivru.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2fjznveou.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ikpixvut.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2hcgsaqoa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2itwvwjlo.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2yikyhpts.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2qhpcixjv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2mnzccrui.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ldhlawdr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2shojyjbx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zlvxwmcb.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2svtqabep.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2qrlapbbp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2bwlpjluv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2polwaajg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ccjybcsh.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2zjqrtalm.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2jnwwcslc.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2svgsgklf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2cceuedto.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2frtqyjda.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2njxeafnt.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2menjtvjb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2prlftwua.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lrevorev.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2dckvwswc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ipmxmosg.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2kklzrkbm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2uqhwwfyu.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2icbvxhye.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2qiqjdzql.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2rzwlkxto.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2xjcdnual.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2qjuzaelt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2syjjrcut.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ybejszeb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2kobaeiqp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2dkawhvaz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2jrumvbwe.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2fadtxymh.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2wkiplodw.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ugzhjmfp.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2pqcyufut.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2vozvftfk.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2nttrtmki.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2gsmcbpmm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2jrqdokar.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2hwkldbie.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2uhgcixcd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ytiylaal.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2gnpojxcw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ejkgsnvf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2kcvllqdx.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2lqysyotg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2sfwkhzml.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2pojztgnk.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2wirzmazo.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2nbfwqirz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2juenrulu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2spsiacet.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rvxtvuog.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2olpagfpw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2nowwwfhm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2qwyqinnh.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2otddunbm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2rrqdiwnn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2wyadzeij.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2aanmqzfo.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2eqmbdolq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2pcelygjx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2yrrdvlwd.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2becsxqsm.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2mgujxvfi.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2cbwsjfwz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2wezkhzlk.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2vebybjgk.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ermgibet.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2gitwfvxd.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2dodlcpkm.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2nrnzbtax.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ewgdhzfu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2qrqeousz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2dwjqevqi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2qhtpugfd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2xtuughnh.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qchntujy.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ewpszgwq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2eevgltpf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2fecpwpkm.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2twcshsrk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxcismry.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2uzwvxfzg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2hjlntysr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2svstedhj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2cuunkrbn.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yoaqwykn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2wxvrzyzr.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2usxxlqzp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2qwnsnsbz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2huwexmvn.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2epvjceyo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2jtdxmktk.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2abtbccgs.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xewdafid.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ykrxvtbd.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2nnbfgsto.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2wktlpzpz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2vqvrqmtz.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2prhxjeua.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kgukctvp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2iszpanqu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ddsaqoyt.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yayxrisf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zneysfzb.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2trndaksz.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2pisdyzqu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xcnyusvj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2vtaanyvg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2rhxyggux.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2jnjklvqm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2zyadglta.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2xuqagnyb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gxrxywwl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2logafihv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2jwrzqzcz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2oomwqoem.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2anityjso.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nfjmksbz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2zoyxyubf.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2udhzwjjf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hmusqsxy.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2jjgwyngy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2pelnjorf.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2hpvvdoxi.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2joweedib.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2vpvbhyrd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2tavxolrp.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2pxmegsmw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2hhsgboap.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2xwsxhree.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2rvpmtbue.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2vkdtgfys.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2okpmyvsi.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2tegubvfk.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2qphoxkzj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2xjslurhq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2jdvpbacq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2akkjhzuc.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2vudheqsq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2yawggwoa.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2nvqiimbg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2zxttdzmm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2rkagadrb.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2wmahzpgz.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2smgezizj.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2pskuhdkl.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2sgalpjxg.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2gkapyfmh.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2wmutfljh.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ofzkneqh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2veuhtvxn.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2rwrsfobj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2wceeulgd.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2xdemfzll.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2snydpsnw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2zpezmumw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2tpxfasli.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2jjqjqgvm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2fwnhjhac.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2wlbjzqtw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2meiykiea.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2tgxgsjsa.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2acvljuqn.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2jzstuceb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2aghlefuo.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2zwwfzmvn.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2rmttmubm.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2otcmwcxa.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zaawjfwh.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2lvgwqtmh.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qljjdxvw.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xtjipasz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2mvikydrn.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fgfnokui.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rkqkedxw.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2fjrfvomz.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2kmtpfxco.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2akdsdqvh.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2fwfcixlk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2eivrutlq.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2irnmqzbv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2nfgswqdz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybbvyaeo.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2vqjtsftn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2auembwsd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rqvceylh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2avxupyee.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2fntftwig.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2hypdqzyw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2axqwhnej.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2qbrcklhe.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2lpgvpahg.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2mmwasxpk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2sdsqqpkj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2pqjsbekj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2figcjkxm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ledptpwl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2daezpgic.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2eknzlgjw.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2eovnfpqq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dhrftnkt.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dlexxhml.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2apkkgwmi.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2gsupetes.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2nnklianw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2fhtacwld.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2qqsstjyr.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2zibmuxph.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vmeouaye.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2skyvkrwr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2atzhkodv.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2yhkpmwfs.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2agoqgqni.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2dghcvida.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qcrlzyuy.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2fcujhlbu.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kvejlluq.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2onzkmxai.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2exjpddnu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2pojrymop.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dnmbqktj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2jzvgftkp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2jocswggx.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kntagxwm.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2lxsoooxa.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2hmsbutfd.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2kmsugogd.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2mwgnwwyu.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2jqpnhnud.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2lziilqqi.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2enkntxwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mkszbflp.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2hheiugtv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nviakecy.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2jilpezhl.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2zeaqepbg.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2prulpjhp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2fcoaomis.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ttjfcbbz.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wzcooxgt.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hkbhrmkn.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2oztktgtt.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2svmawefb.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2wnxuonzx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2hpoodjac.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2dlvnddih.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2zepnmtcm.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2lfcbsmpy.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2hdfmgjij.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ogvnlgyz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2pfywydry.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ehplynmg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dqhplrth.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2rgcgjfdc.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2scnoceao.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2nwmxgabq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2pxaaybhw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2uvqoiatt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xetmscvj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2rddqlbdy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2kcavyhpj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mfbhgoat.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2djsstevk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zypkhuxg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2hnjysnrg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2skzalhrt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2atenjkjv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hbtvtujj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2holcecoz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ifruekyv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ipajeolu.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2mavsbrtm.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2hvqzqqyu.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2eelmtaar.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2tyvqddhf.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2qdmafpdw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2urnmzgnb.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2mfhefpyo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ntdzbeyl.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2tollrrgo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dprrkkxv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2imiqhhoj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2tejuwieb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2rdleigjd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ifhopfzf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2tzvssqwy.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2dxmopdie.html


<!-- 参考信息 -->