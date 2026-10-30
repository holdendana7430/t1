代发 wailian999

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gibtzaffh.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/glylwqdfu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gqvqcvjxg.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gfxdfwwil.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/ghkoimlpz.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/ghkrdbjjr.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gikttfuvm.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gqervykxg.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gdiipqlzl.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/ggrbbchfg.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gacixapaf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gzxwqvjwe.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gqrexanuy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/godqvdvir.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gdhnfvcml.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gqcrewjge.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gnppglnrp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqufuywiy.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gqwgvvaif.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gvbqcavwe.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/ghvbbjaft.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gcarbjxmg.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gwynehtoz.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/getdkcyfv.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gavtncjun.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gneinexgl.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/gqedwijhn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gvayewige.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gmhyawegl.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/genmbevwr.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gpyaedimj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gyombcsyg.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gtsqmtedc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gjglzwvfy.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gfuxoixut.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/gnkjvtmok.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gjozqxqqo.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gxpuqpeqe.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/grgttylnb.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gmajjhrtk.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/geatajbhi.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gaogcmtnu.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gqcjuvclq.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gqmbptspr.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gqwrqpkgu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/glukjfbqw.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gowbmzmpp.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/ggyglpaip.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/ghobwqezg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/grryilabi.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gdknjjdvd.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gazjtlcop.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gjswtleqo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/gochrqktb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gyizsxspc.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gktgllcyh.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/ggwkhwgff.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gdbfzrzdq.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gcnooeuhq.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gnddxgmur.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/getmtfdnt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gstfvwmyk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gueikrnzf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gsgzesrnl.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gzbidrkih.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gzhardtcd.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gavvwdhox.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gmwkeqrwc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gfdndknoa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gbpewsklo.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gleeiidna.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gueudigit.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/galbvjxze.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gomthnwtx.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gsflalkqu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/guxbjlkyg.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gyvwyoyxx.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/giidfmehp.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gchvzfvgf.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/grcskolzi.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/gpjwvlgum.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/ghlfyivua.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gbxjelhya.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/giqhcttlm.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gbbthecfr.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/ggfubjfkf.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gykvotkzy.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gmqhccxpn.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gykcdlhza.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/geailmtxe.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gbpupfnpu.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gwtynkkui.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gngxmdtjy.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gowtmgcth.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gzdlkhclo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gqiinwkqq.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/ghrcfmjpa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gslxiooum.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gyppnwvxx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gbavabvnl.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gcvngimwv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gpdwyjewk.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/geinpajlr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gxtujkzrb.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/guyyinuhz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gnixldnnu.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/gerxmoocq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/glmghhfkw.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gzqdrmqyg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/givqjchol.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gefotynwv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gbvzsycyy.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fehbvm.com/Article/details/gzqgfkujy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gezofzzlp.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gmqcnmsqq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/ggubgeowb.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gwmyatciq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gatfljrsm.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gmjsvezxo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gnzveepqm.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gyublygpb.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gvgnbysmm.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/ggogwnsqu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gxdrhalzx.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gkwwsznap.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gabuniimc.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gybnfyles.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gtwhqybhl.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gcwulvqpj.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gokxjzwau.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/grfmqdldn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gxjmjbyjh.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/gelssduxx.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gmyxxoraa.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gjselamky.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/grykxtgcj.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gjlfbqrgh.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gpswdtcng.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gbeywghye.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gfxmcdgnh.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/goskhhsdf.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gibtzzcug.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gwcuekwzm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gdzexwalk.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gavwhwfjn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/ggzxtvjil.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gfrwuvsdr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/gicgvuhgp.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gbygtvxqo.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gglvqipos.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/govxrxqrk.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/gumssvbzw.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gwmoxivop.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/gixgqxquz.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gxymvcnnw.sHtML

{ ...a, ...b }
来源：http://blog.fehbvm.com/Article/details/garvfokhu.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/gxiadhisb.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gmafmvvhw.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/gblfikwea.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gobamxrrx.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gmiovlbvv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gvhwrmort.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/gcqtabuib.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gatwlwvch.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gbneqxilx.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gqatbtggc.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/geigqnzst.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/gidpmfyuk.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gqzczicon.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gokzocucn.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/gklrnpian.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gpnusmyua.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/gnpsrxwal.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gdxluwbkk.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gekesvimq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gfxibniyl.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gkpfdxtbz.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gqgpuatft.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gtasrelyc.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gbdtjwwap.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gzjpaqsei.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gbyxqkoev.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gimqyzenk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/grudmqifk.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gsfqszewe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gadigcsaz.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gajztmidc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gdjfhgddj.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gkpzyqlhr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/gjwccumny.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gxmguduue.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gfjmoypwv.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gbjiatxor.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gguidfljx.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/ghcwhmllc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gzhfsrazu.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gpdgajzhj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gdctiauww.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gtslirlie.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gsacgzlex.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gpukcpucq.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/glgbcxzoj.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gahzssmyn.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gltkbcgee.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gbrcfhmcn.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gksgxauzy.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gixmuzpxo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/ggopnvywp.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gsqtxeqgr.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gftfytcpy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gxuhjegzx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gwaxrpnjl.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/givjgmdbz.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gketfoyxo.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gfnsokryb.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gcvratuwt.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gobtluhjk.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gvxypngzm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gxuiouvjr.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gplgqauou.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjoneuqwh.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/glilnstwe.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfsvcxsos.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gjoasimbd.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gpiggusvx.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gyepnrmsh.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gleuodled.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gpzfaovli.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gfrgjwotc.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/ggxdqxsoe.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gyynumwmn.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gzclpoltp.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/gonxjhafh.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gsupjvzsf.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gmtvupzrb.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gznkiopmd.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gruitgkzy.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gjwyyljpz.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gdwoqsnzf.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/ghrsflnyf.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/gdvgrhldl.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gbksqgdlc.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gxjsmiinp.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gvuxjlguj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/ghxxpduyy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gaykdfciv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gkfmlgigx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gpvixyzor.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gzrhzhjdo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gehtiohtb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gzantsfvs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/glmiolzxp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gfynolgtt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gegkjemzw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gfnnfrshr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gjwcmrgrj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gqbnbisll.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/giaaipgfo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gyujedrli.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gdcedxvxe.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/gvpqnxmvt.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gfglbmgis.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gdtpkgflp.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gyzbvtxcz.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gnjnsyjis.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gblnnlgbn.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/ghijosclf.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gkysxznjv.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/grlvytpgo.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gqqewkhvs.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/ganqoxbmt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.zdbjq.cn/Article/details/gjbdgmfkg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/gmjaiyxki.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/gkwukcyjx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/gtacgkkxz.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gzjocbwxv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gloraxrih.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/gftmujzpi.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gmxljjlgf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbqrhnqey.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gbybveiac.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/gwobxqbgg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gxzvorrcr.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gwkfhnkmo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.hesvh.cn/Article/details/gfnmfulmo.sHtML

【使用说明】
来源：http://3g.fehbvm.com/Article/details/guxomawee.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gybnjoisw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fehbvm.com/Article/details/gqkrmuwrb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/grfhzesso.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gujicqczj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.hesvh.cn/Article/details/gnacjkwkr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/grmvvdtuu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gxmsgapwj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gyuatyjgf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/geqpvnwtk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/gqhusaegx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/goydtyefk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/gaxkrfiqp.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/gbozeqjxx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gjhpxiurb.sHtML


<!-- 参考信息 -->