代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlzruofp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gugezwahc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gosqdzwdz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfcuzbfx.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwruyxukv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/goofnbljz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwvasygj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqiedhnht.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gzqlkspfb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gtpzclavb.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwzfetbh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gskboefgq.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkgtnnbk.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gbipceism.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdjrocbb.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gnwpedofi.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpsocytb.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhxwgtks.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkutkjph.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtanhxbo.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gojrxtqlx.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/galxanxri.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gliudgeqc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/ggjsvmxag.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gfgykuiyt.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/guxngqbnm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guysfreyi.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmioqeum.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihzowuxm.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcltkpgol.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gupsabofd.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gahsexbet.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjgzxprj.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gnbkonmix.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/gaigddguk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gutxyoqng.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gvnmhzfev.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gsqnzytyr.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcvrjery.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gyjhkyycu.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gykghpgwq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqurxdfsz.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gozsdiaad.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gqwueebab.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gjjjxiqlg.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gctfdvrvo.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaessyzm.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpayzbpx.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdkujfzhc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gtktydacs.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gcidwwzfr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gewldjflc.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccamocxr.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/glihjwtqf.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/goqmuvzlo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxttfzcmu.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpvzszmc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gqwqlrqui.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/grcwihtcd.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gfovukqqr.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gqvbjxtjy.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/ghweqhgve.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gzuuoujnf.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gqgalahbf.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gnixhmygn.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/grzjrxvon.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbdrtikt.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmiquauj.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/gnxepqint.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gyytsqdwr.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gyehettfy.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gqirsggnh.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnarqiff.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmklzlopa.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsfzupaf.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmqeszkq.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/grorelohp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/geodoabjh.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/ghbrjjtfm.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gdngeyzfm.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gushcxcsn.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyggbqwk.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gwetgtmkh.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdugcsfgd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gwfyycfmk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdlnddyb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/gfkozzvwl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsydncep.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/glrszknss.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gcpywhgqu.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/gqvhrrbzs.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/gijrdwolo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gdmosfyma.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgmlaixl.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gcbsyamlb.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqggjweh.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/gjonsdyrm.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnqsrfnm.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gangnqfkf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfccyszbe.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbsatvae.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljycxatr.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/glfbjkggd.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gqegqbelt.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/glpaoeseg.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/grmhpfsxy.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gldkbvjep.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzxmtdas.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjzkajcp.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlmdjglx.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gprnobkua.sHtML

$obj?->method()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvraxieok.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gbdzcresq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdunlptsm.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gcuxjbndw.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzoztjen.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gfvuaddhz.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvwmbrqz.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwrbtgli.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/ganzhjehy.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gkflbzfjp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejkrnomh.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzufrqgoh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbvwsllo.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gmzswpmio.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvclskrje.sHtML

[U62] PHP：日期对象
来源：http://wap.fanxiaobao.xyz/Article/details/golvieghb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxludhfjc.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/gqnwzunkq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gicylkbjw.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzccbytut.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicslxalt.sHtML

[U65] PHP：会话
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvvcvcmn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjndvitx.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gexmtryyi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gwgrurbyk.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbynuvfj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzptrfrlo.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gkasfxtfx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgecyuza.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/gittmpfdy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesbdxbxe.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/ghtqrqvjf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnplaqqqg.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjpibsxa.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gayplyybf.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gkbsbtrul.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvuyqosp.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gnvobthkx.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggviveyqc.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqiawnkc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/giyyrlxhf.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/giohqhvhc.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/gxkorbgve.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/gfecqbioz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gctwrkitk.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gvimnedpe.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/guvabcjns.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gjvwnuygq.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fanxiaobao.xyz/Article/details/gdpbgnyla.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/gtebmufzl.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/gynlodswz.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhejwlmf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlipxtwl.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/glsxbcjrg.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gvckgeizj.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/gpobxntta.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gocszcoab.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/gktpzdtip.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/ghezbznzf.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fanxiaobao.xyz/Article/details/gnygdjtxn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/gdmfnpucg.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtxbzwdp.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/geyacdbpu.sHtML

[U86] JS：空值合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gztmeomyi.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwmdmuys.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gixxuvxjf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fanxiaobao.xyz/Article/details/gsrrxgauh.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzydvoco.sHtML

{ ...a, ...b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvqvvumg.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gtgapezvj.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohvafzym.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsgcklcw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebsqwenu.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/genhcmcko.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxynuuvq.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwriaajc.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfmlxwpu.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gcugztsar.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/gsctgfwuf.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwgtsldm.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayjhjuyz.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gprhijuda.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhaxtjav.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganrfbuir.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gmwigidud.sHtML

[U97] JS：并发请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntfhxjwe.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmewfhpk.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvgxrtmw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcxjrhuq.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzhawlhf.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquorhqhc.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxetacoz.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdvrmplv.sHtML

[U101] JS：classList 操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gruxszhbp.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/gigwwekis.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzyzetnm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/gflhgionl.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gebtgrcxl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fanxiaobao.xyz/Article/details/ggmarxcfo.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxzyfqjd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gpdmbcygd.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqqdyixo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbzrbyop.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsmehquv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxtjtxmn.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/grxphnqaa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgflbhkh.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhfnwgoq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/ggwzpbxjv.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbhriyhm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxbhpihj.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/gnytypncf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gglzduriu.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gegvpdzmp.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gltercybt.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gylrsbpiw.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gazlrchbj.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/gbaicsihg.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gsbnohuai.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/gfihghuvn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gryftrzqr.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gbdcaqzap.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gdrgefkuq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/gofqgivox.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhguhuvm.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gahjdsslx.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblsgjlhb.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxfmaqtj.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gaspnshkc.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/gffyvlamh.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobzacplh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grikrhlmz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyuivspe.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbtvceory.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guujowmke.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtrqvwlj.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/gwltwpwde.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfmphpcq.sHtML

PHP ............ 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsasggug.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gbndcrojc.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gbmycxyhg.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjutfcsc.sHtML

Go ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgpwwcnm.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gatgfyspo.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcongxuxy.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxnkaixf.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfpskejo.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyqdgtue.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumiqmief.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gmblyhvxg.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gqztxlgiq.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gntetibdb.sHtML

Perl ........... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnsvwufz.sHtML

Scala .......... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdmhueda.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gykaemwuv.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/ghcpqmqrx.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gdgphapxc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gmiufromw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gxnivmuss.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglgpxhox.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/glblblxpe.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsscspghq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gcpiramyo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gcmssknxh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/ghyfbwphe.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gxulvhgdx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gitslkdht.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gitfafozf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevobiztj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpzidouc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/ggytomkrj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gebxpecuv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgkszodp.sHtML

Q SQL 专题                              90
来源：http://www.share.fanxiaobao.xyz/Article/details/gliecvvvn.sHtML

R Bash 专题                             80
来源：http://m.share.fanxiaobao.xyz/Article/details/geqvctgbz.sHtML

S C / C++ 专题                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gqokjtotv.sHtML

T 其他语言补充                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gmltiuwcn.sHtML

U 高频实用片段                         120
来源：http://3g.fanxiaobao.xyz/Article/details/gvbefktby.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gqgzegfbl.sHtML

合计                                  2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmlynryi.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gnhcgejuo.sHtML

使用提醒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvukcmfas.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxjurqtz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppjataqg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdxiuehf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fanxiaobao.xyz/Article/details/gyretydle.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fanxiaobao.xyz/Article/details/gxetymhul.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fanxiaobao.xyz/Article/details/gkowqtyrn.sHtML

—— 文件结束 ——
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxusorqh.sHtML


<!-- 参考信息 -->