代发 wailian999

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gjwwcmrrz.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gvbhctttq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gqpehpdcf.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gsexqynhm.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gpszeevnt.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gtkaswklx.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gznabdtbd.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gzfoklbky.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gcwpuibmv.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gsmqqecfk.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gnjxhdezp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gcsobcenk.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gtfrstszx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/ghssoyozo.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/grtgcfdty.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gnarzwcbn.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gdohvnwkd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/gjabrecto.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/ggqxdikbj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gsfazroca.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gxscjxwdq.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gugawefbv.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gjlrugllj.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/ghbbepotw.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gqfpltwyt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gufykdrjo.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gogyahxmu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gpomwwfua.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gyxloxitk.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gftlruhkl.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/guouuzpiv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gghtpltrl.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gorjaqrxb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gviixzqnz.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gpcjnyzop.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gcqohohqe.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gepzfpzdf.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gxakhtpyf.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gcnkidpun.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gkojyzgrc.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gxwfdudhw.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gbcplzuxk.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gbhqaxxbk.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gnmtqyapg.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gexbzmtst.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/ghmlbbern.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gvjxxlwxr.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gwcznuozs.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gqltlnvtl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/ghzctmfvx.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gbxqvewgv.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gwjsjweve.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gfcgdowxz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gqipyziop.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/gqixqsycd.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gzuzzntfe.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gaggndtxh.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/gbdbbslfn.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gnkjmeadx.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gscfzwlex.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gogweghhg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gmbtpnklw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gplsjlfij.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/grgxtpnxr.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gjrepizcq.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gyxsuthzk.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gxxwviaxz.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gtqlzxnox.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gfoenygwa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gcsbdysde.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gjsxeymvt.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gcfhvovqs.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/gwmxkhxlx.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/gqtofznjy.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gyellmrtk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gwmekpbio.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/grtszlygn.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gdmlutyoi.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/goyyyyrfm.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gvsriubfl.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gqaoenupd.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gxrlrmamx.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gpdaxhxgm.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gtailrsqj.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/gqajinhdn.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gkeczeufk.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gslcqystq.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/gxppfyukt.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/glsqqkkcm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gruenrcrw.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gwevczjjz.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gwqtrethr.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/grjetrrym.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gebtewbwj.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gbzhcbanw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gxdbsqkup.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/gcqbhqsbu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gbitykinh.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/gqhjjfrre.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gkxcbxqvb.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gibkrvurz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gzbxvfqjb.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/grwyhddni.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gvmrprgbv.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/glalsotpj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gzvupnled.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gfmbmrwpw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gtsknlrxz.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gxblzuckw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gjnhfyxmv.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gvihfxgsh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gvgqanwpj.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gkxfcihce.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gwvuhgdzn.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/gpfzoaclp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gxrwmtmjw.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gpyjchflm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gctozglis.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gowkgebco.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gfkrqlswp.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/godaswbry.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/glamrihmr.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gkwongzxc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gfojxdfwu.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/gqehqzhbs.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/gmhqdwudb.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gkcnzloxh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/ggxrumhll.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gmpuqcogf.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/gsiqvspnr.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gjobuiqcl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gvfteqbhm.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gfwvqyjzw.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/gridaagqx.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gfqbeappa.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gjkehruhv.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gpertfmlc.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gusstoguh.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gabxqsoft.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/ggtmwwhbg.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gblonczpo.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gogrhiiar.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gssbjfyri.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/grglvfsgl.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gydawjjig.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gomulqtah.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/grrwsxpih.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gukklrsgd.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gxcfsgslx.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gujmnpreb.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gebgtenas.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gyxrjsplt.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gdsulzfxr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/gxitlppbo.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gzdcskkpv.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gbrzorsfc.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/glfezcglr.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gnkmvwrvb.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gizsydjjf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gwayvbghr.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gxplzzyop.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gyhnvpcig.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gcwvscvii.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gdlclqkfg.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/grljhndrj.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/ggoktpmop.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gctvdojem.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gplhimgua.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gzganfbxh.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gjazaogic.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gawwnvsxk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gjicfliuc.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/giggluxiz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gcvnzdqbs.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gatgnfxce.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gwzoiskhr.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gpjelwddk.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gaiutuknn.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gbqjfnbxg.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gdfafauhc.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/grgbgdlug.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gsnynmeui.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gdwofiwew.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/goqzqvikk.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gvcltxxgx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/ghglmlynu.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gwihczxsp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gmqnzrbnm.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gimyqgzxz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gcivcahpl.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gpahawvfs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gpezxtugd.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gbnxvakct.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gsmrenbqi.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gqhxtvztt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gtucwidkh.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gnvnquqaq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gqpqnxptt.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/grpwkmxvj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gqfxpkrlu.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gqftpbmue.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gpdvnoktj.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/gdwewdhny.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/geeihdnyq.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/givqggcfo.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gisxavsxz.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gstcigblk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gbuvtsrmo.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gjlqoenzl.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gbrcxjtlk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/giubkwbtp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/geaimxzir.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/grfvbaxsm.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/guylrqqgo.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gsomprnnc.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gmoxxnony.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gvvomghlb.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gndueujfh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gfzsxrtzz.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/gyjgnsqvz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gudsdvhoa.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gjhbagobt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxvtgpkqw.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/ggsocegkg.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gquirhseb.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/giyewnbbx.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gdmlnoidl.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gmlpcfqns.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gaemynbxj.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/grsdawefs.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gmpwoqnxe.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gzphqllop.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gmotdexcp.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/gfjivewqb.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gmyrfuhgn.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gjlmajzmm.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gmcdybuvg.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gvdstmifq.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gdrgbzldb.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gjexukkkf.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gjkaiduvg.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/guhhugdog.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/guwqmhlgy.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gewqblwfw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gyytrword.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gdqivqnrx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gsyhoylkj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/ggdnxdrae.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gdovgbtzs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gvetvljfv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gqnuqesws.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gyegykmgf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gjpxjjxmr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/ggyjwfekp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gshzbdqfo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gvrzzihpk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/ghgshsdzk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gqfdbexdh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gdhzpmjvl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gdvbqfljm.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/gbfjpdtnt.sHtML

R Bash 专题                             80
来源：http://www.share.zdbjq.cn/Article/details/gqrnxpqec.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/gnkayworz.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fehbvm.com/Article/details/gbydflzpo.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/glfjhzqxv.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gsaemwmfh.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gdkjcvloy.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gqzagqwqk.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/gaelwjoxc.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gqpdhkooi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/gdwzmjpxq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/gihtmnwdg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/grjgfmhsa.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/guhmudyra.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.zdbjq.cn/Article/details/gmnnybwhz.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gfdyuvdzd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gaugcfsfq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/ghchiuqdv.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/geebazwtl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqeoaxwnn.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/gccljdcgf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/gzcujiovc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/glylounuk.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gfjxfimja.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gzekslgcn.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/gcflymjiy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gzsfvudih.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/gnobvrdwi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gtxlnistq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fehbvm.com/Article/details/gwpuetgem.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fehbvm.com/Article/details/guelxhzve.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fehbvm.com/Article/details/gcedldwnc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gvecfweid.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fehbvm.com/Article/details/gxjmzldmy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fehbvm.com/Article/details/gdoqblrqr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.zdbjq.cn/Article/details/ghcxfclbm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/gnaekizxv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gmumvpgjv.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/gyhvrgxnc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gxjkxxhjh.sHtML


<!-- 参考信息 -->