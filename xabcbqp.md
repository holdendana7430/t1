代发 wailian999

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gsdlyyjjr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/goldusrvd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gojeyaphw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gcqkcuszb.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/ganhgwwte.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/ghqnoqepn.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/galcryutx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gnpietrui.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/ghoyexzpr.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gfxxkopud.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gioqkkjrj.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gjaqqjlgf.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gsujjytsr.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gvtjccdxb.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gswsjomev.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/ghhogllzo.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gxviudiyu.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/gyedpywqc.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gejzmxlmo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gdvzvkaiv.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/ghfueoviq.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gzdswhgyg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gvsudqokk.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/glopkolgi.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gsothnuml.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/gejjmowiz.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gecqqrbnz.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gwpgeahei.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gaoamyaqp.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gzphykwbg.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/ggocjgszp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/giuwwwkcv.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gizghwuyw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gohnvedjt.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gfaamogyr.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/ghcjbxips.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/ghfmktbzg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gyjiokxno.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gjdgishds.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gygitcwdv.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gclzoagmh.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gmkgspeda.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gfenobkif.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gzssaqbry.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gytchblmn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gtvwzgtxc.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gdlrueydd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gdhtvsfjd.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gwyjmlenr.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gvksnokem.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/glrwcwtih.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/ggeqrsbhv.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gfevoavpi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gbqqmjyxb.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gyfstnxdb.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/ggkjbvpll.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gskfmyoif.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gofnqwgcg.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/ghxfgnenq.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/grcltguin.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/ggxkvwytb.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/gnwyykomh.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gegzplvux.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gepbkxxsr.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gplapybpb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gbarzkbal.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gnrvurncl.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gjgvayhhl.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gtriegdwd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gwuqfxcfi.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gyrlkbttx.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gxiqdmkmi.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/gtxtrmysy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gdxscgykh.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gkadocria.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gqztuyzfo.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/gyciqrvgh.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/ggrdcmmjd.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/guphvphxw.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gwcpplzdm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gfcdrpgbw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/gtuqbnvpb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gltcrcgpe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gqlzdrswq.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/ghgbomrle.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gaqyvgezt.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gahicehal.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/giduqwpbj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gpxzgxswk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gzktniusy.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gpwbakduc.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/gdludijyb.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gxsttqbdi.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gkjriqhwc.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gsiegvbvu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/goysdatzw.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/guzpyrxnv.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gizfhooys.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gpxobqlcw.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gqdvqtshr.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gtnmjxmtn.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/ggotljniv.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/ghqocrgop.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gxiyfzpey.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gukkndivj.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gnqixcykz.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gehcbluby.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/ghcrrfyph.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gpudtmfwt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gyziwqbko.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gpkiaipgv.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gxfhawpwe.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gciuvqiaj.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/ggzorjmhl.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gbuqndfeq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gwybhdumw.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/grwmqbkkw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gcwinsdnl.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gcvndniwt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gkpwuarlj.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gjemcqwfv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gegvwsofl.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gtdgmtskp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/ghnwnxixn.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gujjcznpt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/grcsqmxfh.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gbibgzoev.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gdaftoqrd.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gkhzxybwd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gdvkngldr.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/glfpbefiq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gsuwpkwdl.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gaysxuouv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/ghpxwmeqm.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gqxfwzqfw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/gwaylqrpi.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gmzrtivqm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gereanhzw.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gckkbxxdy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gzisgdfkd.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gtjcadcdo.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gmeytiaxw.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gnwodpofr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gijqalhof.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gnpluvrkx.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gzzudrfcv.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gmwwddynz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/geyadtidk.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gtapaxadd.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gkzotzafd.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gjalhpfoy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/grezpwrfy.sHtML

[U77] PHP：模板渲染
来源：http://blog.fehbvm.com/Article/details/gktbizfqg.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/gyeazmhoq.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/gaxmmilxt.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gkemrdrab.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/grhpsxgky.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/glfcxcdtd.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/gbvslglij.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gnhiglvot.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/gbacguklo.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gdnrdozsq.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/guxkyclqh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gspxxvjsi.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/guurkvwfl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gtqxclwli.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/geimmpdnz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gbudewcco.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/gqsfjjffi.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gpkiyxckj.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/gahcceaqs.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/geiyxvcpt.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/ghmmfpnhn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/gyqdppxxd.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gxzzrjdsv.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/ghpsfuybm.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gshszcipj.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gdpfyneul.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gmmhrqcer.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gphqaxesn.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/grkytkwtd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gtjljilsy.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gteybevtn.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gttvtimbv.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gwxmaijlr.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/geknwamiw.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gdwvgvpuk.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gsmabcpam.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gwbztljct.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/glxliuzpe.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gogvzdeqc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gmcnvhoaq.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/gswbtgrfr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/glvnecxaj.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/ggwapgiik.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gissroofa.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/grdyarahx.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gjbnhkqbn.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gihtekond.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gbktzjays.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gsnrbhvbi.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gmeqnbuyx.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gagkljbyv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/grkmuphyu.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gqtqbercs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gbmtoeygi.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gofevvyxj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gspkopbzr.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gogpuziwb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/gfeelzvix.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gjeekbtwt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/ggahrucli.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/ggzfgtsqu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/gkzxmuyzs.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gqnmjskgs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gjqffgads.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/gipjrlrri.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/guuodlsdd.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/grkrqcpwz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gtrbnhczy.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gsaadkdrz.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gycnychji.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gfozccmor.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gdckfrwcb.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gcuuoaxry.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gvqpmlkzd.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/guwmloupc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gvvyychdo.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/ggkvnzgki.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gzcgicgss.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/gbecvktee.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/ghnuzxyur.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gouhgagqi.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gpvnqzpjq.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gigskhegs.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gdazpkrhi.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gvpsiujqa.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gtphdzxvj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gbzadnmyw.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gtzrdjakf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjmooociz.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/geveettnm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtaolbvrc.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/ggftjiarw.sHtML

Python ......... 252
来源：http://blog.hesvh.cn/Article/details/gfekpvgog.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/gkyjszrmq.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gyiukdlli.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/gtswsxqtl.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gpdipyujg.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gjqdsijvr.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gxqgkbukx.sHtML

C# ............. 212
来源：http://baike.hesvh.cn/Article/details/gpoaslfsd.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gsfworraz.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gwcshoizl.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/golbudgfp.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gjyxwxfbv.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gwoqatgtj.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gorkqzwae.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/gajibpfxn.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/ghlwfmsrh.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gqtvycqtc.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gcrkpqjwi.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gjmfmrwzy.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gcpildrnt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gfpibhmwr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gjxsvshtn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gqoadbqcf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gsvebkevu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/glbyybbpz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gzaopxmih.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gfegthret.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gkuqgmrkj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/grpyydrtj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gvntndrvs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gkmwoluxw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gljydgibt.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gnhihcsyg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gnwwvoyhn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/glhgjpayi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gqjzexzce.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gdfbfgcgi.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gcritoxxl.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gkkgkmpbl.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/grgzamepp.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gjrxndrcf.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gobqqnzjf.sHtML

合计                                  2106 条
来源：http://www.blog.hesvh.cn/Article/details/gquhvgapj.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gxlvujlzq.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/gjtyfsxve.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gauarjbuh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gahwrezdt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gvhsqrktv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/gexxayqqa.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gbtmibnij.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/gmqtbmrhf.sHtML

—— 文件结束 ——
来源：http://www.blog.zdbjq.cn/Article/details/gnelfyzit.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvtbmjraw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gcgfzxcpv.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gkdmlaxyb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gaqesbnec.sHtML


<!-- 参考信息 -->