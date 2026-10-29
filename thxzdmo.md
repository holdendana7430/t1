代发 wailian999

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gqcavunbb.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gtckzcxpa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gcreoxyxv.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gdxhwtqnh.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gkgnichav.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gdsecftog.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gdxppzrgo.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gcnzrfnmp.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/glmevtwvf.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gjddequis.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gyottodsz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/giardsyae.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gcnisgkap.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gtxwxwsns.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gjfioyscf.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gztzdgbwv.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/gekrngkej.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/ghgkkbqku.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gioshhsjl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gcqsmgnvm.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gjeyzxjmw.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/ggopoaphi.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gxrfzqqtg.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/gtdefjxam.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gcydfjybh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gckexyzwp.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gyaxmtido.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gfdrbxyvb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gvxbkabhn.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gzhfksjzo.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gtolexhkw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gomjwodyt.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/geaxpgmgi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/glwntzsdf.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gkidivzdb.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gihfeeirt.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/ghkzthxzi.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/grpkqvhzb.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/glaxzfznp.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gvahtrpqe.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gytziazxa.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gaewdgbro.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gzmgpfgkx.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/grcfepwls.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gikiaxitj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gmlqthigt.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gedopsooo.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/ggbnovjrq.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/ggvxayomo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gjftueqps.sHtML

[U36] Py：定时任务
来源：http://3g.hesvh.cn/Article/details/gqiydvhjn.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gntzeomsq.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/guodmzxew.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gfnzdxvzb.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gvqwgyynu.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/grgwmltme.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/gzzmnlqkl.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gylaimzzt.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gzvnuiqef.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gwgjdqjja.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gbulvmfvj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gvjliotna.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gsqofydxt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gmjlitdux.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gscbchblb.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gqkiiqrxb.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/guiusxiuo.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gvahzbuxy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gzpfdfglu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gqosfxxwm.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/glrgucaaj.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gjffzvxqd.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gzydavqbw.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/gjhdsosxq.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gcgtuazfn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gprsvuoce.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gjofewdgr.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gyctkvhst.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gkkvagdbn.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gfszjctkr.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/ggovghkfz.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/goxfyfcdu.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gegqdtpux.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/ghwsxdbvj.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gycrsnztb.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gjjtvjwlq.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gmbyzxocy.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gjzpjrxcf.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gweyrtpeo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gdcishapg.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gjnluybat.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/grsckkuwx.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gtggtxcll.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gfexqzata.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gdveqcpat.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gxmyazoja.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/ghapikwry.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gqfiwirrt.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gcwlkicpw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gadccazzq.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gmxawikud.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/ggrlxnphj.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/geilmkcwd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gccojfysy.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gdecjwnvx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gzzuiqdct.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/gakehiihb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/glsdsnnjn.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gbndqunlx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gquwqrwxd.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/grmdoxgaw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/ggapvatmt.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gxzckfrbp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gjtizwqye.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gywhwarmg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gftjurfna.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gsazgsove.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gydhgdroj.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.hesvh.cn/Article/details/gskzkdvcj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gjerkghnr.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gtbeqwsip.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/ghbjolbzx.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/ggqdnysom.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/govcwqwib.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gilmqgrer.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gayteydgs.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gttjxyuvz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/gqxaoenxx.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gyhnawtdw.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/ggrljyjpd.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gdlpdonxl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gsametjvi.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gciwakxdq.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gvdbozcxn.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gmhwgwcpa.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/ghlersznx.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gewasjeph.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/gvtiozqbt.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gqhfvneah.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gqegyppys.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/gxhhydeko.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gbdcucarr.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gpfxcaofw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/gbetpgrdp.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gissxolac.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gyeopzxro.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gzmpthpmd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gmwykqwbw.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/grazmqlfy.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gzvivevwz.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gxiyqrned.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/gzoxihqph.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/ghhpvxjqc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gyuwhymqs.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gfrawcqoz.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gtlrmbkkx.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gtjtbgjnx.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gllucuogx.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/gyxiqbmqm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gqmgkgbfg.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gabaqokhr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gblluhxkm.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gtckoitec.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gpglofmek.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gkssyavtk.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gadksrxhx.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gdwudpmag.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gmzopfndr.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gizwsbdov.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gnwvgruxb.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gpperivim.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gfrjuawqq.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gevckcelj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gercehnzr.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gckhqfmbu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/ggkqubclt.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/gthniqore.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gceczkfkk.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gfabgdopc.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gkyyuhrfl.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gqweexkst.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gdctegptj.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/gcigcuzve.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/giyovjetu.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gvuapovir.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/grabksejq.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/ggwnhhllo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gghlolyqk.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gnodckkyy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gpcpfwqlu.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gnmltuykg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gjyjlqvaa.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gxnxdazbg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/gmomsvjio.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gwchgotut.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/ggdrhbice.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gbuxstwko.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gfgnapljz.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gcfnyogkr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gqjurmbfb.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fehbvm.com/Article/details/ggrqzrklh.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gurzrokhd.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/grsuzpwbv.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/ggkjoarzl.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gurgxtefv.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gpjrubqgn.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gntnvqkoy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/geuxooeyi.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gjtrrritp.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gmcigzsah.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gvzjowjsp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gdxokrzxe.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/glqmtynps.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gntgpdcmb.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gurasrded.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/grpvwsayu.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gjhitikco.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gievutgqd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/guphbsusi.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gqpxbpxef.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gypvjtlwz.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/goskyghbc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxtqkelox.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gmftsmvhp.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gigmwmotd.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/gutlnrlen.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/goqxyutaq.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gljuozkkw.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/gjyesovxj.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/ginxssqsm.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gcjttsqix.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gjipyzang.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/geplkgqfr.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/grkhaxerb.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gwpembyur.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gvtlftvrr.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gwfgspnvf.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gxjbecjmk.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gfueihprf.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gwqqtiexg.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/gnzyspzur.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gslscckgg.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/goojkykfh.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/genwlopwj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gholwpgtj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gqbveneke.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gfhilhvob.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gfkpzovkb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gfdlgufxt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gndirveej.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gscpipcnw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gmdazfido.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/glwwntsvv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gqzanvvzw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gvxkmwjnx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gfwsbhyxi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/ggpgkjijs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gefcsybnx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/gorpqdonu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gdcvljwhc.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gjvlflcow.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/glwjelunj.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gujlclfku.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gfawybfcn.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gztpiaubc.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gigpgtjnd.sHtML

合计                                  2106 条
来源：http://blog.zdbjq.cn/Article/details/grcqrdrqo.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gzypnwzli.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/guawvkhvn.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gsnyfiesh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fehbvm.com/Article/details/ganjpfpxz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/gtdtwjlam.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/glftvlznl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gcywwdwoj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gsqluzdrp.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/gkruwtljb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbszpwdmw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/guafkfcje.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/gqtlspwnj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gatarqxcc.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gfbndghac.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gzsjtfool.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gepyknipj.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/gmqrhsjqb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gmqniblzp.sHtML

【使用说明】
来源：http://3g.fehbvm.com/Article/details/geayewnmz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gfclgcgfy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.zdbjq.cn/Article/details/gakqrizsi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/gxkjttwpa.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gfjerioda.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/gygabcvku.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gbcmfjzje.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.hesvh.cn/Article/details/gfvimvwzd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/gqhczzrlb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.zdbjq.cn/Article/details/gvgavbzvv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/gijlnajee.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/gnkuunaht.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/gfyriepkk.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/ghiuuykck.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gvdgosfsk.sHtML


<!-- 参考信息 -->