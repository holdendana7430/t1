代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhspnkvy.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/grmoanffm.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwvhhydt.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gnxxspbvs.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxetjpqa.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjbsmgwm.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtkswxre.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gneoieanb.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghchbxjxd.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/ghnvraewc.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzdeuxgw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/guiqabwon.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gdzblonhr.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/glvmlzxfd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/ghrbmbfbu.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcapdnfsi.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkseista.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gjaqeztpy.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxiojnhp.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexjwiiup.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gylliqsxh.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsimtagwv.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebvjfmvk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gftepuifv.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmxkhfdf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvmaaijb.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gsmlaxkcn.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgmpmdmv.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxupmybmf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/geolnmlwx.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gnpcgwhzh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/grxlwuxwl.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gfldjnncd.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcotnpik.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gbjgnxxka.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gyjyentrx.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gysifndyx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gfxzsojvn.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/guqfewaql.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gdelwrrjn.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztjdinbt.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqqxvkbk.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbnwpldv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwkkelbw.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gznzhhcne.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gzwiegnjf.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxwtmqbl.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gamliorfy.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqswlrmu.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwvdhivi.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gqffkdrsy.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgojsyaf.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnjfhbai.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gzzkfauqf.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gtlvsqbrx.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmspsfei.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/gbxcpbmde.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/geeluxkgm.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtfywvny.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcygkjorn.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gjfywdoey.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gdhnemijl.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmhegsze.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzzwehpo.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/gshjbgbvy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqwvqvmp.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gerlnbtry.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/glygzckrd.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrhymzvy.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/ggglqiolv.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/ggwcopixj.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gxehcyiuq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gohikhqas.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieompkks.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/ghyzvfzui.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/goizgefoe.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/giopmswml.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gltytgiul.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginnbcmfa.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigtovasu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/gytdvpeyz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnkrltnjm.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/gvvqzypzu.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/gbsqtzlgt.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghopiryia.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gazocukty.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gulltjyql.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fanxiaobao.xyz/Article/details/glffmkdsc.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/gcodpgiji.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gsiymmdhe.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gueirnmoh.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/ggnqjgzws.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpeewbvv.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/gddkrcemk.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gausdyioi.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gfqpabuml.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhkmfgpp.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fanxiaobao.xyz/Article/details/gomqcixkd.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fanxiaobao.xyz/Article/details/glpntkzks.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/gqrxmpuab.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gqcbrgdtc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gggmfqwrl.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gqquzewuh.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfbbjszk.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwxruypx.sHtML

"值: {$a}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghuwvdavg.sHtML

[U58] PHP：数组三件套
来源：http://blog.fanxiaobao.xyz/Article/details/gvdupdijx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxvdhtyd.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/geiqoeset.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gfaxufnbk.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/gnjkcbumc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/guahyqldd.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gghibxmrl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzuxqkhc.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdaeoguoa.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/gblzlpuej.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeasuvrd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/gmwklcjqd.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpdjgujn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/gchcbqntt.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/gikvgpomv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyxixiwy.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gtmqzwnsm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzniujidj.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/gkbquhxfy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fanxiaobao.xyz/Article/details/gonbnvbie.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/gunobyvpj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhwwfokd.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gccojkcph.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gyzpepepx.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/grunbviqg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gmledtsgx.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/gqpxugavq.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gqgtutkih.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/gykymkmow.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/getfqioaa.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/geubwqfgv.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuenmisr.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfixeryy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpscnzhjp.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbzdxrcy.sHtML

composer require psr/container
来源：http://wap.fanxiaobao.xyz/Article/details/gaectirrf.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfzdjsnk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gtmnqpypc.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhomdqsq.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/gewknoomh.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gbtmmcoof.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fanxiaobao.xyz/Article/details/grrsbvliy.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gajbfsopj.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjjlkfjl.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/ggfrfsvkw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/gggdpzcny.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/grdxwqrhg.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gefkxioss.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gvgfvbuct.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggacusshj.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdbysary.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/gwthgplxu.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebuonbbc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjuxqgsd.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gnmfiwptq.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gmptetmxu.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyokybagg.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/gtilbcdwt.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczpfoljt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gouyjwioq.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrxokddt.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glraryqui.sHtML

[U89] JS：数组去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gumidkjln.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxiotvce.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgaesicj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gizxjtgzv.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gjfppqltq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjmrrvky.sHtML

[U92] JS：深拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjtgnwvq.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvofmaiop.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gtpczgxgq.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/genssjzlq.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfithqnpk.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/ggvosmppo.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/gzbemtwpu.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gwupuicxo.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gwadhonvg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gfvsdqlfe.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaujhbxp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/grepnnsfd.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/glptdatva.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fanxiaobao.xyz/Article/details/gjvvngyfs.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/ggmhgekkh.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcuffxxp.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gjflqasds.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpazkvfkb.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/gqcowxgti.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/geaethyks.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuoavidj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrynooit.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/ggtddrout.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/govnrkupf.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjemyolz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gildvnuoh.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gmqadcbzx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqmhchnh.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gwahwsbag.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhhcdohs.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gidgapgow.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspousxig.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuvouctr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gspyiidga.sHtML

[U109] JS：数组分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbfwljah.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicwsqnyb.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/giiirknby.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzhrdloy.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjspxjwv.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/guscnbbxc.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrtmfdrz.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gfdyxsndb.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfadjouub.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/giyclmecn.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gubzeiszu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/ggrlsxnuj.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqawliwc.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdkeljpd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/gcaybrvuf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkulyvlw.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzegluff.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fanxiaobao.xyz/Article/details/gzvphvopi.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gspkwnzjd.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gruvwvdiu.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqtycdks.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkuoqigq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrlwpfgk.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gfohlovxw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/goxrmnhzn.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzthrjztx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gssucnnmt.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixnwrwso.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gdxuzgvzs.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxnooihu.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gdapwubum.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwudhsvk.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gpdurrxzd.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gigfbdkpd.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gizirewmz.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipxfbujg.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/grhkwkmrg.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwrkfikv.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gcqkwrqru.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gcnacrrzj.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/giwxpszxu.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gcopkyypb.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/gcxktiihf.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gwxwltbuo.sHtML

Scala .......... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrttlnam.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gzsuikcqj.sHtML

合计 ........... 2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/geoxtzhmm.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqxfzqlz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gmmmfntey.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gwtiejaoc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfswzulx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkutatwo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gplhtvuqs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gemnrorhn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gbhyeyvmx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gculmaizz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaalnsrz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/glufdbatp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsyggqsh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpqkqjgk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gqugfzyxc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveursqjp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gyaijlgxc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gmjbvjohh.sHtML

Q SQL 专题                              90
来源：http://wap.fanxiaobao.xyz/Article/details/ggszupcee.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfoxbezw.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshntsuix.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gaxvenlep.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlbjxazm.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteeeegka.sHtML

合计                                  2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gfniudaly.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gzryxjaax.sHtML

使用提醒
来源：http://blog.fanxiaobao.xyz/Article/details/glvjwmols.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gncmjadaz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/gljaqndxj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fanxiaobao.xyz/Article/details/gevdnqjco.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgskdxeh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkffmluyo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fanxiaobao.xyz/Article/details/givvfcsja.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryjmuqth.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjnukusjm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/gflkgfxns.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmijtvbu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjbfjvdw.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/gzpbxwoxn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/gczexgibu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbtxkild.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjxznlbo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmxjoywn.sHtML

【使用说明】
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrqligpa.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fanxiaobao.xyz/Article/details/gfftvpnlh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxyrssbz.sHtML


<!-- 参考信息 -->