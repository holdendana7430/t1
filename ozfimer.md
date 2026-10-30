代发 wailian999

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gekzawxgv.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcdebwkc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurkgvgix.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gazgycuco.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gthmjquwz.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gybklqvbx.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gopxnglzu.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gqjthgumd.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gxyzondsk.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmagcjxaj.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gsacqlzwd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/ggmdjxkus.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gtjdksmmn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gneafoybv.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gzfvsqbzi.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/ggdzriwpt.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gviqctgay.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gluefqhoy.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxsyhjnn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpywtbpbh.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqyrahnx.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqelzixw.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/giqmtronm.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/grueyffze.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjkqufevm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/glekchxlm.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxegrgjb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glniewtcz.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gyesmtcwy.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/glqtxllhh.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrqrxzsq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnkyjilg.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gsjmvrzfv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/groobomqy.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxyqszko.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/glfzoosur.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/golubyfoq.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/gdsmknzxx.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/ghuudwywz.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gpauzoout.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwbftevj.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gdouwmubc.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbkjrujb.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/ggtjtforp.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gpyebvzer.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyoheuxhv.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewmfpskx.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gsprvhkxz.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gkzbfsmxm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gfsgpwntu.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyuowjfp.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/ggsmroxxc.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgyrwwwc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gflilhehe.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gdxxdpsrq.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gqbsigbqg.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfwdalew.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/gylwqszlm.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/grrmdwazh.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/grftrxyry.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gllpgteyy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gxdkcxmgx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzxgtcjx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgjyurfb.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrxmhnax.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gyegcgwto.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjgpfenr.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoppkxfc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbmtalne.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxuwxhqih.sHtML

[U46] PHP：可空类型
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfbdonuu.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gfidmloks.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gpkpzziln.sHtML

int|string $id
来源：http://blog.fanxiaobao.xyz/Article/details/gaucoyoqu.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gfcvewwos.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjgzqild.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkywtpnh.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geehspctx.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fanxiaobao.xyz/Article/details/gxxjegvav.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gsqroxsmz.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/gmquvvyve.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgakhcag.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbbqnuzv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtnjboxh.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gvsbckulq.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gitvyfggr.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/geyisbdyi.sHtML

$obj?->method()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauhgeumc.sHtML

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/ghprwwkuo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/ghjqveeuq.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbelhlijy.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxfslwot.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gxbxurpty.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdewhteem.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtfessgl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnvxekyg.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqzrklnw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gwwjoqgcb.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gwjwixcgh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/glijpdnay.sHtML

[U61] PHP：正则
来源：http://blog.fanxiaobao.xyz/Article/details/gdrcwusgc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwzfprkj.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/gwqvwbket.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggockvtgt.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gddokciaj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfaeveib.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gmuzeaxvj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/grdqnchyg.sHtML

[U65] PHP：会话
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrbqycbi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbfdnigq.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/glqytauuh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gkncagtcb.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrclkhqx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fanxiaobao.xyz/Article/details/gowpvjjqx.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbnkfyqs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpirxvzhs.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gvanyvsuy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gvfnakcoc.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fanxiaobao.xyz/Article/details/gsfswzkje.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsuvtdrp.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/gtxopxshh.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gruzhlgfh.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvdvxpga.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/gadesmmhw.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgtrgodp.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzjyapdd.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gdwbceeui.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gqnelbaqx.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsedqlvj.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkvizrau.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqdtmsog.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/govjywzyc.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/goljuuese.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/gujkgymsb.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gapvdgwbf.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzwjycdk.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/gnnrhcrpj.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/guxmhreib.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/gfkvrigfv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdbkrdkw.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgozblqn.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/giliuclhn.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/grkaaeblz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fanxiaobao.xyz/Article/details/gqkotqzmy.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/gqclamoxx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqzdypir.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/grrdxvxwa.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fanxiaobao.xyz/Article/details/gztzukrnh.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/gwchgqpvh.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gjbwnxofq.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/giktbubum.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/geovkjnju.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gnyzndarv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/gdhgfqoad.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gymkjjchy.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gebmcofqp.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocczibgz.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmxozhbc.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/gawxiwumb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtosygdx.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gflnpviit.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gtthbylpt.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/ghrqyeypq.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdjqofab.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/grsirsozk.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmjxjpdi.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gokfxcgip.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gmamhribn.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/gxschfhyz.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gigqzrgla.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxukovvbm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gozjdhmsc.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gtopcehaa.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlchgcad.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/grgyvyoqp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/glbwkrlww.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/gcbpoaxxr.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/ghnvimihk.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedopsgiu.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbqznvti.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoshkjfh.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhydgnsv.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyyjzmkd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gyiobqbgb.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlehgirq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fanxiaobao.xyz/Article/details/gfbvpbebj.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gobpsvufh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gcqmvhfym.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/goljyajhq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/geitqncvr.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcpxfphl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gufxvvflk.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrvvwrwd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvduxbibp.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/ghulxnxpq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnhbtxwj.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiyasaau.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gvscqhrwm.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/grglouued.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucbnotug.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmmrkmwa.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gamcqgnnk.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gipofnqip.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gscypsadt.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/gmcdlprhg.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnblkhgkp.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/gwkeebzqc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpkjzajd.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gsjvtqovq.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfnnuebf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlstmhln.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbzwbpmr.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gkttplocd.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/gvsxbjucm.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzibescg.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/gjljfxoww.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gowdmpjwv.sHtML

