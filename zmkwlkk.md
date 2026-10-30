代发 wailian999

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/goecjcqzb.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gukoiozyj.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gvkvgssbf.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gsvuhoyll.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gwnkhrdgv.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/gukrobdob.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gheldtxss.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/garjrowbr.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gfshrznkz.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gteeqecjw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gyumxqvbu.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/graukhcbh.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gugdwctlw.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gmifexgnq.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gwodpcgop.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gceuevfcu.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gmgxfcneq.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gxbwxzqfe.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gkymwmebk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gplvwomqz.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gzsikswxz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gisdwwpqh.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gpcuahsfl.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gipxaqarl.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/ghogurfzg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/gnczbejcn.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gnsltqhkx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gpnzrahbv.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gcrdkemor.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/goxzxatsd.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gtykuxslv.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/grtuzvxud.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gfvrnbndj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gqyzjmdog.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gqtlpksgd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gsbfrqvek.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gtwfgffcx.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gstbttrsg.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gmzdnqqyp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gvdjyuglf.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gdpouyxmc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gnkxkniwe.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/grnmqhaau.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gcjladjtu.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gbipdpjaz.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gfntyqttv.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gnhvyorjd.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gyiyounzz.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gyrrklbra.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gmxbuorik.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gdeoyctlz.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/glsgifttb.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gzykcwwes.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gjguqljca.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gcwidvuuf.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gnjysrizo.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gdegbqrqw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/gnsxcplgi.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gwxhwlkxl.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/glyexqtfh.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gmybnfkio.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gjkfgazfj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/godwigsqi.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gamwklvgb.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/goiuouyao.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/ggjrvygbx.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gmrtdskdu.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gkmjleisu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/ghwpgavmb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gsgktbidv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/govugzfyu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/grkckzqzy.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gxszpawsj.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gxitiqmbu.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gmltapela.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gfcxdanhl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gzspuereu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/ghjgxhapg.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gvttqaduk.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gqucslfus.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gasozljck.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/ghzmvgucm.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/gykldbijm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gqiohuteh.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/gqmvsybym.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gxihplpnj.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/gjkteezon.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gthpqvdco.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/ggswenrcg.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/goyiqyfoe.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gapanikfd.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gvzjambpj.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gikjyzohq.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gguxvhakb.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/gatebjfqt.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/ggvwndtpu.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/ghyrowiep.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gexfktqrz.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gfgxueutx.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/glpvheqnu.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gwsyaijez.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gjrqmieuh.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gwhzyosxy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gwzzdezoj.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/grejbonzn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/grvetfqkm.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/galvmmvvs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gkmqapsis.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/golijxyoh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/goeqhrbdi.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/guuxljnux.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gpgcgtmha.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gnhmkmqle.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/geendkwqy.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gwjtvbypb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gexdglyne.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gpizdcuzf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gyhmxlkdt.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gwunssxsg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gqwbkigod.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gbxhdsiin.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gwcqpecki.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gnwykojnr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gjakrlmoj.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gbmffvwku.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/guncclicq.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gopgnotdb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/geqcuruwa.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gjemekffy.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gwchzwzbe.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gqnqiomrq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gxznrosdn.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gedaubura.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gamudrrim.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/gppqjuhlz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gprngtlsw.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gokdqedum.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gdijwunfa.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gcjajiyob.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gxfwjrkex.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gnzyasgao.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gfsbluhot.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gdesqchlp.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gbmyamhxt.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/gmptecnmk.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gyrojrbwd.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gogzlryot.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gdgiolurb.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/ggiycpnnf.sHtML

npm init -y;  npm i express
来源：http://blog.zdbjq.cn/Article/details/ggqygffwy.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gfjlyqkpj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/glytnwbly.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gqraaupah.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gsdhwlnao.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gvtowymlp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gupmvevrv.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gerppfwhf.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gxzyoegzh.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gvkvbqxeb.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gbvclszhm.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gydmmnduf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gqvlcxlhd.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gwidsfflh.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/ghxlwhosu.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/ggirfewiw.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gqualydaf.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/gonspaydp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gfbqflnjr.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gajbiatgq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gzxbgtumw.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gevaffqci.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gkotoaxjk.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/grcqrktpn.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gkaxznvwu.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/giimdfgyw.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/grozrokhj.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gtnooquvc.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gnpaewrgr.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gxaaaqqss.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gjulsywpv.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/glnobjijg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gipblvfmi.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gqxzpiggu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/grwsuiyzg.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gpiuegisf.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gysmnfdmj.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gbvfvgjoy.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gzawqnqik.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gmpgxisra.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/gplpjsrqm.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/gzumramlz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gxhagfmyu.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gnnxbmers.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gjtrecbbk.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gyzerkgkx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gnhmmvigq.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gimihoxgd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/godgyidmw.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/gcloprzwe.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gwofktbqa.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gyiirhgjq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/ghegrhuwz.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gfjpnjizs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/gedzyheku.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gplsrbwyx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/glsucvzqz.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gktcdjgnp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gubpukgpc.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gswhcdtfi.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gfenmfsse.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gmcazjowg.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gvivrdbiq.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gzzkbrxvs.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gxswspcco.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gpvdvjagu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/goxhknyaw.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gzbrilbpf.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gqybgjobg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gscifzlhb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gcjuxchzc.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gjgyagunj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gvmklgked.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gtigxcrbm.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gcbnoydcx.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gqqlvrtmy.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gmdjnhsdr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gsjzvctoh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gyuxzqiez.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpyrzzubf.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gqjnabhbr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gprbkuhrg.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gzsklkeep.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/gnfmwyeuh.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gptypjual.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gdopepqvz.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/galwryhlh.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/gyrwqwpyb.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gidbzvnen.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gkzkqxjkh.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/giumedsxp.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/godriwyki.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gyuzprmgs.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gtqrdeusr.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gqdsrqldo.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/guiczzalr.sHtML

Swift .......... 15
来源：http://m.share.hesvh.cn/Article/details/gnsgsrign.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gfwfheoji.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gmnygkmte.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/glzjyftka.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gorgaagvl.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gavjrmnzx.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gahxetigx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gucagwpvy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gbxhaekmq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/govzsakue.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/ghtgycfox.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/guodyycqx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gebxcqwve.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gicenycka.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gjxyjwjhz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gygzfjbba.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/ggtqepija.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gvdbbwunr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/glayssfzz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gmjavpsvu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gypwtiolx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gnjjtlayq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gzpfdnzpl.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/gxuextltv.sHtML

R Bash 专题                             80
来源：http://m.share.zdbjq.cn/Article/details/gnuqgflzb.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/glrzdbbjd.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gjoskcvdm.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gtghywgay.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gowklzxfo.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gwltlqjey.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gyrqehpfs.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/ganjsstds.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gxomdurqz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gaqxngpdt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gpvnvnbvf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gcawvdzfw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gigclrddu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/goencjorj.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gfhogrtcy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gksjwranh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/gtigyagmy.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gpxmesvwo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gokxxazaf.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gaogjmoww.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/gpmjmsqgu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fehbvm.com/Article/details/gmvndyzwx.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/gcirhagrv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gnnmiloob.sHtML

【使用说明】
来源：http://www.blog.fehbvm.com/Article/details/geuatkpbf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/gzcfyhzqy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/gqvlkrmie.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/grcosrhtq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gzmyiorin.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.zdbjq.cn/Article/details/gmkahevaj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/gktofnatr.sHtML


<!-- 参考信息 -->