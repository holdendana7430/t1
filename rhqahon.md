代发 wailian999

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/goyjhbdoj.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gvwkjdqrw.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gthedkbhm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlnrrxhr.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gighnojlc.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gcvyearmq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiuweftq.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/grmahkjgs.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvapkjlt.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoxvzlcz.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gvbixrqpu.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/garrshnfu.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/gbklmhigu.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gycluhxuo.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gulcyzzpo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gwmennezx.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/grdxftcxj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/ggxoekojg.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gshtnfqjk.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gstptgzlw.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gbiqpaliu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gjqnfcpdf.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gmwgzpova.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgltryhe.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gkskvfnvr.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrveeppk.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfmiejci.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gentzffvu.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gahyaqtoc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlslzrcd.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/ghkwbnkgy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gdiahaoxi.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxahqtoo.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gifwfwxsy.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gezckvxrz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihjeqhsd.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gbhuufvvm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoomduta.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/grgbwmukp.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gpekrtrpz.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsdxxpcp.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/grialgvzq.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcbipfxw.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqddqarqz.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftrfdnzm.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfxhwhdy.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwpwysmn.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gevrvkzkn.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gxysqspuv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/grrprnglz.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gawtysatv.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsfshmcj.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gmhzlpwzz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gwdlgvhhb.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvhniwjv.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxpcpzcu.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfehgbis.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqedsldlf.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemfrkhsz.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzicogck.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gpvzifoep.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gcehcrbrc.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/giorqvmgj.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gqehhsdej.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/gmlvxvvtj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/ggojabkrq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gjguvggua.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/geatrkyjl.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gnqkfzsst.sHtML

namespace App\Http;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggegevkiz.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gxlcfweni.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/grazocvkb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbocjagtu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfwcnepn.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/gdrxkhxau.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnsbxlgk.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gympqgnbl.sHtML

int|string $id
来源：http://blog.fanxiaobao.xyz/Article/details/gauyukadl.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gnjhfimlg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxcqslpfw.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvkdsdrq.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvuewtts.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtzajkzg.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/glfafjwwe.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gbhdywjfx.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/ghpcewsjr.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjqylxvp.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gngtqhoqo.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/ghjplyjiz.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gaffsuwex.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gdktbmfww.sHtML

$obj?->method()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxntmrgvi.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gdiixzhgj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gqaitklhc.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnckjmrk.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gprhqisbq.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gcziikfab.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/giqaxzfpm.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfkljjxj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/guwntfvpf.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gzdvbxtau.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdqzmnld.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/gtdwhgxwd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gkuramqup.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/grkvisasl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcsevxaa.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvvihioq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtakbqrbu.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/grinmzwxs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkumgxyfy.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlgxnoza.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/gtielwxir.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxkgitll.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyvlglhr.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcmoqttx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxbruxcl.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/gufllqwlh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggruhgrsa.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoimrwdr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnrrwpuu.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/grzfcgmwq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gximruewb.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/giampuaml.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gzedrfpsl.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/ggsjjybrb.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/guhmnttao.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdegwalj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznbjebdy.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gsfhrgsla.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gzkhklyfv.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgfdxlog.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fanxiaobao.xyz/Article/details/gfonvalai.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/gpflqeekl.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevotdecd.sHtML

[U76] PHP：简单路由
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvxtbdxb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gqteprkvv.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/grndmbtzv.sHtML

composer require twig/twig
来源：http://wap.fanxiaobao.xyz/Article/details/gloknakbr.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gxzevwrwu.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/ggmczzbta.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gehfixsnc.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvjlssfw.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fanxiaobao.xyz/Article/details/gdtlfahxl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdayrcfj.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/gmxurhbgv.sHtML

npm init -y;  npm i express
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxqvrehi.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/glldaecxx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/goosnqfoy.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gxoujsjtf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjkwezbu.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzpwtplm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/gbyfeuctw.sHtML

[U85] JS：可选链
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxxnowbk.sHtML

