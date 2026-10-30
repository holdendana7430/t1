代发 wailian999

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gizozhqov.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/goezobjmw.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gklwlhblm.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyopuqgd.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gaiaukrpd.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gkxjfxrpp.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeqakdwr.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gqhuacnnp.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgamjmzm.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gldeswyno.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/ganagdkyd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gfutpbtjd.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/glpuznmiu.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhrsehcv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/ghqrownyw.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/ghzamnfnd.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhegsmlo.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgnmsess.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvtqudnh.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gheboedct.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gylajcxfx.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuqrbylm.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/gcmaswhnb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwqpkatm.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/ggncwdtul.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/gdeselymg.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcclssxx.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlhcbkut.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gmieuvgwq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glprzazjr.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gmzmxlaot.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gyqphtmsl.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxlnvamm.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvzvrrhb.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/giiqocnqz.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtnsrrjk.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/gedvlzdhk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiuwmhlg.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gotequjfj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkryqfsz.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gdacrxhzg.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/guwmdetnu.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/grsngupto.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhqqjjmf.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/glkkaelik.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/grmhbidri.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdcrzwas.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gthnxtavt.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqmxcswl.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gjcqfqern.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gldwcnmfe.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdecenfjp.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoeoygdc.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxbpqbpm.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkodtxor.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/guvjpcxzo.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprbmiktp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlptjhpp.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlvhylcq.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxqebbun.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgsreaif.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpokpppp.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gjteonphy.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/gicajrlau.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/glbxnmiqh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/geiuoyfrm.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/grpuloyfd.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gabaelsap.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvgiuziz.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/gahwcisul.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/glakgutdo.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/ggppozojp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gntycltet.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtpsvhlq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhpmqmhn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/getcffyiy.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/guxmptjhy.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gohpzblok.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnglepfg.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqharzqqh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gfqyikjxb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzwousme.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydhvgjvf.sHtML

?string $name = null
来源：http://www.share.fanxiaobao.xyz/Article/details/gswfbjifb.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbesodjtb.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gktbyswki.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gilpbyaff.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcrctutfi.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbgtsvbw.sHtML

public readonly string $name
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqpzzzid.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gbcedagrz.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkuqjilx.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gxinsplws.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhsddkwy.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjqagwte.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/ggsemlylu.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiavexsj.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/ghzitjbwx.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/gbvqwehal.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/ggqbhniww.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzavbubm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzqhccpv.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrtvzjfj.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gobvqhhyt.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gizfxouop.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/gszjymfzb.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gvsbofzzm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/glptxknce.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/grqlahztj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazcuiroy.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gksvqdakp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbucdroc.sHtML

[U61] PHP：正则
来源：http://wap.fanxiaobao.xyz/Article/details/gpobcwrhm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/guolmozob.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiavtqvc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/glyjifpky.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwflalfwt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gchrfkmhk.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gsqrjlxgn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrwcgxqn.sHtML

[U65] PHP：会话
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvovizom.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ggdcvhycf.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/gdwshtntf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekdarbiv.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsqupyws.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhbaqrco.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjcdfypb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfvplwyj.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgleeuvb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttadhcmn.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fanxiaobao.xyz/Article/details/gbzhycwrf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/gqskapgmi.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbexvmdl.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkguexzg.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjygfgpn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gdmmrexoi.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gjswlbntb.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gfnjnsvzn.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkplzmepj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxceytdq.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/gtibhzwws.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/gqvcpnicy.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/gszefzsaa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gajwftxys.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gqlifrqkr.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/giyvlgkly.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gilydwdtz.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmzlwcnu.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/gethtnwnf.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnkmvzrq.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwucaecn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/glmlhkidn.sHtML

[U81] JS：初始化项目
来源：http://wap.fanxiaobao.xyz/Article/details/gexlghlvx.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhqbdple.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/ggohmgjou.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdqdijip.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gliwuukxg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gnamstexp.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdyqfxqu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhksbikp.sHtML

[U85] JS：可选链
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdrnwojk.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqgtftdy.sHtML

