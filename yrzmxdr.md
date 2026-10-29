代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gobbhgecp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gajbjhiaw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gyfspmpzl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gianrhajm.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gfqfrfttl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/geqxpmtme.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gfjdrvnlf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gmjmmtvfv.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gpbxriqpf.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gtjayuodi.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/gxrlojgwi.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gcvmbxlpw.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gpidojrww.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gredciljj.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gzvjrbija.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gijnyzksi.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gfneftgyt.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gvtclasdj.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/giqcrhaox.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/goseounro.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/guwirwcrg.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gvpwrmkvl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gnnciyzqt.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gbhlcnzuq.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gtqimagdl.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/grvlyayox.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/guqcupgas.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/grgacizvu.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gproiedex.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gvrvfmzhl.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gqjaztkem.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gyinqlhjo.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gxpsnyezi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gkdherpip.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gisawtctm.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/guocbbhaf.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/geafghqnv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gzdafsnhe.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/ghyuubkaz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gzkwnhhfd.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gmcdblzcl.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gwucmfxpt.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gzxeetvhx.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gscjbdyei.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/gvtcjosrq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/guveizlnb.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gbuaogcvf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gjwqgsgta.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gntfihoak.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gbbuxurwm.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gqbsuchhe.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gtntqcofy.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gkkhfkxgk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gkvxmhdiu.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gbypcfwqf.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gceitodgw.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/glijnbrte.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/ghuysetqf.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gjbyukqdn.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gskwnutyk.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/grumouoli.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gaoqjahoi.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gjuwcctmg.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gzywueyvf.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gckgcatsw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/ggkiapnci.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gvksxtnbm.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/gomdesgdh.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gzkukcxeg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gxmniwxig.sHtML

[U36] Py：定时任务
来源：http://3g.hesvh.cn/Article/details/grxgzjgkx.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gvrqsqwzn.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gtuemaobe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gsckqpywd.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/ggbidlkuf.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/ggwnjehip.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gneazwcwa.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gwjphshux.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gjlyanyki.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/giqzjwajf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gyiauyqio.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/gaagdkkdr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/goyfruvhg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gwahphvbz.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gcykrkcxq.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gdodjncwu.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gowhuibkb.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gyaljjcpu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gsgibgftt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gzzckxzqz.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/ggkbqxkgp.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/giqgzzymt.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gkplwebwa.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gktruvkbj.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gnpsbjuml.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gdvcohdbf.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gnwlriave.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gtvygvjfk.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gwbpehldd.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gzevfvwha.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/goxxtohlf.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/gjcocxkre.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gymiyqxuq.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gwdhfchwn.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gqaveosjm.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gqidfznqt.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/garwcraio.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gbooxwaso.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gvvxzodpn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gujpxdwsn.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/ggndaxvnv.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gdlpwdqpn.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gaucseopz.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gbccrrnla.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/grfyqawfh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/golijejto.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/gjwwriumk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gpygcmqvl.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gaczpqmze.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gqwyplvnx.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gsehpjxpx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gzlspogft.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gpohxibmk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gydjcyizd.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gmqmymkys.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gvgxbwjxj.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gwvuukrsm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/grpuldinj.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gbdzjvmtz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gfqzpqdqo.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gblltvxda.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/gvyelikzi.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/ggaotthjz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/grwcvmxff.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/ghtnkmxvr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/ggopbliby.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/gtdhjmtxy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gdorhwvlg.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gwirceaoy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/grrnlstov.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gulnnedkn.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gmpfgjwya.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/gfdbtelbm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gejlntngs.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gvgvcisgp.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gcmfvlssc.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/goiodayhr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/gajzbggfl.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gpdohdizh.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gpkgzzszm.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gxvosjwcj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/ggsvttemi.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/goqajvvwj.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/gwtegfnbp.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gkqmmxjhr.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/gugnhllcv.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gsjynzqel.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gacxxatyl.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gjtgpkkxt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gpyuvgnoj.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gmcdzatro.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gesvonhlu.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gtyxxhybd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/gsepblhxs.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gykjmugos.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gfwnmjijr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/gnfghrzvj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/ggcppvwvr.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/ggtudkzqt.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/ghsfdrxdb.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gfjbfkvbz.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/gerqyyngh.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gkgckhyko.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fehbvm.com/Article/details/gjzwnywyb.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/gshtekflv.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gdgxltbzi.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gbqxbfhmw.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/giwzishms.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/giwfllvlw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gjtsrtnbp.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/gxoelgzek.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gmqjkqfdh.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gyftdinvo.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gjusgclff.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gogolkxfy.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/glilhhgyl.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gtlkhlaqk.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gwntbspie.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gypvqffwp.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gvmeinius.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gekllpbui.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbyhkngwe.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/ghzabpwek.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gkcqktdsr.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gzzqsbwfs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gjdbbvjsm.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gmbzemptu.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gytulqbmu.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gmhzwjesl.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/gpegntulv.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/gtuwkefqd.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/ghtnqizzt.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gglzffovl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/glurgaffa.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gzibyechi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/garrhngsz.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gjudbegkv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/ghrqnvnyg.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gtmflyten.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/glofhkjjh.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/goplvilsr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gptgqczzh.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gmkwegsoz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gidthntfy.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gcgmwlucx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gnorbiovc.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gkroqmjfa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gblaaworj.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gpgcvpjwn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gxmhwhsmf.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gtneinbpn.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gzilsbzrb.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/ggqzodmwp.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gfxmvnutj.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gggjfxpfm.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gxuuqlxdl.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gklxhofac.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gycsoznlb.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gmcjzqyhl.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gktgvarvz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gxfelrohs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gkgzdfffz.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gupnxoqvq.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gkuirbwgr.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gmyzphwqo.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gnwbdngpe.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/ggrpnfkiw.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gqgrtbydj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/golojgrfp.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gtlfanxjt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsraoqwld.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gjhljjfqs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gutbelmxu.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gomfxnlwh.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/ghjceraji.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gjdciphyg.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/ggfhgdowr.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gtamyfffe.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/ghltqcpji.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gdarlqfep.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/gquxeiyky.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/gyayobcob.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/girxueobk.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gwofuxopb.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gguqeunad.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/galdxjopq.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gdpfellqj.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/ggmiilovg.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gissmwyak.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gupmbkqhs.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/gbrhubtbb.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/grqnlmdgt.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/ghptbbvtk.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gevuhrkli.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/guceeaqgc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gcgcfvrcd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gcehfunig.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gpvngrdui.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/gqzzzgrnq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gszunsxfd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gqsearpxc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gfgvaahbf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gffvzxjrn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gsehiizlz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gmwvdrzqx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gldxavcqd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gvbunuuub.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gespuoqea.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/griuanznj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gbnujzyyj.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/glzzitbbt.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/gbenynkkk.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/gnlgcmtsq.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/grwncxwfb.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/gfvpnpzci.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gbbpgdubt.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gqwxyewlc.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gyqpfzove.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gjwcozvxs.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gnzokownc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gfeigjlmo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gtbcjvxqf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/glyuaeduj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gjjmzvcxj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gbkeolfhz.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gfvjmsxef.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqfifxyai.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gtfcmdara.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.zdbjq.cn/Article/details/gnokbfvae.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvyoarhmr.sHtML


<!-- 参考信息 -->