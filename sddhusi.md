代发 wailian999

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gxwqsmtwv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gbghypycz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gpymbvxya.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gdzalzgen.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gqncszigw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gfyjncbuz.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gcodornyr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/genmgfhaq.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gtwcslfnf.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gryyyeblv.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/glraeyktm.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/geezxpsoh.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gtjeolmiw.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/gcgfdyako.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/giqpntsrg.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gpuqyanbb.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/grsprzgmw.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gegroupej.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gqfaordph.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gmrjmfzei.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gmxizhbes.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/givxtdgrc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/grcprehkh.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gtsrdsmhz.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gegaletey.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gryhnwhbo.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gbbuojqsm.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/gyslwjjkn.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gzznpmybl.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/ghycsemfy.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gwhghexqs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gbfujtrvq.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/ggipecglt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/gusknklzp.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gyvsxvddd.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gtjiltosc.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/garvyymit.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/ggyovupxl.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/galdwofnc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gloyirrqc.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gxzpqokpa.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gxkrqnhjx.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/glwdnqmbm.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gytqnwfbs.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gqjksxfkm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gngfygfsf.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/ghxlbtcux.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gtndrrrbl.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gzeijmapb.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/grzaazzfy.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gplsxqvla.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gsznnbtpw.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gxogxamsk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gtbqxyurr.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gqnmxhocd.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gzjfnuzux.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gfrypqqmw.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gyzkpptkx.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gcvxzcckx.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/ghrqjltlw.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gdqqunfbt.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gdiunxynk.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gccckmcmr.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gksmjyhnb.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gsptdpoos.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gtczbcjrt.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gkeessgpw.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/ghascskyb.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/gfkjlrxvl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/ggttrolpb.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gvfubjnvz.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gyxotkhnl.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gnthpswrx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gonvszqiv.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gwpddtagw.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gkqztktsb.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/gaosyjqbe.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gwzijgjwd.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gwyxngndc.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gznlbxuff.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gsildxlqy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gnqyofhvx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gvxlowkdg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gipnwaibm.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gvoxpbbfy.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gkqmtcfxh.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/geagtpplh.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gzsfpbxgi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gcujeupdw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gpahpuski.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/ggajnyzik.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gdnmftnaa.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gzwmfsziz.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gmdolwvoa.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gfvkbqstg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/goltrgrzn.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gtutxmsgu.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/galfixndk.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gheggroda.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gxxzlwgiy.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gtwrfvuox.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/guylzdlxm.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gpoeuqakt.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fehbvm.com/Article/details/gqevmzkdl.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gmdjimklg.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/gcwmsabws.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gkvxqclgr.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gwttrzwsq.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gxurqldxm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gmgjyvnbv.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gvabzlmye.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/grlntrzfc.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gpqenznty.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/grzhfvlen.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gmekjsoqt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gqohzcpbs.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gkyieztqa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwibtksop.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gvtunxwbj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gxgahbase.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gwiujgwgf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gieaaihig.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gsypcrjfm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gbehrsqnd.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gxqybxobz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gcbfmqkwz.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/glgxktrrn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/geosimttk.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gmlczaena.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gnkjncrvt.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gpbgqapqe.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/gvdmykwai.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/goerobvck.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gtaxjeryw.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gqzuhahoo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/grdmwanvk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gidewrkrw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gshwiwnzt.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gjexldega.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gxrabmqks.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gnmdeshca.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/ggljaxuxw.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gmtsbjkcm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gthtqnaun.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gduusnicg.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gixgpwhyw.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gavmneojy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gyiowydir.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gjnoqicti.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gvkosfukl.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/ggpzlmlvm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gxzbrkauk.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gmbuxutsj.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gclatdvao.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gfsastvki.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gqdmcwbwr.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/gfqnbufrq.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gggurigxi.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gcpnawxvc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gazrmzrck.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gjebioupy.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gixkmtkkr.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gwbpziyih.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/gjadttydt.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gshpxgckp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gculqersm.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gudlfsfpj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gvegjercv.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gewgtspgr.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/ginzevayy.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/gekqltilh.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/gbdpyuvxj.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/gdlztsnsn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gagjnwijt.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/goxejbteu.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gaabdxkzp.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gpoifrvey.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/galoutmgu.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gxujjevii.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/glmuqyhyz.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/gjraxcvpy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/grljkbcbi.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gqnjjpaxx.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gnlqtwcsc.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/gvvtifyuo.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/gjmwpjxca.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gdqiqqldq.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/gjnawnbuw.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gnniczhut.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gclcimfmi.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gshnikbwd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/ghbhnaktx.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gothshqyq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gnhstuome.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gdluqxdao.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gzeuglruy.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gcoxqwqjc.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/glnxnpqfr.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gefkedmjv.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/gwtjftisz.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/gnkhvglhb.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gqtemvbem.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/gxiedwgzz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/goxgbrhjo.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gzzfdybny.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gxreievyy.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gdbheqmpf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gaeudojoz.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/glzqqxvyg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/gyarvkhtv.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/ggpuhbvum.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gzljuvkkk.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gidzdysov.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gzasbolgw.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gkrwnwlrl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gpjxgbheo.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gfvkllmly.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gdghroumt.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gvgipfdoh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gkfmjirdm.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/gdswzntwr.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/grkgacvaz.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/gfjhfqzaq.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gijbhmqmr.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gvonriknz.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gdrcnwtcv.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gwipxmxcv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gjhtkprbw.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gznswjzpg.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gouaogxmz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gdfafqias.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gcdqbvhlu.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/geruudgdy.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/ghsbhqzmv.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gjdxglejy.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/ghwctwuhu.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gnsiarsui.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gqauwwmnw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gcadqzcwi.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gctfnyjhc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gezcylbnj.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gmjlvwwsh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gklajkion.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gjnyknrzl.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/ggrpkffsh.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gqrmejkyf.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gprbpncti.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gmyolsqhh.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gegxmscyt.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gnoabrmhl.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gzkcgxayp.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gfqeahvkq.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/gcrqakvrq.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/gguabkqxe.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gmuoaxlej.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/gvqgwrltc.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gpgrbagez.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gthnihjqg.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/ghjeujhvo.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gpcqxsgwl.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/guvxlyqbz.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gzcccgeub.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gynlafdnt.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/guwaqxbmd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gcqzipasi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gdyytqomr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gbbuyapwy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gcvvaovho.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/gykbxjvmn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gvkulcmbg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gtyaibgwl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gayzmgtgy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gqekhtfqv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/godfzumwl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gbqjxqlhm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/ghbbrumxi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gbeolphyv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/geopivsut.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gdljtmxut.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gfanxputg.sHtML

Q SQL 专题                              90
来源：http://mobile.fehbvm.com/Article/details/gcthglrqu.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/goelgnorv.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/gxzmvgzwm.sHtML

T 其他语言补充                          60
来源：http://blog.hesvh.cn/Article/details/gmqvmyqvb.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/gogjpsxjg.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/ghrrwlsuh.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gupwuglui.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gojnkwxfs.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gnlwiuvdc.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gptfyqcza.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gwjdayvuw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/gwjaznjcp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gqmkwaehq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/grhfvqnts.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/giuvawcfb.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gzckblcre.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggkxflkzo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gggpwkkkc.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gibeytnyl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxtkcbvxx.sHtML


<!-- 参考信息 -->