[U86] JS：空值合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gprwfxokg.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/gonlqrxpl.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gfynbvmal.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxuxtmrg.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufizyppg.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjltjxnb.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/grnmjggax.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktwoqtpj.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/guoxkepdt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzllrgdx.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgpfowfn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gkllzetsv.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtfnuega.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gdnhtfjvu.sHtML

[U93] JS：模板字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnrppcnl.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gndkyrpzb.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gftyojwby.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/glruuraqa.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkizqfwb.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gutblevug.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkvqbpts.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpboxoiis.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoxppuzf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/getykiyvv.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gqqdkandr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsqfajet.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/geupzhuwp.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtkvalho.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/grvfnzcuk.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/grzbiosjo.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/ganhqcxud.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gvghdcyls.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/giuegruks.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyzrmunq.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/gizwoajfc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqtkosmc.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqhinfed.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmhadaox.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbacgwfh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/ghglacuyd.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsbjkpxl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gspabjczy.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbkidttc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwbgxujg.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/glfsdrany.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gpjkjrtip.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/godkrhdqa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfbqodda.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/giystwgsr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gttcfecxk.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/guhdqwoer.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gabdsmxtr.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/gxrdknjpc.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/giabgaiuv.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glisdjxyp.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gwiuvlpgd.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttkqndhu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gugywqbiy.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gnltzvrkl.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrdvookw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/gejkzuqau.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoynlkbh.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gffjtvhct.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/gltnzjbvk.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/giorqyfko.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzzxoppj.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/glpviuswb.sHtML

npx vite build
来源：http://wap.fanxiaobao.xyz/Article/details/grhkzjgcl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzisjyjj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxmacdjj.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgzabfnd.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnxrpjnj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gtrfipytc.sHtML

按语言统计（条）：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckdbkuri.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gtziracoj.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrngtpcy.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbuecele.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/ggkeafbwf.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxddfepf.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqcheqgh.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmecwaim.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gtjxrcaes.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gztqohrpk.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcalqadi.sHtML

SQL ............ 90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklidritu.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfapthpxb.sHtML

Kotlin ......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfcywuvf.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/ghkielkmm.sHtML

Lua ............ 10
来源：http://wap.fanxiaobao.xyz/Article/details/glpmyubsr.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqobouag.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwdacwxa.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gajkegdot.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gbxihqvem.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gtqypeanx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gjadkauhf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gaybnfirw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpouxqun.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmjegzwg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/gztqvqcgz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuuvaape.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaxfuecf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/grxlysqti.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipuyvqip.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gotnfclao.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/guibnppym.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/grstsxldy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gguaozjav.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoahsren.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/gjycghngz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gswdipstk.sHtML

Q SQL 专题                              90
来源：http://www.share.fanxiaobao.xyz/Article/details/gavvjzeae.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/gapglhrxp.sHtML

S C / C++ 专题                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwkspupk.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/ghydzlacz.sHtML

U 高频实用片段                         120
来源：http://baike.fanxiaobao.xyz/Article/details/gjilqakyu.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gqoyqahns.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gchtdqlbd.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvnmkktx.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoqaurxh.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkxcngjl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvjwpadh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdgiglvp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlhyclsr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyocxqow.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxuavkrx.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbqpufui.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwknqxfcy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fanxiaobao.xyz/Article/details/gsugjhsuv.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuhcqdhd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtulndns.sHtML

【收录内容】
来源：http://read.share.fanxiaobao.xyz/Article/details/grpdvsxjg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fanxiaobao.xyz/Article/details/gutpfvdfq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/gnmcirfck.sHtML

SQL · Bash · C · C++
来源：http://wap.fanxiaobao.xyz/Article/details/gyoquufvd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fanxiaobao.xyz/Article/details/galoavpal.sHtML

【使用说明】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtmvsisn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fanxiaobao.xyz/Article/details/gfhzaxabp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fanxiaobao.xyz/Article/details/grgxzhlul.sHtML


<!-- 参考信息 -->