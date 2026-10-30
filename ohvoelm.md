代发 wailian999

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gsivzijha.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltksozff.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gjirflqfh.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyjlajre.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gapkaochk.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/grsgfioka.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gtgwizfaa.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvdrempp.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gmyiozklj.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkndyxte.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/ghybttdfs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmstxsdwy.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gsghfqojc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gixhfguus.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gptctwtiz.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gytwonazk.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gapplbghr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gxqtsaawj.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gfdqhwpqm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gmtkihdpo.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdylkpxpx.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsfqidiu.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfeggatz.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gkrvqkpmw.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghtlrdgto.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gbriwzigr.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gjhyruiak.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gerlauvzl.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebwsgkql.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gvbnkpmxh.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/gotagpcwa.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvotrfcam.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkcatndw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyucrlctr.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcmfptjy.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gkcjuaqea.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbaljzent.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/grmtqxtlm.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gmnfqtejq.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/glmflruma.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoqukqxq.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbwjbbzv.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gssxtinab.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gldqqbpuz.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcjzqhsy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbdujdtx.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gfraiqedx.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gbrlwooyl.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/galxexxap.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gavsipagm.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgbnezcd.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gplklrjto.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzrjxjxh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/grwlxxvlr.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/gcdlugqvl.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gwjocnyrp.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgnwiepo.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/guwprqffw.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfagkfqi.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrzrzupy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gslopkujm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllrhbmvj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gysfzupmz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkivacppu.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/giwlgxhvz.sHtML

namespace App\Http;
来源：http://read.share.fanxiaobao.xyz/Article/details/gccrolwis.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gclyqlrgz.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaemwbfm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwswnotfv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbkhynvou.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfsinynu.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/gktwdbvdm.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkssnokaf.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/grqiuefer.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/glxhydzps.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/giaubtrpz.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdragktsi.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnddqwvhb.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/grgrvdtyd.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/glooaptuu.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfmhluyd.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/gsoujehfd.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzqnwofd.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmefpopyx.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gjwosfwmp.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gonffgfvo.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gmleowjcd.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlyzzqzq.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/glpzxdkla.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtpclkpm.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/ggvkcdzlw.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwixiedd.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjyxboud.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/guuhzmutm.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gwrrxqbfv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnipzhqzp.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/getwqwgns.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gseedzdwu.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gchubdhdq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gvgcmxjjn.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gazvxpqsb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gcezfoyiq.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueqpyrrg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfrahgbt.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gktgpdcsk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiuevtrm.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/ghaioxoxb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gymqwlrgo.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/guotngxps.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/grqrkhsnh.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/gznkzdsok.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsblszjow.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhnbvctb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/glktlnyhu.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfavbjbf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzamiaivx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gcowuhhgg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgziyast.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gwqnstmvj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgvhndck.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gyelhbcmt.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gmxuxjker.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/ggywzfato.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmwdblat.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gbjiinccd.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbkmrmus.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gckodvjxh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gskkdrhhf.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/gufszhkcf.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gpytzwfmr.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcewwvvn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/giyfqajba.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gvuvezxsu.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/geytzsbbt.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqywmdyep.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gqablrbcd.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gcwntebbw.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fanxiaobao.xyz/Article/details/gadhrfury.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/gnweglmsd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlcqhial.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoqdjaue.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/gjetxtyxt.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/gdadffmuo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gtjkqkwql.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtwftqrl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gjdxdzwyg.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fanxiaobao.xyz/Article/details/gpzpkuzca.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutjrmvrb.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/gakqdhhei.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahzfcvyo.sHtML

[U86] JS：空值合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsgksjxb.sHtML

a ?? b
来源：http://3g.fanxiaobao.xyz/Article/details/geesxukzo.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/glidgsicy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdelvgea.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwpsyizx.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/gntgdeomd.sHtML

[U89] JS：数组去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxjtrlwl.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gyswulpjv.sHtML

[U90] JS：数字数组排序
来源：http://3g.fanxiaobao.xyz/Article/details/gvkqnnzbx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgzrjvbe.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gjvcwxvdg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqdtzkgw.sHtML

