代发 wailian999

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gkpdobscj.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gasyombay.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gnohpsytq.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gqqcekxna.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/glzcvoreb.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/gfutznbrs.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gviohyikp.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gmqxasegs.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gkroveuzt.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/ghliuowdk.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/glhesecmm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gglsbzlro.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gqssfeyla.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/geafxiisy.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gqfzjglka.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gtblnlhct.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/glmrmdqlu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/gymchlbig.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/gbqyqvsoi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/grlxkejbi.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/ggtqjelak.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gqfbmjhck.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gdmsrttkf.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gitdhakrh.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gtnblvwzm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gohsszfdw.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gjvckiqnw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gpcwqkqou.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gvvqhpwjf.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gkomtblvh.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/ggwpdcmje.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/gmnmqfsiv.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gzzxkgbcv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/ginwzsdtc.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gajxhymjs.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gdgndpxwj.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gzcfxsiep.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gyifzblao.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gcnogspui.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gskklirgc.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gwpyssreo.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gdqianuln.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gmwujpwwh.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gyowakysf.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gaxrgqorz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gnlabjjsk.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gvlbxamjp.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gyqjmiffq.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gzmlrzzly.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gdnnujpzl.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gxqekoigo.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gbtybmrmd.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gxkivfutl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gjauoppda.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gsnvxhiel.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gapkbrxzg.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gjxmrdews.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gwpphphpf.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gjshxnaad.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gnjibdgbd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gbqyxpaxn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gsnqvvkno.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/ghoolgwrk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/ghtiocxiu.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gxkyoydvx.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gaxekbseb.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gpkownhvz.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gzwbxrgip.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gvmccjlbc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gwimwcldt.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gqenqxsic.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/ghklfewsv.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gzdxyxhjz.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gfqsxrswd.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gtuikqlkw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gxiwchdqp.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/guqrfyhoz.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gyftmjium.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gnkafrerl.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/gzmmemloi.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/glduvndmt.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gwxivtfsq.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gfbixvizb.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gbfujtije.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gamypqyaz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gcaznceff.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gbbvxzmju.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gobkijkws.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gzianpyfd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gtldonuqx.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gzpqsjblo.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gthbmftjz.sHtML

[U57] PHP：字符串插值
来源：http://3g.hesvh.cn/Article/details/gidbbjskf.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/ggalnjbbs.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gddaldjqw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gxcobuibb.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gffunpnyc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gjjsntaqh.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gygrxqhdy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gkovsqtyh.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/guknaouhx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gpibtqbci.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gukdjikrn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gkuxucnmu.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gmqfbqify.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gowjbeozl.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gflrgidct.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gktnhgbzp.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/grtlsbdxc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/griugicoi.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gdpionjfh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/ggsqjzrfv.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gzswbdzrd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gqqrhwbbi.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gypbpurjr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gthydbhxp.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gqnvasork.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/guucwyvug.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/gueyrvkkv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gkljfpfko.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gwkdfritg.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/gncehaggt.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gnwxobynp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gygksxvdi.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gaghgzjcu.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gzajgxvfs.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gjtmexcnh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gvkkaybqr.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/goppkdxgx.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gacrvsikm.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gvpiiihrs.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gjwqnynqn.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gsljqxegx.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/gbpawotek.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/gqkmwqcgk.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gbbvaxlry.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gfxdqqqgp.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/grwmcyddv.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gukgpmqae.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gkqjmsvxd.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gtxkeumut.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/ggjwfhdyz.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gvotjibhl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gbptuujxw.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gtollcjkk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gouthtrlx.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gexfnxwbb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gapnxobdp.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gzuccfskm.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gxgikxxwh.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gakkteriv.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gdmbbiaij.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/gbpwqhafh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gvxnzwkyu.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/gwtnnjstq.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gekrhndgn.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/guitnckcu.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/guenozfat.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gfnfbfqav.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/goruwhkwg.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gbejzssth.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gvzqpbzvy.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gzauyihwc.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/glnqzwzow.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gqskmxhil.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/gnrkqfnrg.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gebhkdcpv.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/gjelwjtqy.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gxkahnzvz.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gaubhzeqt.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gpucdbnmi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gxguqcnga.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gszzuqdjd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/grhonockx.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gzzjxeqbi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gyonbqlnn.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gukcviosa.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gzqbsuzpe.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/ggkztddzw.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gcwldoklz.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/glxqfhkio.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/getsezeja.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gwmdtmrqv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/gbsxrthwi.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/ghexbchkk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/ggqrvxjqo.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gtwcdpupv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gdosccupp.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gtelyccmz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/glzflbfbw.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gavisqdni.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gpzosospr.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gabnvvndm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gbjizcumv.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gqsxipcdf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/ghgnxebgw.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gfgnvrjzk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/grrohxosd.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gawhtdgci.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/grphqnhcb.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gnkydxyek.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gkcuecpvt.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gqfnjcnft.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gwvqgpfer.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gpsgrzavm.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gvmpspewe.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gubmlfgcn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/ggyanagiz.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gudmnvclw.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gttaoeggp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/galmaikoj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gglwnteog.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/goikdjzqg.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gdsflkzgo.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gjsjxyzfk.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gfrypcmuj.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gsbucmqtt.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gjuxlnktz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/glcchxzht.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gxwcfyxqg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzojksjas.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/guxjkzkxw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmfcexcjm.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gdbjythmy.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/guvfoatnk.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/gymovrtgz.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/ghhmxsbgq.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/glkaiqref.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gtreqsqim.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gcknrkkmc.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/glnblxkmf.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/gaekvfsje.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gaukxbglr.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gnpoytxks.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/gjtjxbigf.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gxgjptobl.sHtML

Kotlin ......... 15
来源：http://baike.fehbvm.com/Article/details/gvfjyepdm.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gtwtjxexg.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gmzlxrytw.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gsgqtftyw.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gfvhubidj.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gnivaovyq.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/guuxoqsbx.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gvgflfeyp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gmifpwylo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gocgyywfz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/goumobeqq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/galkuhlup.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gzbspedzn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gcboafgfk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/ggkjbrjbd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gkjumbyxu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/goyitktne.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gbjduecca.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gsmkgmtkp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gvjehrbth.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/grjuwnynt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gsflqxvyu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/gdbcyrlag.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gzaflqnfo.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/gvrjmthcg.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/grzbcdumt.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gobrliine.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gwwmpsqeq.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gndffeigt.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/ghdodimdt.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gvybecgpg.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gpvonbjkl.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/glraoikpz.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gnaegnupa.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fehbvm.com/Article/details/gxmgjkhix.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/gksiiczud.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gthjvvuef.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/gvkvaqrqm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gxtmzgbzu.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gvqdcqoaw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzpsrhtvp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/ghfpaegdz.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/ghsnaepsm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggvseigcv.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gnqvemdqx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.hesvh.cn/Article/details/gudrgqgnn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.hesvh.cn/Article/details/gcfsqlmir.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gtuuiyhtz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.hesvh.cn/Article/details/graajbsos.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/guoxaplzh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/gnquqicqg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/gdxlegecq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/ghzatrpii.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gehzssubn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/ghcqakljk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gtlfxztzm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/gndsinsly.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/gmnclqspz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fehbvm.com/Article/details/gczpenrmy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/ghkekupvw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gnmyvzjee.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/gszppnksi.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/gilwtssal.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/gtscafccv.sHtML


<!-- 参考信息 -->