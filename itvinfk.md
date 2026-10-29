代发 wailian999

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gwyspnfyk.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/giqbsyezi.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/goirdyohr.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gebxsvubz.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gupcvwmui.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/glxtoeajx.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gttkertny.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gwafnqkbr.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gxgrlmqqo.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gwookzprl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/ghabfqwwe.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gnfkxqpfu.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gbxspdjny.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/garsejsjh.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gwtcybaic.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gzpldgmil.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/globzoynr.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gjnaopuxx.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gsmvwziwb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gdgpxfteg.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gzdhhbowz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gjxnkungc.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gbhttqxvb.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gxsklsjyg.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gnwlcxgum.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/ghpjayaej.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gqqsuuhxb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gjqrtxlny.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gpmqexiwa.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/ggkftbkno.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gcyhkpnzt.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gjofhmdhj.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/grvnoudyp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gmwrhdkwv.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gtospccpf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gxcuhusje.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gybmagbko.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gscnsuapl.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gvfgxzcci.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gljwimdxs.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gskvwxtft.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/ggtvzscqm.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gihwhbgbi.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/guirogqdo.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/ggprlxneu.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fehbvm.com/Article/details/grcjbwfyq.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gdgknmaxo.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gpcqllamj.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gggbpwsif.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gztwiiraz.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/glgjiqabi.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gdaonqxon.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gqvydalwq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/ghnfhqzte.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gwmtcdbis.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gwedibbtu.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/grslujvcj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/ghisgucga.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gtjzzdsyi.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gkqojozmc.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gchempcho.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gomctgajt.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gchnjtjte.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gkzopuqiq.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gtsxqnfds.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gtrvtleoa.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/goditbbtw.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gulbunnsp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gcgvosbdg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gegmuadhi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gafsbrlxk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gultinldj.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/guvcrpczg.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/gkkifuown.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gamdscfpc.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gtgjgawvs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/grlqluaok.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gveehzwpc.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gkwafoxgy.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gxjrtrwck.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gdxaupreu.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gbiidvbgh.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gllybkwxn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gbztfmrxb.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/gfcwlazkz.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gkvufrivh.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gwnhnhazi.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gtpxvpdkf.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/getwydgtp.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/geowqogkt.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gtjrmtlsq.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gvvjilshv.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gxnjvqkkd.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/ginttgyjq.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gjoenzlrc.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gaufydjyp.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gnrwthoyq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/ggrheuyhl.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gsxsdqxyq.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/guhkdpatt.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gatzvrprd.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gfbpxwmpi.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/glqhfnvce.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gndrpwgqp.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/gnmubwour.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gktngkmwc.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gcvzonnxk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gsacvfmrz.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/gbdkhjtaa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/ggiqqhzml.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/glhyrbjam.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gnjhmifiy.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gpmjemaub.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gvoxlcrqi.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gjzrubacw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/ghdwzcbfs.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/gatjqdhmx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gnxgefxih.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gtlvalpws.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/gdikkbzyp.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/grgzfnupi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/ggjewuquq.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gnshnviof.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/grlggaevb.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gitmztwmo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gcbomacra.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/giwqzpxwv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gqqihnabh.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gysqupelq.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gmdytfjfw.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gdjpbuhzg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gnezssiiq.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/gtnerzfud.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gisajmkfb.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gmjbdzrmh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/glcnxwrvj.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gfmjzfyqp.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gckbgoonz.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gcjcutixm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/giwcxwcmx.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/gmkfcxclz.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gzrdxakvj.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gfekpxhai.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/gdzzkyuyh.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gktnwykfu.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/grgtglwdz.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gylhmisko.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gewwfqdjn.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gcoyhhxpd.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gdlxcdzop.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gjxkhahtd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/gewgjclwq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gemufiyhj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gtmawtfcd.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gpozhkzwv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/gmlshrsgc.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gtahnbgve.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gnfmhoejx.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gaxafbvbh.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gaaxgynyo.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/gbrpfqymm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gctohjrle.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/grtanttpk.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gjbyklcpy.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gpvjinjeu.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gyjqpshoo.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gtaewzurf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gbmhyxilt.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gsydikxpm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gutajsxnd.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gpolpliow.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gmwegyrfa.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gsserexuk.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gyxmytkjz.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gcqciclaz.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gqgmwarxi.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/goflcehtq.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gnppxvncw.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/gnhcspuuq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gaasgzbep.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gxjfmbeeu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/glajmzfta.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gcrorqcxd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gnyjxjksq.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gzyjajprv.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gpdmkysya.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gwzhoilhu.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gjdgnsisl.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/ggyvudrfz.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gruwnwxeo.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gasklxtnd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gegslssnu.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gwsacozht.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gmpfegvwd.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gstbeeydc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gmijxvbzj.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gnmmkkpdd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/gxuiukome.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gilwwgsyy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gwxummozl.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/gmaiunxrp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/glcixlahc.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gqblanjss.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gjbrewhkf.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gckknzogs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gxdphmhpz.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gaeqttivw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/giqrixyvr.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/groheupib.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gpqmdosrj.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/gjezggqmk.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gcasrxkky.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/geaqmiztv.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gozcssczg.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/giwnijfwo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gqdwawzgv.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gvtkavsgw.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gttqkgqvy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gluiaekjz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gafthyobm.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gtiopnxbj.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gyqyenanf.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gzrutwnrn.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/gxhgmhvvp.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/gdxusfqzd.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gvdpezkcp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gkeuxmklb.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gjhogciyp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gastivvhg.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/guliecqao.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvmlsnndu.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/ghaexwnqv.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gdwavxojo.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/giscxqbtz.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gwtdqgzei.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gvcfywxtn.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gcsdhdqcn.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gxnjtpjcb.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/grnfcxvhz.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gctnexmvb.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gthbqkhbh.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gmmtvvrac.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/grqsttfbs.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/gjdutmfvi.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gmfvvkuln.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/ggyksojht.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/ghwrxwqpe.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gerckunwe.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/guglhkpjt.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gwzvaitei.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gqjojkqlt.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/ghmjnldvb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gwpnykied.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gnddvlhty.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gonfmjqvo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gzodabfyi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gsswbkzyx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gkcbqqzns.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/glyxcbzmz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gnbhqezzm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gdhnbkepc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gpmwixqui.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gepwiwjzo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gqobzekun.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gzzfxvdzr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gscwuivdw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gwswoplfm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gjeszjrfq.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gklvjogcu.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gavicntid.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gxkynqdjn.sHtML

T 其他语言补充                          60
来源：http://www.m.share.hesvh.cn/Article/details/gpbzwdmrs.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gcdtoovzc.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gfkuqfbtn.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/genpgmbev.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gfmsjvvks.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/grzvdqfvt.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gjnwzjhhy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gipldqwiz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/gvsbgsrij.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/gnaxgypmi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/ghguaaleq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gyzfpnohw.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/gsqimudpq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gislvgedg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gvydbnjad.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gelzlfpqe.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghcytaqre.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gxwdjkuvi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/gybdmpvnp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gbfjotyuc.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/giioukmri.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/glulngrsw.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gthbgypkw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gqzlpjdyj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gpofadvbi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.zdbjq.cn/Article/details/gvyvkucig.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.zdbjq.cn/Article/details/geeanaemu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/gacqbxhui.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.hesvh.cn/Article/details/gjmlnjvyk.sHtML


<!-- 参考信息 -->