代发 wailian999

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gztlezpms.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/ghqppjwqt.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gxlvtizai.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gklzxzzhn.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gahnqjarw.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gnecygmro.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gqjwwrbil.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gjyhfmogs.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gxymmoluv.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gdqtdhwcj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gdjhvcdnw.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/gftnckwxl.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gechxyvah.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gqocefkjm.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gigonxqai.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gclastouy.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gpqcblyvn.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/goiqervsq.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gkjmtfvmt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gqhblpmen.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gsxfblyiu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gtoobxhqx.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/govuldoqw.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gptyrulek.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gtsdsilqg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/glfkbsfok.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gnlmrowej.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gxwblvlpk.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gedekjbng.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gclckxuzy.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gyomvavni.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/gkdelbgbv.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gabwcrlcd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gtrxrxnxy.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gfcgpeoiu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gzaitonsb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/ghetsfoje.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/grqjlfaan.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gwnldefzr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gujxmzegv.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gwfmswmcc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gutzffhaa.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/glomebeus.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gvhkqvsev.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gktsfdvth.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/glqhiturx.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gibwsayqu.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/gzdexacrt.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gxcrxdomo.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gdvbxxzju.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gphxfdiyk.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gegifzvzr.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/gofrvxtoe.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/ghykkktpx.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gmjyfaaoe.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/geiearbli.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gtkptpfwm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gisxxogqi.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/ghltpqwgc.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gwezzuuad.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gnpsaclmw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gfjlvlpxi.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gyjpqomxg.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gwyldlult.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gskdkjrtl.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gqoswlwee.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gjwsiqsvi.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/godoougkl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gostdfeqt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/ggxajyvjn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/ggbxtfdqx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gimknvccy.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/ghkzjuuev.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gpcjzqcbt.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/glyjcyaqx.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gjfoxolxf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gouwucdac.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gapnwnggv.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gmaukjceo.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/gtyhvrore.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gifqrqpyq.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gttdsmquy.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gffupinpo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/ghrfneuwk.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gghteoylj.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gxrouajuv.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gnqobtfer.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gqqkogzms.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gfwtiujhi.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/geojafoen.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/grbzymrlv.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gilhscnlk.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gfufyecfy.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gqgcvsqqu.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gggiexxuk.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gohyrfkiz.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gfgchpdrg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gojurvcsl.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/gqiqqqjze.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gtimdglrw.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gwohutnib.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/giyxdyylf.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/glspsrilq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gfvfaqvyo.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gsqbngebz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/ggdqzdfxf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gucywiuex.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gjpiidvab.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gqlbxorcq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gkravtpsr.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gjcmtkvwx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/gzxmiwiwj.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gnrhcsxqc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/glizdwdcl.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gxaqtwaco.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/gewycxdrr.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gonizasjs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gaaomwlvp.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gxhevouoy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/gjsouzokc.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/guocbjlxd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gfegpfbtn.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gsillgmxh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gxpuhzzaf.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gsmmcstre.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/gljuticpy.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/ginjodzhk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/gmlcohsva.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gzyxqmnid.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gpjofepbq.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/gsjiqremp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gexxawdss.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/gkzsmmwiv.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gjpfyxflk.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/guvpuqdit.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gilpmqlvz.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gluletqhi.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gpcqaxkyq.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/goixnneib.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gmhatwnyc.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gukwtpcog.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/gweaorukj.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/grvvawybm.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gtfbbjlzk.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gsbplxlhg.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gzfxevoix.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gkfjtazol.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gnrtzgtav.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gdstkrdul.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/guxceglmf.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/ghhnztcfa.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gwymjmrut.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gtwwkdgar.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gyqwatlej.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gridbtxrg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gfrkaqsyy.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gadaactut.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gzmispjea.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/ggwtmehdq.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gaeynrpii.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gbwgtljfn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gsebtoxnx.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gnuhtcjwf.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/glqldfypz.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/gwrslfpye.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gwkierfkn.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gvhqpgpmz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gixzndmjo.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gcegektfn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gnpbkeqxq.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gytkumcek.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gjpkahnzf.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/ghytaaero.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/gvyeztruu.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/grxenemui.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gmkxgpnmw.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gqqqqdpdu.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gaehffest.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gggrbzmfl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gquucggsr.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gwlsjyeti.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gqkuurhsl.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gptgwdvgt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gglvmiiim.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/gyadrxalj.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gspazvymy.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gcutgtugi.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gxpbmcvxn.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gpwypcrmk.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gwngzhoep.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gcsctdanz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/ghspzyibg.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gtenebjcy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gnkzmlfze.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gqnrrsvbk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gnnsnpjni.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/ggzxjaozk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/ghixehzqo.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/goiegyluj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/gkbdnkpek.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/golmodsws.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gikgdtevl.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/goccupupa.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/grwafmejl.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/grpblaxux.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gwiaammha.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gnskwjidm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gbnmeesqo.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gitqhyvgp.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/ggxvediaz.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gtwmjvbpy.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gknofucfp.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gbxspjptm.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/glgmrqmrk.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gycdryvfj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gapnnetag.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gctdsktfi.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gbstltxid.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gwsrszdps.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gyhxlfslk.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/galxvkgta.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gtvqoefjl.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/ggsjhwqvf.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gdommjpkt.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gnsftdytw.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/glvqspsml.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gtkbcpsmn.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gxtbnekgv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gebzetfxe.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/guciicwng.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grldhgytq.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gyjxxdypp.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gcynkizra.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gxmxddmqp.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gbowbtbhu.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gazzvnymg.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/geiyesxyo.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/ginrxueuv.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/ghpiuhfis.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gzddwfwkd.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gospynohp.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gndrjegfi.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gsplmrsmj.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gmuwpfzeh.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gdbcncrab.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/ghevrdram.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gmequqvfi.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gkvlqxhlm.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gwaurtjfe.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gqxyaffeu.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gdrkaayrz.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/galnpsvzu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gthaczgay.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gvgqadlab.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/glhpsusnp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gpskxduzg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/gcmuzggbw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gmksuamuk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gmmeleyii.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/glpokandl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/ggnunweig.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gzvljyixk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gzdvqsupq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gybjjznuk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/girhqkdud.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/ggvakuiql.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/gngawnhcn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/glajkbiii.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/gwsuospgz.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gxagemscx.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/githinuiv.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gpowumihv.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/gdanafhep.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/giretvddd.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gbnbdcayu.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gvaryedsu.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gogxpnvte.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/geghmyxax.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gsasawptd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/ghgdtyhwx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/gmoembyfg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/gpvzfrkzt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/gqxggfkel.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gidbtknur.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdapqiveg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/gjebejweb.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gblunnvuo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpgjqmqlh.sHtML

【收录内容】
来源：http://www.share.fehbvm.com/Article/details/gjkdnvhcz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fehbvm.com/Article/details/gyhfbqucu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/ganhmdrsf.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gnxinqqjc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fehbvm.com/Article/details/gwpsluybf.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/gapxnxwre.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/ggcsytcqv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/guxkjvnrw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gadpcwzzm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/ghtsrvlvf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gedkfplhh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gjfwlvkwj.sHtML


<!-- 参考信息 -->