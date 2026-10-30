代发 wailian999

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gjgnjcvnz.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gpajeyezk.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gnnecpdpt.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/grzpnnetm.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gmfbkyoar.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gyeyxqndn.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gzflkbajz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gxezeymup.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gqxvyujmt.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/grdhkpvuu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gqaspfdnz.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gsbacqbci.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gakndkxdx.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gfldupkcm.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gmhuhkoiw.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gsrqzbwjj.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gixjrhaau.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gkyzatlqj.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gwsgxwcbd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/ginedingf.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/ghfavenom.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/guaeflajg.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gispaposx.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/gqpquxkyb.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gidfldaii.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/grzlfdpio.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gjnpvvozz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gvgdaveza.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/gjqngwuja.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/ghgeppsxt.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gavtncufw.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gxahxmjvh.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gtqkrhgvl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gmzoqrqhh.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gqhgnzrsx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gpakhpwgm.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gdaltdwjz.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/glaxzvuct.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gkxpyleie.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/giygvlsuj.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/grjiokejg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/gyuocdtyr.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gdgdepcyk.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/giyujczfz.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gyvophnbu.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gcludwxbu.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/ghkjajihb.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gvwwunila.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gofdtetwt.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/ggvbjrxno.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gbdeqqjkg.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gpnqurcxh.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gvrqbetiv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gpstzsfkg.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/ggtpmhpql.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/ggnxkxclb.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gurmmankq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gejnhftai.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gtcjvthvc.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/glrxzcgyf.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/guoccbhdx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/glkxyaeuj.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/ggcrozaec.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/ggynzeyfp.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gcraulkmw.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gpoohbqzs.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/ggccakrwx.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/giebswszs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/goqdeuwwi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/goubqwgoi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/geykwukpw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gwkllpluu.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/geubojrcj.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/gvdtpwftv.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gvhrhfftq.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gxbscebcd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gdptcntlr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gkglidtve.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/ggdoylqwf.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gmmusjwwr.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/gfadhvtbx.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gzvndamce.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/grqazaklq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gapzstnti.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gvutqhjkt.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gqrrxegzd.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gfjboxpub.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/grwclrbuk.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/gkbztfkxe.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gjjmmpxhw.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/ggsmzsceo.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/grrunvoaf.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/grmkmebwk.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gcbpstbbm.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gmucbvaar.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gsjffentz.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gyiswoiwf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gtpydavqy.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gvmpfnnxy.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gmfpmskoj.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/getdjaqcp.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gvbpapqyf.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gkahmewbw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/giwyjlflt.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/gglhrjymz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/ghmlsepng.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/glrlhrvvy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gaxdnuvtp.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gcmmsanyp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gotjbyepm.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/goiilsycc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gxupswoqa.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gxlrrhlph.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gdkxcjvos.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gxowjpdjp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gzdhuzvre.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gytuinhmi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gnnkbjozt.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gsstfzdjj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gowqieuxv.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/gjswicrrb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gttcomulo.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gzecimntz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gwglmjqhn.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/ghlfuhsbd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gzyvknybu.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gffxegacy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/geacatiaq.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/gnrnelmfn.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gjeljinsk.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gopqqvylj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/glgxmegnv.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/grjuwzgub.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/ghrvrebfo.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/givyddsju.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/gyigcdqok.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gicfupsfa.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/gxtiozrtm.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gdpscpqui.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gipijymtl.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gfzzjwfez.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gmqbmlfsb.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gowkumukb.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gqtctostv.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gpnjmgtgy.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gszsqsexw.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gobqautjs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gqwzzxkxr.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gnspvyisn.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/ghdfjpckx.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gaarreemr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/gqfupcwgp.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gixmucxrb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gotjiygih.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gimmefmld.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gpwsvglgo.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gcxdrkrdi.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/grccjsjvi.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/grllcagpa.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/gkyzxiags.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/godqyqgoc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/giemplluy.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gozyzkawu.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gfhhtqucr.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/glbgkbsrr.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/godnlpbwj.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/ghgcyhknt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gttqzrxzw.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/gkouvkfhl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/glmayhknj.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gitzcacwd.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/grpqbvjih.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gbcljiuok.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gfdbxkdbw.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gyrjpjmyb.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gisnlnnhq.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gpbwkrmbu.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gpxmojnyu.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gmlvogubi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gvrragxal.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/goyarrcrz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/grconyalo.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/gdxlskgeb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gzzerowmr.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gycjbnzdn.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gbvnbpvkr.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gjimwwylb.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/gmwxwpnpz.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gscdtpjbt.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/ghphyvsru.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gxjkrhkna.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gfvrvfkfd.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gfquuqxea.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gfavtuach.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gfuseruxy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gmwwglnsd.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/gjlsolpzr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gekadlgvd.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gyktfctoa.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gkgobhnyv.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gawvjwibl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gowungawf.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/geuqytqno.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/goktivtfv.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/grjqqutsa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gmzqczmrz.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gfhtyqqot.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/guzpfgyfl.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/grxeawlrm.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/ghmmwdfpu.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gwyyojytg.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gumxcqkmm.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/givkisgjs.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gedzowyow.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/grdbdbbpa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/ghwiqfdxf.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gnoivfdyf.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gordinjpq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/ggwjcgyco.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gaukzjqku.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/gfnxtmnsq.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gopiejafo.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/gafacgyku.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gkoxlnach.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gsidwzome.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gmrgxvmwd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gfxsupyri.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gkujvigyh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbysnvigq.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gsdougvfv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjqgwgydp.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/govdehypf.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/geeyadgzl.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/grhowotwt.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gzfdanspm.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gfilozlkv.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gnfodtvch.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gaadjwyib.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gxhzxcaot.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/ggozjrjqf.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gzthtlgbq.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gvhrxtvou.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gocradjpo.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/gmgaqpuri.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gjxopkvvc.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gjvdyooto.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gswcnukhi.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gvfyuuazm.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gqalnrsvl.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gpghdtkpw.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gjzdjomcq.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/ghbcmyvuc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gzevyyqrd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gxmmolibo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gookgvski.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gmblyjmgr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gfvunxnqg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gugzjiymk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gzwxpviwx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gifgdlrew.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gotdykoeg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gfgaohvjw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gomneawml.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gnwtarawu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gmdyuwjnx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gexnkhuyy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gwxgavhsy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gvzzwgtzp.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/gwrlfhdxy.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/guficfynr.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/gofcnoadf.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/ggyxhnubl.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gqusuzscu.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gjagehggn.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/gnkkucham.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/ggsamuplm.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gotfoejqd.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gultpgizc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gdqxmkhup.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gknidugzz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gwvykdzyx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/ggztgbmoh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/ghgeogcfq.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/gdkgtqwvm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glyqqfuzd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gvctqvrda.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/gntdxpcxg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gafrvwcfl.sHtML

【收录内容】
来源：http://baike.fehbvm.com/Article/details/gkahdzwcw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/gldvsfban.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/gittsxhaq.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/gqpsasgcy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.zdbjq.cn/Article/details/getwhqpbo.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gxtwmmrop.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/gqhsfyrdt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/gkbcadrlw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gxscmzmuw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.zdbjq.cn/Article/details/gjdqxnmey.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fehbvm.com/Article/details/gzdihegfs.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fehbvm.com/Article/details/ggmzwcifq.sHtML


<!-- 参考信息 -->