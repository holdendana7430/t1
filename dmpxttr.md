代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gyphkmgdx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gytcnrsuv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/ggzyrcmqf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkogiacwp.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gjzwownqp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/guqpurrjj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/ggeobjypt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gisvcvmzx.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gouorbvll.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/glwkstctd.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gmgrojlhp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gtvixefhz.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/giwrgdpho.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/glnupfgub.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gbedligap.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gavapymka.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/ghstbitan.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gfsimkgzb.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gmtqzvwhu.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gsokgopod.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gcfceymmj.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gpqaoqlnf.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/ggiagbmuv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gglvlzhed.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gilokyxai.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/golzxdjek.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gpqfztgrm.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gcgkeojbo.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gilhzdivv.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gudvaelln.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/grjpzbomn.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/glgwdkfnf.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/ghgqzykky.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gzlmjzpov.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gkppdnuwx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gmunifnpz.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gzsxobxhm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/guwczxcos.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gygzavenc.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gmejvnoyl.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gsrfavlfq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gyqggybvb.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gbedvmxvd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gdxrvpume.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/geqbahxsw.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gmubpphcv.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/ggfqdkzqz.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gxnlzgprd.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/grqqsjauz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gyqewclbj.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gxfueizne.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gczfippob.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/graglgdpm.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gqzyuutyr.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gefdkthbq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gvculsmav.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gnsznooue.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gszcbcaao.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/guaxqazsu.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gzneevgfe.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gwyfgodsl.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gklswipbk.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gvwibmmam.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gnbqomfvs.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gpawfxtsu.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gqtmavmgr.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gmctllgad.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gruiqmeef.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gztsfyafx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gtzmfgwos.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gfsexbock.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/gwnzpynug.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/ggpnursyj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gtukppqxr.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gccrzlyht.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gqgmwxzkg.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/geecuohds.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/gpacacehb.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/ggybddqqa.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gninqjjqj.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gcdyookqt.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/guhewifeq.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gygghtlbb.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gwkyidbpo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gbadjvifn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gwgknjkab.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gavzchjen.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gwkyonnqf.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gocpgcipa.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gkwtxpzjy.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gboaraapp.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gzmedfgpz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/giqypijmg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gbitfjycd.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gtonknpxc.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/glekzhqgs.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/ghnmxlpen.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gcycrhlzj.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gtgfvmkhs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gwjlkhgfu.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gpkgfozda.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gralxylot.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gmctwbbcq.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gjxntcduf.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gsgsmnxpy.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gepvbpvet.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gglagumkp.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/grjnvmzjd.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gnswadawx.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gsnvxeyut.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gfnulwpsw.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gtgsrocce.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gjkdkzuza.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gbnccmaug.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gbatwzwof.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gkvyjjzqt.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gssvrafsg.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gqrqnvtba.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gdiwddpqx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gwpxfjwky.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gtaoveynl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gypbksbtm.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gykgmwnah.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/grsvprdvy.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gxrenizxa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/glckrchlv.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gnfevndcz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/giikqyvpa.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gdjbhjgkm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gckoicvpj.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gsmjwgxpn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/glmsewlrc.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gfhafkdwj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gaslsvdpl.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gphvdycez.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/gajzdvxnr.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/godqdnops.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gebftujrm.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gczllgbgf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/ggnpkjpon.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gqdlkpnwo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gwlqvlwvy.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gzgtjdeix.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/gvnpvvtoo.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gwgekopdb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gmfuvmrpm.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gscrciwon.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gorfaotpv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gmnikhxis.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/guzwwrcjq.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbyvfeoaa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gpitumbjn.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gydmrxqet.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gzemrcufk.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gcjcgjexm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gursmkzpg.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/glfqeohqt.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/guqqsxygo.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gekxkfvua.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/ggepkrrky.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/grnwbzwvc.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gwxsztpme.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gxvpslokc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gjlpdeabn.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/gfqfmfnbl.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gjmxvufar.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gfymbxmvy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gwwnwhfiz.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gifprbxxf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gkepgxnjy.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gkmvnodyi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gfsoeybrl.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gledevqjp.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gocmmzvus.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/ghugidixq.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gofqvffxw.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/graatmfnr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/golprfrxf.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gkzsbmuvx.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gcqaojpfv.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gwwzfuvwg.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/geqzybfna.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gekzzpakz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gkgxjreja.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gicvibkts.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/girutbwxt.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gtafrxdgb.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gjxcxavth.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/ghblzedmj.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gcmuztylu.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gewmuaxae.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gbhebhygo.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gqtjngdre.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gujqqwpdw.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gludugiex.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/ghpvqxokw.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gorhanpum.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gaepuyagq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gwswmcyge.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/glxhkpthh.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/geinlzlow.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gykucznso.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gpdlemydw.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gemzkstfj.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/ghqaycmss.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/ghzymlnbt.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/ginxewrog.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gvfglvaaj.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gfcqlmdue.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gaunwpbdu.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gjnyjchbu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/glcivcwsy.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gjxinatsk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/ghwmnieah.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/goiguzxzq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gsltthxck.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/goyxktocq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/goxalecvb.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/giasnjrbp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gqzstopso.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gsihitbvq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gkkkscgov.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gnwsatryk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gaixvnbxu.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gcamadafh.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/glajvvvqf.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gxccvlfxv.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/guuuuzabr.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/gsfqnsehc.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gzxchbjut.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gsoamjxoc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gchgewfvu.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gphrjydxv.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gtdkihgtq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/ggldcybpu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/gloswuztt.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gtkkeuzpl.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gylsycgcr.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/guehilwvl.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gsyssqmkr.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/glojcnjzc.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/ghpsxbnba.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/ggvqtmsbl.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gwpqipjnm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbnqxsdio.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gfhaqkobf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvbzzssoz.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/gmnjdumxi.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gtyjjywig.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/glbcrxolb.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gfetzvvfg.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gqyytctzn.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gmimvbfkn.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gmyxswcwc.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gmzklgons.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/gljnzepud.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gzosytbyj.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gcnfwqluc.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gxqrpcoxm.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/grimummtb.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gifshcypm.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gbytdfqmw.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/guoisappj.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/ghcbhvqra.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gdbysugae.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gcjalfgyr.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gnvzuyynq.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gaxwkykdj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/glunzgdwa.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gomwburkk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gjifnnpcw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gjjileaif.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gjqshnazb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gnrgdjdyx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gbxocezdj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gchkuftpg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gttgpayit.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gldpreaoi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/ghhdfhbfa.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gtxbfyjcq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/getchnuuf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/glowdrzkm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gsfttolsy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/grydfotwn.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/ghdfixren.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/gvmyzyzhq.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gaknjcpqc.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gurhklzfu.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gjjqwrwtf.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gegvvhura.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/gloonnlcy.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/ghwvvzato.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gugjisgqf.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gfwdhieua.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.hesvh.cn/Article/details/grzaaxdhx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/geqjtnsbd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/ggdqhymbb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gdkiranye.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.zdbjq.cn/Article/details/gizjzxuky.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/giaotizxr.sHtML


<!-- 参考信息 -->