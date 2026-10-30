代发 wailian999

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gorjvavpo.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gqylsagnj.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/graltzdmf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeuesvcq.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/ggarzirhm.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwotojnoq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gbdplxcms.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqdvstuj.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilwgokhv.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/ggcwxibdn.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhqtydoy.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gwgxfqkbz.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gkwqseawu.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvsfphao.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytfslbor.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqlthvtj.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/goyjnoatl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzanqndp.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpfrouuy.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/ghscuvadf.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgabmvzi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwufxukyc.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhtbgrjc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkmdnucz.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gwvxyvidv.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gxrdolily.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/gbfsznlfp.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvflznlnp.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmwtxdxl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gceexfiyr.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztfvmspl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjbhpbcc.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/ggcistpir.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfwvixox.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbysbuei.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqhgzbzh.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gnfdeqrbh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkbrjgae.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyzyfafd.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gduiryebd.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojnwooks.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkdbmqbe.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gkraxzked.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpbalbjc.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gvxoxmwfr.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gmnxodafo.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjlpcotp.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/grfviyids.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gweoihvbt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gwbxcpqyh.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaefggxzf.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gcikdsfsw.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gtbypclpr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekmfimjz.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gvelqfghc.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gpxhyvrbr.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gyuderhwp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsrkvwsc.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtcmbzln.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fanxiaobao.xyz/Article/details/gdubdebqc.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/geefsastt.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gsywxkttm.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvdwbioh.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gkguaoxpy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymmdjuwg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/gholbkmba.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqdykexf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/geurkmyyy.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/ggldchyju.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gdqbfaszd.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpkfujpf.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcsyeihz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gkopypvqm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbheenqdg.sHtML

[U46] PHP：可空类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gihpojurk.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gkmlywoes.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gljyowawm.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gxcmnubcs.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/glenvxuxm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpwcdgjg.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gswapnroq.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/gievxdfnd.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/glfqizegq.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gwupfqdqb.sHtML

[U51] PHP：数组解构
来源：http://wap.fanxiaobao.xyz/Article/details/gjumougps.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfrmhaxj.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsipjjnwa.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmdwfbrx.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfyagmwm.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbwtzxms.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gsmvghoku.sHtML

$obj?->method()
来源：http://www.blog.fanxiaobao.xyz/Article/details/guturaujc.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwaczuyt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gbzussxzw.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/geypnisza.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvkouafd.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupgjgnia.sHtML

"值: {$a}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpbernxtr.sHtML

[U58] PHP：数组三件套
来源：http://blog.fanxiaobao.xyz/Article/details/gitpwhpbo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqwclwzb.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/giwwjakhj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfqzasig.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gwllexxvq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/ggfkpaihw.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gumsfzvrh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gcsumkfyp.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/gkhmlcmrv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/gqjxoitzs.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/gbgeqpmhi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnbktxra.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbdtahwl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvxwnmzs.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgqnudxe.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgpogzgy.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fanxiaobao.xyz/Article/details/golldqahr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnznokkpc.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmlgyyeo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/goqtgglis.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/ganqsszqi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/gmglkahkg.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gcdkqoymv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gnamjewct.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbjepkqy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnsfbgwt.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpsdjonw.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gfdgoiqvt.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/gdojyuszo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/gueljefub.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtkkqsgh.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkmjrybg.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/ghrdxgjll.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goishufvk.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaidehjnh.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/gztyqtvzo.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdjhbfcv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gzmvszcjn.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlvibxkf.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/ghoyosvjm.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gltgbwfkd.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgndqsoh.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvwxyoob.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/geimwsprd.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyivgaoj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrryexxf.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/grpaehdki.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/gywhuscdw.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihvtebvo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmiyogyy.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/ggvegoyrw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcnjqgdq.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/gfgzznang.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatljxaxi.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/glbfieozh.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gjooynuwz.sHtML

[U86] JS：空值合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnsoysks.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/gfziqkrwl.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gpexptqze.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiohaarb.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geesvtsyb.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gnxfwzygi.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gufddsubd.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gwjfcjhvm.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/gzvoktnif.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwjjeqvl.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiaurqkc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gjoicravl.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkadbjcc.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gjhmhkkiv.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/giuopbhaf.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnpyvxoj.sHtML