[U92] JS：深拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gedcwpcdi.sHtML

structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gftlvgelm.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gqwqojmcv.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzntcjpd.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjdvlhsp.sHtML

const double = x => x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdvxozty.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhrblasc.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/geewzucjp.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmukkogqr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoqdyryk.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gzwmrusgj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/ggwsaicay.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcfenbty.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/goyjxrvxg.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqzujzpk.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbttkbjo.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhsjejgd.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmhqbgkl.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcyhbnaw.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/gikzcmzsr.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgdfebjt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gunchfzhy.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzfgfdet.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopcqfhyo.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyculqwmb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/goywszwvp.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/grtrihsiz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gksummbuq.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gfgeyfxgt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gpffqulvr.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigcbcnhg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/goezadaqq.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakclyjre.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnkoubto.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/ggvpkoacq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvadzzon.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/gkzczpmnr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/ghgxtvkbv.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfneitnt.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gdmjgrsvw.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gvrqcsfib.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwkusykh.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gigscpkvt.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gesvfemax.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gptbunpaa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/geyomkyla.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gktapfuzj.sHtML

crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbuoiyja.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/gqogdenuw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosgrjovo.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gaizrbbuj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gytoljaik.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/gzcdxxuzt.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyjlrcaa.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigzzzgwy.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweaukgco.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gilxrynxk.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtobswqrx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcavcehgo.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhozuprj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghdxnbhnp.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gqsmfiuhj.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gpfutjsgf.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gtorqific.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gablmtsdm.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvsxeakx.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gxosvvovn.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvdgagwu.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gwyhvlvyi.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gibewczai.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/ghagddgoz.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjfyesdm.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/gboldzzag.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/gfofgelwt.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/ghmvnrlrd.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gereknqga.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskgjyrzp.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/geyqfxrwn.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrrptajh.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffwurfhb.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gnjqwzpse.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gttjcrtow.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/giwdxsjsh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gmokvefzn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfmtwriv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gedpamvyj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gncomdhph.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gmamktpsx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gllgnpast.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gspltjwrv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/ghupsphnw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gfysowmia.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvyvqyzo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwftyimx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/grgcxzqvh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gqsjohxsq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjenrted.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/guitlmrkt.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/gxxxlupqh.sHtML

R Bash 专题                             80
来源：http://wap.fanxiaobao.xyz/Article/details/gwcbeinal.sHtML

S C / C++ 专题                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrmporez.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gttmksroy.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmfmvefa.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gvahxtoxb.sHtML

合计                                  2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbprvbbug.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmxvsrmu.sHtML

使用提醒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhfpmzwm.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrncmyxf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/glyqodlxt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fanxiaobao.xyz/Article/details/gsusdvlpp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmouqarhy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjyidamo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fanxiaobao.xyz/Article/details/gyzhwifxj.sHtML

—— 文件结束 ——
来源：http://baike.fanxiaobao.xyz/Article/details/gnslteogh.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqddfjjj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxmrpnrk.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fanxiaobao.xyz/Article/details/grkjwgrgp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/giorgbzhn.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/gaeeibglz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fanxiaobao.xyz/Article/details/gpcnmwxuk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fanxiaobao.xyz/Article/details/gfxidqfuo.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gniwnxtfj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fanxiaobao.xyz/Article/details/gmpyjpvxk.sHtML

【使用说明】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibkedvua.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyqgdtsw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fanxiaobao.xyz/Article/details/glxwlbeax.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fanxiaobao.xyz/Article/details/gbgxkflvu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fanxiaobao.xyz/Article/details/gefngutui.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fanxiaobao.xyz/Article/details/ghovfkejp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fanxiaobao.xyz/Article/details/graoqirtz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fanxiaobao.xyz/Article/details/gbckdndhh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuntlugd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fanxiaobao.xyz/Article/details/glxqutjta.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrjfsseu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fanxiaobao.xyz/Article/details/gnywhlhei.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsmcbjwc.sHtML

【文件统计】
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrftjuff.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fanxiaobao.xyz/Article/details/ghqgjeynx.sHtML


<!-- 参考信息 -->