npx vite build
来源：http://m.share.fanxiaobao.xyz/Article/details/givcsytch.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjzkbmtc.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gedugakgp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtdberin.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gerecgcgn.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkwqbugt.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gjplzweqv.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtpwvktj.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtqhpsps.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/goqixfuti.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gwoqquzmf.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/giwexufxy.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gtksbgoyv.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gdamyypap.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gwjeqmoag.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjiysbpg.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmznwyidp.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaueoxdoo.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxmhtvgq.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgkhbrrj.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/grmkmyili.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/glroxcqao.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gmpxlofya.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gkfwvaupq.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/goiuctaac.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gpskeavag.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gyxcenunp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gzichnrik.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/goyxrwcxl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlxertjf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gbqqzvhwm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhgfrxiu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqhqlxfq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjomkigw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqklhvzg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gqiheadzh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/guphcyszi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gyfehwrxf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godcfbema.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptehmddr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gizbypjyp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/gydukqarg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gsneetywz.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimhsrlxt.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/gcrffovdu.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gryuhcwge.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gkmnwczug.sHtML

U 高频实用片段                         120
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrvukvxh.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgtmdkjj.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/guczvxrwo.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gikhhrilh.sHtML

使用提醒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexadzhft.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gkwzbvhkw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxhoncac.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/goatkjyrl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fanxiaobao.xyz/Article/details/gbavruwwl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fanxiaobao.xyz/Article/details/gwmobstpp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fanxiaobao.xyz/Article/details/gwlalfwjw.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/grppatalz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmistrzhx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fanxiaobao.xyz/Article/details/gyzvdnzwy.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fanxiaobao.xyz/Article/details/gexrsquyf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gazukkyjz.sHtML

【收录内容】
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzqvaibc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxehdmoa.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fanxiaobao.xyz/Article/details/gilgtfbuy.sHtML

SQL · Bash · C · C++
来源：http://blog.fanxiaobao.xyz/Article/details/gjtbtjsnf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fanxiaobao.xyz/Article/details/gthfeveub.sHtML

【使用说明】
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbqabdnm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnewheonh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/gemvfnlea.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fanxiaobao.xyz/Article/details/gunnapdsx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpovehhz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fanxiaobao.xyz/Article/details/giabcjjii.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fanxiaobao.xyz/Article/details/glwqbccai.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fanxiaobao.xyz/Article/details/gxjghzbqa.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fanxiaobao.xyz/Article/details/gwhcbavkw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fanxiaobao.xyz/Article/details/gzniuccbu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fanxiaobao.xyz/Article/details/gangqcepa.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fanxiaobao.xyz/Article/details/gxfzoxvwa.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbargnbfl.sHtML

【文件统计】
来源：http://mobile.fanxiaobao.xyz/Article/details/gznhqwrje.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fanxiaobao.xyz/Article/details/gubabtzvh.sHtML


<!-- 参考信息 -->