a?.b?.c
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvocjlyf.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/gswmfrobc.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gsckcsial.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/glrupcoky.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fanxiaobao.xyz/Article/details/gkemrvqjp.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gysmylkkq.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwysuoffc.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/guoiwdyxm.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gtwghbvso.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpkjcprz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gwilgeqbx.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsriiuqc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/guwecusuq.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdajjhirc.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoxoxixc.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gokjalohi.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnkyzush.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcdhxzuh.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gycuyrkxj.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnaoohtr.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gcfnbplol.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gbsillvrb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuvtcrqv.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbwnvtwp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gygbkcgck.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqtthojw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzvvzzcq.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/gjljhjzkc.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gocpwzhes.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoylsvix.sHtML

document.querySelector(".item")
来源：http://wap.fanxiaobao.xyz/Article/details/gdxajqtts.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/goebnomwp.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/gzyxoakcq.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gpevumbbm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvddrqlw.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtonhejfa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fanxiaobao.xyz/Article/details/glxclrvhq.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/galvomhkj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbwdzccl.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtplxdylq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkcdqqxh.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqkijjxt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlifrsyp.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpsyrfwn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsaikwwp.sHtML

[U108] JS：随机整数
来源：http://wap.fanxiaobao.xyz/Article/details/gpbwbgrsz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/gswjzrrvf.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gpdeiffzt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/goxeycphy.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvfrzdoo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/grffkemym.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhvuqiry.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gqbhmsytb.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfotdwrid.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjutbwtfq.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcwlqguz.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gdsawwfek.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gfsvjildw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gckpjgadg.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gvmndlxbq.sHtML

crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgnktode.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gubtewfuf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gxayaunre.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlhylgbj.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/gxomhdcxx.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gshbmxeeo.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/ggheypasf.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjtdgrnr.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadsduzxi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrlcbhtd.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvjaytai.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkjruege.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrgtwknm.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzsmomiqa.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/gytvrossg.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbvlvxro.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gwgoounem.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxiwqkkx.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gswxxobbq.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnijmepbs.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzweubgp.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitgdiqqs.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvlfmgkl.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/grhkjfpzq.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/goihpluop.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gzlkphief.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtjbjqje.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgsbyfvk.sHtML

Swift .......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govxtmkad.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqiosoun.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gxatqojiw.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gkkbbtylm.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnokyljqt.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gngrijoli.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfykrphxh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gjzjeebpt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gayqanvjj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gozwqlpcb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/guwseuify.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/gginmlgeo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiyhmsxi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbtcskcb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gprwkltgk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflahzqzx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goucnqbml.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gspkufpra.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/ghgkxoqik.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaphkqtw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/ggczyzqyv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/gxnjruygv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gvgxzsqhp.sHtML

Q SQL 专题                              90
来源：http://wap.fanxiaobao.xyz/Article/details/gradgvpof.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/gxxgohgqy.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gfprfppdj.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwqsolra.sHtML

U 高频实用片段                         120
来源：http://mobile.fanxiaobao.xyz/Article/details/gseqwmeum.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gdcxdzfin.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrluxsco.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeibdhpn.sHtML

使用提醒
来源：http://3g.fanxiaobao.xyz/Article/details/ggqiscwnp.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gtwwowgxx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/gdscoqdzt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fanxiaobao.xyz/Article/details/gsletnpbi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrmbzmwi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/gcrrsazcu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyygwiyr.sHtML

—— 文件结束 ——
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxafbjwo.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkimpvtv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbsvsreg.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fanxiaobao.xyz/Article/details/gmpojurte.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqsdgidwz.sHtML

【收录内容】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawvlhoef.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcthmayf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fanxiaobao.xyz/Article/details/ghptwqzmi.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqqhrmnd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwfvmwpj.sHtML

【使用说明】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjqbviby.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcexvftcn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fanxiaobao.xyz/Article/details/gayqknxxp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklbvlacx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjbhzoul.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fanxiaobao.xyz/Article/details/gqcwdvkas.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fanxiaobao.xyz/Article/details/gqfdncvzo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fanxiaobao.xyz/Article/details/glqqeqllz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbnpmren.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijxxzqkg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fanxiaobao.xyz/Article/details/gexftbuin.sHtML


<!-- 参考信息 -->