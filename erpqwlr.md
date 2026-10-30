代发 wailian999

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gcljtaeqm.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/ghruqvdro.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gfpdzrmuu.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gcpcaytww.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gnwubajut.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gttqbpfmj.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gbpwyknwl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gbocxfxfm.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gwhnbbsop.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gxgcoxrtj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gowfbjfku.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gpwdvnkla.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gjzweezac.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gxwymdmrh.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gemhzpemn.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gdvuusngg.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gxhvmxwtw.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gkecgkdyp.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gqdbykbqs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gdllghupu.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gdjgamlaj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gsiiurvuc.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/ggswmndul.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/guusbyira.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gcnezatdx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gtmylofoa.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gmygoiemt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/geskfolbi.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gxtpnpffe.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gordbyqve.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gjdsxolzr.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gmbovujao.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gsdnhbadw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/gjwdhzcmu.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gmffoxndj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/ghxquakgh.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gcmcgvhpn.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gvfkzlvqm.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gpxhzbvuq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/gkgcspkkp.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gozenzayo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gapfimyqt.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/giqttvesf.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gsrjekhbl.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gitrirtok.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gvpgsamwf.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gimlgfath.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gcbhckhgy.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gweoialty.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/gceclwyjq.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gklyefrcm.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/glsaxibmx.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gciqgozhi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gtjpkvggx.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gydbscejc.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/gafomuvzd.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gzxrkfeiu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gotenhrgz.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gozgzqymn.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gprqjafzo.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gliofuhpj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gmfxccogg.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gbiiyhzos.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gbexcohvl.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gbyvtkodi.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gxkfbyxhz.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gwdjkbmgi.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gpiyrdarr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/ghbhxadee.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gvhukvdmh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gimctfevb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gttgvvsza.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/grvmgzppj.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/ganlpwhyp.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gdnmcpmju.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gfpuifpbd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gmryngbgg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gvvhjajmr.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gptgrofaj.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/gotwcgzgj.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gzxviplki.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gdpjchjsq.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/gwwyfkpdl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gtrexkaxn.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/getpjfdao.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gxzthqtwl.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/ggzqhhajs.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gxsmslcwb.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gtdjcfeju.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gydkikcmm.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/grjgfzqmk.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gdqatwigj.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/gojybtqbe.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/glfxpozbh.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/ghsrdrvsm.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/gxcatvwtc.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gajeqsnwl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gkingnuat.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gemjstupv.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gshdzlods.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gmqfulnel.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gnhwlxpjn.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gogasafob.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gejvkccfw.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/godqtufwf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gvzbkxrny.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gatmfisxu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gfiqkwpbv.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/guigabplh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gnphxxkth.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gdvznsusy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gacwkgsto.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gbxcwqqae.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gnbvrpayl.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gvhrtrcye.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/gpiesdasb.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gdzvfytjp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gsffxprig.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gmvgrgtmg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gknkgbshb.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/grzwgrxzl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/giqmdpben.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gonqcrsgs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gvnknpyts.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fehbvm.com/Article/details/gnfzsvetz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gzhdncbrp.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gxsvyfais.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gonaovdlk.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gzuqgitfi.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gedkukcjk.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gfyhtfnvk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gnzkzfsqj.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gklrvjfcc.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gxaortxsp.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gkfiigdbf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/giwnrdqbi.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gzmlgzsxl.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gexhxgkbv.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/gugqumdrk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gfahmnzjk.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gdhxfuuny.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/gtckpkfzx.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gpdyexepu.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gwejrilvl.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/ghkszheki.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/goshbuyyc.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gfyofgaim.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/guyldusum.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/glfswrntt.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/ggkegllxc.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/garwblmqi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/ggrvupcyd.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/goegyxtbf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gsgxhxewm.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gpugykksf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gewlnkpts.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/gjfxaxagd.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/glucqvcuy.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/goaoonoas.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gjkegutak.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gdihonppp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gawvinceb.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gfqvotzvs.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/gsktzsozb.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/grocdhmui.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gexbbpgyg.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gwchfrwmf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gaszpxazs.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gcdznscvc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gufckgluh.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gfqobjfbn.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gqrwdleof.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gotorkoxz.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gasjewydo.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/ghtvljnze.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gczakjsrd.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/galxejegs.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gvcrxczfx.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gexzdzytb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gtruaovhm.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gkwdznvjs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gpsgiukmm.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gjvgevlcq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gynunjnlp.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/gkgjbrxhp.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gzivkykxw.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/gpqjxgvcq.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gbjcgeygv.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gfxyhlmqj.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gclciceaf.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gxjjdfwpa.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gibttrgnt.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gimyohrub.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gqfizmrxx.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gcwqlqxfr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/guaqockhp.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gcwmxelbu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/ghwdsdyfo.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gnltnjsdi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/grsgxzcaf.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gekjgczjr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gjcxfbxys.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/glkpoyibc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gfuukavuu.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/grrhdqucn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gmadiqcmd.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gmyometzk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gdsunvtgx.sHtML

[U111] JS：对象转 Map
来源：http://read.share.zdbjq.cn/Article/details/geujjkxle.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gfzezbimb.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gvlqizjrb.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/giiwpqjqw.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gkmpnmeqk.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gimvuamyi.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/ghizwxfca.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gningcgjj.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gfkrrxwum.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gvrdlpkop.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/ghzftsujd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gcxvjvrwd.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gsrnzyqss.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gixxznhee.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gnlyreeyi.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/ggsgqbmkb.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gojvynnob.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gcporuhko.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/ggmweymea.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/giuvjtlsb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glbigguwo.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gblsffdsb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grmqxkncx.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gdccjdsug.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gqyxdnaoe.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gddtoqdxg.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gfcdoqxoi.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/gozkvczdv.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gdaoxbtxy.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gbcvgwgaf.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/geaeppckv.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gdeogyngz.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gcxnqdkvc.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/gpfpfgiph.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gzyyouung.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gjmytdchx.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/gqlmkvvlx.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/grcogucxc.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gavqadylf.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gasytbhwc.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gqjacsttd.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gskrdkqiq.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/ggtgozamn.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/geykbalez.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gqlnygebc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gwxsvfzsw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gnbfujplx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gbgfevkac.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/ghazycoro.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gpzggvigj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gxgvkupfb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gxapcikiq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gqresmbfl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/guglqhwwr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gcrfbddum.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/geqbvbbwb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gqieqsnzj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gonlucwkp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gidladelb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gswjezkgy.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/genlchubo.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/gsuxybapp.sHtML

S C / C++ 专题                          60
来源：http://mobile.hesvh.cn/Article/details/gucwddxuy.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/gibxxtveq.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gqpwywiro.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gxddekcsb.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gemrgmbzk.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gmhowepwn.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/geqhrwihj.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gmllfrsec.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gfqidttao.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.hesvh.cn/Article/details/gebogkmkq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/gksnixcyj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/gqrmklymi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gpcldaasq.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gsvymqmmx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnvhtsrtw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/ghsgjvzcs.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/gxifqqphd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdcmozqmo.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gecmdiyra.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gfwoxwetg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/grkdpgmqv.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/gbtkjgqyr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/gqksgigfy.sHtML

【使用说明】
来源：http://www.share.zdbjq.cn/Article/details/gytdcgtkn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/gxmebzvlh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/ghjpcqrcu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.zdbjq.cn/Article/details/gqiglvrio.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/gicmecoly.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gfexslxlg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/glpxgbbfa.sHtML


<!-- 参考信息 -->