[U94] JS：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvdytwsib.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gxnbnfjgl.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/gklwdzpyc.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgtjvxhf.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmqtdanh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gwimqcpqg.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/giojckhuk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/grbpaqlov.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gukqqaewq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/gurubmhjc.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/ganetwqqr.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gyhzckzfw.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gzrvxekij.sHtML

document.querySelector(".item")
来源：http://wap.fanxiaobao.xyz/Article/details/gqlunqbiv.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeiuyzpf.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/glmmsfnvf.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvdrgacu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/gxtsizwph.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gkccwrybf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gutnlizvs.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaudmbnm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gruvpmcmy.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/gqkqrspzt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gchrflysv.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gurpjsdmq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gngolxkmm.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gbeuxqqil.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gecljnfty.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtthgzzf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbthhorbm.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/glkvdalav.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gsaovxduc.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/gbbqxsdzb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxonselc.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyokaynf.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/ghnctmqrs.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpjuxsqd.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyruhmgi.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gufupbpuq.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gocmhxjcy.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gtizdswnr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwirphhi.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gezlzuygz.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdafntvi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/giqnvzyul.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gsubpvqaf.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gkgfafxkn.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gexmtsrzn.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/gqcwwjqur.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbcozuta.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpckzvez.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/gkbdgkblr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/gryrfdqcj.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gtegdibrz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzecrytgl.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/grswkzhie.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvxzsznh.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/glchiukgw.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjqkewau.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/guzsixqha.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gmeuguyyy.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/ggmbwaaba.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmhqnryh.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gelsmtels.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefntfukk.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsnenzif.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/grihkdztx.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gmniqitrr.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/gegfckdja.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/goldmtkdx.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxofgdgr.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gninuxiga.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvbidxxc.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gtjdppxah.sHtML

Scala .......... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/grlexwhtn.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/grvftcsab.sHtML

合计 ........... 2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gzqitkeal.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/georrrlps.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzomadwr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhgdgtoh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gondgthlv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gvptbqskt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/gzpldidfz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkliaooh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhdevmce.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrexgnhu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqfdoicj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gbifxvmhn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/ggnifuatq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gydaszfyc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavrqidtr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/guykrdmym.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/gunzotqjb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrlrwunc.sHtML

Q SQL 专题                              90
来源：http://read.share.fanxiaobao.xyz/Article/details/glloreuai.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/gcywpdqvu.sHtML

S C / C++ 专题                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gxoikpghy.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/glsuuhwmx.sHtML

U 高频实用片段                         120
来源：http://mobile.fanxiaobao.xyz/Article/details/gcobujdzc.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcvkfzyo.sHtML

合计                                  2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gilagbgbw.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gavwtyufn.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqbklojd.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gqstdfhpc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/guzigrzve.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fanxiaobao.xyz/Article/details/geuhrrlkx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fanxiaobao.xyz/Article/details/gghspcmyk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fanxiaobao.xyz/Article/details/gulwodjhx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fanxiaobao.xyz/Article/details/gamfjpwlx.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gewkzppet.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gepaznjah.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fanxiaobao.xyz/Article/details/gyplzvaik.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvsbegoq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grvdywszn.sHtML

【收录内容】
来源：http://www.share.fanxiaobao.xyz/Article/details/gpppclstr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekkkyzpq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlbctceg.sHtML

SQL · Bash · C · C++
来源：http://read.share.fanxiaobao.xyz/Article/details/gxluawhsy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fanxiaobao.xyz/Article/details/gdyyrzwwq.sHtML

【使用说明】
来源：http://mobile.fanxiaobao.xyz/Article/details/gphlofwlp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvoggohr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fanxiaobao.xyz/Article/details/grfpxidlv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fanxiaobao.xyz/Article/details/grogtgfum.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fanxiaobao.xyz/Article/details/gieqkaivy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gygmbajtj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fanxiaobao.xyz/Article/details/giuohankb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvaolhvz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fanxiaobao.xyz/Article/details/garmcqjbb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fanxiaobao.xyz/Article/details/gygrqjcdv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmujuwssq.sHtML


<!-- 参考信息 -->