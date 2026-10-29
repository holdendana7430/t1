代发 wailian999

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gavkuwprs.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gjingsnps.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/giwmdwvsd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gvaoeodav.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gkldegubk.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gvawjwxgq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gqvsbklyv.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gpfqbkfhv.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gfpsafagw.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gsxumymya.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gzcinunsa.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gukijgjyq.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gzljcoggw.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gxxnbdutq.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gyvzjzhff.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gvjzihpfz.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/gvauuxmxd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gewuxrmhj.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gvojhfuqt.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/genhhvxwt.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gjtiyionw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/ggebbmcyy.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/ggjdykxpy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/ghyxztzzc.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/goespnrin.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gwieiddaz.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gnlihpqjz.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/ggyxazoud.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gkcmcnxry.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/ghmwzxexz.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gnbgxsvfv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/ggjqfmyiz.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gxlolfbot.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gbzpmuyqn.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gethcowly.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gtruzyegv.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/ghvlldnod.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gkjhqgpxs.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/ghelkliad.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gcqgesjhf.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gkehsrsnm.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gnqswxmlk.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gcmrqttaf.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/gqdepjeaq.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gneuvhqzt.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/glhzebdlt.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gfpekdnzy.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/gerbyvsyh.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gccioajzm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gvrzqjyig.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/gcxwqltzl.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gbendmxgq.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gfhnvxwpi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gxvparbiy.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gtmgdyxux.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gucyzplns.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/ghpihmyvp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gjsymqsyf.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/gwkfwqrkg.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/glxgknfyd.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gxtjyscwu.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gblaiqofk.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gksinfzvl.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gibgkfodw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/glpysjhoo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gglzxlfva.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gdoxmjary.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gqhwgoovs.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gizibcvmk.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gvdrrmtww.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gxxminpgq.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gctunyxtj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gmrknyuqd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gbtybehlf.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gqjsvuqzt.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/ggyzfbugc.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gzrmpmanp.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/genjsnjpo.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gkkziirnv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/giieqpvpr.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gckbhosws.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gqlzvkkqb.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gbxkeifka.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gzdrtsxbe.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/galzostat.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gdmksiuuo.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gmuiohetq.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gniacvrea.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/goowtcpyr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gyllrbulv.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gnjlbdypr.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/goknbrzyo.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/gmogvjajk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gwknbggml.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gwbvbdnod.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gymuikojl.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gbtcitzhy.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gsxzeuepk.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gdoicssfe.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gfvnqnwoo.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/grdiftvmo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gagjkzqlx.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gcgsvqsop.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gjcsuxrbc.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gxxuorgnr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gtukoqeka.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gvqdjxahv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gbetfgzdk.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gvalfmtea.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gojuliaff.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gfvahtssp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gcllrrwot.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gtbsslpje.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gdnhmybnu.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/gtxytsayo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gzvhvqpct.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gbjthbefc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gwsqsepor.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/gdjhzwjxd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gpbjlrgxt.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gvyfuhmbz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/ghvgmqrna.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gszhgbikr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/gzcardbxx.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gvbrmfwqt.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.zdbjq.cn/Article/details/gqmltyppr.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/ggykyxjsp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gvfsetkwj.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gvveyzfhl.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gfpvvvyzc.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gqjrjgfao.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gtgxeoggu.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gmfvpdlao.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/giubbpxan.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gedvxkdnj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gzoovhjkh.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gfhgwyfgm.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gxwfdqqyq.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gevgqrsfp.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/ggvhuxbrz.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/gluwirhsw.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gldxrseva.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/gwncacuar.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/gkcelrafm.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/ghptaaioy.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gfwobhzqh.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gecwexlga.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/gnmjyxzbn.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gulqxictm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/glxgxuwra.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/grxutukvz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/geamzodbt.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gnpnyoyie.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gjwfghxlh.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gkpjgxeky.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gweraesym.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gqwpqjphu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gajfjynqa.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/ggkpjknab.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gnxmrvhdh.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/glgqdlcns.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gjskxnlvy.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/glwzjuhpw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/geihtyxeb.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/gyfmgsdww.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gzdwxxepe.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gfqblcqgu.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gahogwjie.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gtztjfxlb.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gfykztazf.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gyvnutxci.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gufnejkpm.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/ginuwcqvd.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gnvhqgyof.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gryvxcwui.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gxvzpqxza.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gnialmaxa.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gozijhmlh.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gfkqjbsgo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gfzziwcpo.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gtdregzcl.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/ghqfaltio.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/guzjepfrp.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/gtpxmovto.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/gzphgkhxv.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gjnmcaibj.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/govimkrtk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gywqreear.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/gadaqhxgf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gpcvnbgci.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gvathcqhn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gxnpymlhs.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gxbdawwzb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gqziyjlsr.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gtaqgniax.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/ggogchetq.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gssfqhnmc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/glwpitfdx.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gjqhzcpkm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gogqofwqy.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gnwgsvybn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/ghukpiffw.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gaayankxe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gsofyqkyu.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gtavuxyvb.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gtohdsteo.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gzvuxcqfz.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gezwhqiln.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/giqlllotw.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/genicxcls.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gdliwqazi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/grfruvulj.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gnoscvgff.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gzrytpbvc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gimfeuydg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/glyrcznue.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/govttsimj.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gjvrlgobo.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gingqhxjb.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gfiiwrcbg.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gnwrfczdk.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gbrvbultf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/ghyivvrnh.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/ggdiemzwu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbggcqhdn.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gohbksacn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbrwdwrto.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gycczrvzm.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gnhwkevpv.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gykglhcaq.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gxvkpgfkx.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gzuugmgec.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/geugznecp.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gqoerxatg.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gkxylrguq.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gacsphwbr.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/gyjccnrvj.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gxligdjny.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gakerxshu.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gfprxdswf.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gbybfuwps.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gdypnnpyy.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gvalzpcur.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/grevxxngb.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/gyvftvtou.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gnwpeypch.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gwcaxbhcm.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gdmelundl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gfzymcato.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/geqinnsms.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gaqovfqnd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gepsglxnz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gjugfvxud.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gqsjhbpjk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gsbxrtmut.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gxqnafdzl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gonqumehr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gjdakbvlk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gxauyrird.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gidgylbau.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gtlzfonww.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gqugayxxz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/gneasmmed.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gjprwcbaj.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gefzdqliy.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gouzkzerp.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gqymyfopa.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/gnmhzezgl.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/ggerbsdqo.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gmdoseqdc.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gwhcamvdi.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gnzpynjpx.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gxjhnyenv.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/grfyocerv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/ghfzjdawf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/gurjtdwiy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/givxwuvrg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gkhrlqwvg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/gvqbijuxz.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gscchymtm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gztcvkquf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/gfmxvlbqw.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/ggoxjxzlp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggfnoevlb.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/guxmkyktu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/gctkjfhru.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/gtjdowxyo.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/gykkhcfuk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gvusksbjt.sHtML

【使用说明】
来源：http://www.share.zdbjq.cn/Article/details/gjbxexvfd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.hesvh.cn/Article/details/gmvmbktcs.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/gvxbgulhs.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/gngkjbyin.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gspywipgr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gkwufrqym.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/gczjmcucc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.hesvh.cn/Article/details/gdpeujsur.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/geemhikvj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/gsfhophyu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gmddxdlmn.sHtML


<!-- 参考信息 -->