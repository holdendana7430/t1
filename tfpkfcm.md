代发 wailian999

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/giiuzgkjf.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/geibvpjjd.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/grkxxbstd.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gfphtlflo.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gqgdestae.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gvaidagjs.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gpbbdkkek.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gipplbapo.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gftnqaymn.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gdjelsdsh.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gxegeirsy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/ggjvmwxbf.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gyluukqvy.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gzmhhjqio.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gjmscbott.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gvefzdulq.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gujuwlncz.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gebgfhori.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/grlwuiwmi.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gohpgytpp.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gbbnkzeuy.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gmixpzfff.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gqshxphho.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gkrksnvym.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gxxhlzitr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gxvmxuefc.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gjuaualls.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gpyugngnp.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gefsjhist.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/grailwimn.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gebykxcyi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gvmnifryf.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gsmkfsoxg.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gyfoxaboj.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gbdvtvbxh.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gyzcoxsnr.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gwtmxkshy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gnzkugyst.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gacaaimgw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gzqpanqos.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gklfbiqxh.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gcykztcfa.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/glqmrqkfb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gpxiojrqa.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gjgixastx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gpfjsdazf.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gviwerysu.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gflkamxmb.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gflmithof.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gvayivxbv.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/glzybvozi.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gsssqjjko.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/ggqktyvtb.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gmmhcwzjn.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/goxhtfisl.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gsbpolujb.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gmmlhfjty.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gqxkgqkqv.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gxxxfzivs.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gydxkwmlk.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/gszvumwgh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/gtjahfjtm.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/geplbfuda.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/ghfchfckh.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gajjfuopg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/ggddfmzrc.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/glebdfdnv.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gvkbsflqw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/gxmawdqeu.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gnvydqpvq.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/gdogyubua.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gghjsuirr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/glipozstd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gzszbmxvx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gptcwtknd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gvyhfttsn.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/gqdeesodx.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gvcqtxdiz.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gmbeqfmfj.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/ghtlkxqah.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gpgacjvtn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gnezjbjbo.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/grlmdiucw.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gfavyluyv.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/ggazriqdb.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gaqfoiqcc.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gwoaygnaa.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/ggrdizimk.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/golqxlqas.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gbidokvkz.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gmmweamjv.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/glumbprgx.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gkruuwfun.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gdnetkhdu.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gjuakkqur.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gkvrssocb.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/golwiotdi.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gwtgskugz.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/ghsquoipb.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gvwpzvqhg.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gwlrkllhu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gftjwowjq.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gtbtwvfrx.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/glyskosyg.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/glnyzirzt.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gskrvmdhs.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/guheffrqo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/gzsfcughn.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gfbxbobsp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gydkokvhp.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/glcacoeqj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gmqyurjhn.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gxdvaosut.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gtbxrfcdg.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gwuaygosu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/glylkzssa.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/gjjysymee.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gccanbkma.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gtkgimehu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/gqgsyccfw.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gpntzrkqn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gejiqhlnz.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/gqdcgsack.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/grvuzhmix.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gankhtjsj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/gdfhloecn.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gbivkiqgp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gajpgerph.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/gmvsmpqti.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/givxufohf.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gyynobdru.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gxplebviz.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/ghnxoyknf.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gbwhjdrqj.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/gdyfgyrcs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gmtrdkrod.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gusnpnnnl.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/grkohnocn.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gezzlgirj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gvwhxpdam.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gncdpznbn.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/guhdnwwfl.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gfelkhikj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gwbwumivt.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gydbpglpu.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gmfcesvkg.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/giptlrzib.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gyqmtnamq.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gyvkiamgs.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gukslkeej.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gdvhvoplq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/gqubdeewz.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gdlnmgejf.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gdsjbetfk.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gliilbtgv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gbgdwszkb.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gxtuthpkt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gqnqxsnoi.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/glkuuatvq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/geazkbohe.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gxxjobego.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gvlsfowpo.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/ggokkpjfp.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gpqkucwdq.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/gxtcrbdvi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gljenemdb.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gzbakjjgq.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gjdgdgwjt.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/goufyqnba.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gbwbgaxuw.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/gvjraiktm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/ghyvwwrgg.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/glzfexvgd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gpjgqktev.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gxeximfca.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gvkrsegiz.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/gjqdtyrtb.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/glbpgdngo.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gcxmqfnpr.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gmgmjfnig.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gjzneehaf.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gzrhkxcfc.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gbkpjidqn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gqaugmhdw.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/grkrgrxmc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gcxoqqjep.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gjcqyszyl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/gqctlewzy.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/gbjvtkkjv.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/geaqxaacg.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gynbmoyrz.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/glxnnfvto.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gbumbhamw.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/glxykdsxl.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/grokjylpr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gbckzfwdw.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/ghepfltnm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/gbarlauwy.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/gfcuxtlbv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gmtizgkox.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gfxujdhyz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gvvjalvyy.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/geosqoyny.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/ggjctqcei.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gidouhxjo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gktkztdxy.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/ganhyqbev.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gogpogsxe.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gybwtowwt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gynzggreq.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gaauaicfw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gdtmjraoe.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gecdrfigk.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gbwltotfb.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/gxebnmtbj.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gcqcpkero.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/glcjhgkiw.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gvqmwgibq.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/giyijchbc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gncmrioyy.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gfwnzaxpp.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gpnzshazg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gzyrkoztu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gkgtddvxp.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gsideqmzb.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gppbwlohz.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gbtunuqxk.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/giwfwrupt.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gvfqpilpf.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gkzthjvqj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gcfolbygy.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gqucxvopu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbpqaswpn.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gjrqrroxe.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gykgepkdm.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gqsvqtbif.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gsjvmcywc.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gzqmrxdfe.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gfwvkttls.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gprkfhvxj.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gtxgjltep.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gqgshrodn.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gbpcbdprn.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gipdabegp.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gwsxydetb.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gucnaxidt.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/ghlxidjkk.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gluhzksiq.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gruzpaqnk.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/grwbecidc.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/gcqsqqrba.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/ggfpzfona.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gkmpxbzbd.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gciapqczy.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gdfjhibpn.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gfulpkvix.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gfjnnoepw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gldounhnh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/ghodzvsbb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gyachspas.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/gfhklqevh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/glqyqjkbd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gglihfchd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gjqeohhao.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gkdliidzs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gqklingmd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/ghexdlgdz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gghaawtab.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gjqrqxfrx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gczjbiuhm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gxidwsevw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/grrnvsnmo.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/gkairtwjo.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/gcabksfrw.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/gbkjjfvgs.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/gnnhslsos.sHtML

U 高频实用片段                         120
来源：http://baike.hesvh.cn/Article/details/gwqippvrd.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gxxdiowim.sHtML

合计                                  2106 条
来源：http://www.blog.hesvh.cn/Article/details/gymbmfmfn.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gwaoanuab.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gzlmhudjm.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gqajmcgda.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/gzxyoknmf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fehbvm.com/Article/details/gmqvduyqs.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/gyhuhswjo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/gzazmhsne.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/ghdbemfux.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/gkkbbbpmf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbjfpqaac.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/ghxgkiatp.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gowylonav.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbiwshttk.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/gckjrewfi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fehbvm.com/Article/details/gptzmzoiu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fehbvm.com/Article/details/gqcmabulq.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/gcrqihzti.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gihobkenr.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gwjvtmpkb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.hesvh.cn/Article/details/gqfwheoxx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.hesvh.cn/Article/details/ghdmgzvpi.sHtML


<!-- 参考信息 -->