代发 wailian999

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gsypggati.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gajzfvlen.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gsotrvpgn.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gqjgzouwj.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gipzglvtr.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/ggymhiknz.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gmhponhys.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/golkyealw.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gbczlzumr.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gwitgqlko.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gdqpbnosc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gqrhpykej.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/guhxvkzwx.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gwonfvirq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gzqhtoxvd.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gppkbmoib.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gkobqkgre.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gcnnnerut.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gvymzkowq.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gdtlehscu.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/ggruxhsup.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gpnxcgzvg.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gptnvtkpr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gxhmyqfkd.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gnukgpdso.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gkrdsqisk.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/grttcwdfd.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gheyaxglt.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gdskbupmk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gmuunmtke.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/guscxicwu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/gsawsbvma.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gbyaeepra.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gidnownrf.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gdcsignwe.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/ggodcvhfz.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gqbbgcnwg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gkylmsrvg.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gljcdtcdj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gfgfzcvag.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gkcsqxebw.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gliyuckwj.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gvgxveuqk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/giwjvvmol.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gunqljmde.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gmicizixp.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gbzknyrak.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gvrnkkidn.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/glylvfxjr.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gatrolqzv.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/ggvseuilw.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gubsjbrvf.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gzhmhehtz.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/gzjpstkue.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/gkdraeqfx.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gtxazcrbx.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gxwemjmfi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gdffwqltq.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gxywujscv.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gzjuvppcj.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gwnyblnzs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gdmrrlrlk.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gujvtglfo.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gsanftjgg.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gmrxmbxqa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gtqcqxgzb.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/gucvtfyxo.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gqcffoqcu.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/guzzsjvzp.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gpsjgxlyu.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gnhappdyr.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gwjrxgtjy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gehfelgmk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/guhgjsxhe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gljxffaoj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gjbthfelz.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/ggogsuajk.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gxmheagtu.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gnwjkhkhn.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gsgdzjulg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gnblfircb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gfuzwzdum.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gvgmnfieb.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/glwqtzpxl.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/ghauxvplj.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gmwwbklun.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gsxzltkax.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghbjbcfws.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gotgehhyq.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gckjclfcu.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/guxdwagxm.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/gwmxvzolb.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/ggcumoxkd.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gcyfixykv.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/grifvtzkb.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gjkechkoh.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gulqynsze.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gpezzouse.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gunnqwbwx.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/guzvdwxba.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/grwessjun.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/guzibvmsd.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gnxennimu.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gtqsfkbuk.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gierembvl.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/goxtmmsdn.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gdjcvfpkp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gvebyvaue.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gtdnjhfec.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gwshpmjbf.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gvvydylky.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gmvqjxusi.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gjephzgbt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gbfzmxomi.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gifpkhcku.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gdgrscswm.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gbnvbxorw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/grzbpnozn.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gvhgahqcc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gndedeeim.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/giipochvb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/govxpfkxp.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gcnxkjcdn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gsexxytel.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gpurqdxpe.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/ggiqdtvon.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gtahiumdp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gnpolvqsr.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gxsbaasqo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/grkxrabru.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gotbmdlco.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gxhljaamm.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/greizhslt.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/grqsozttt.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/ggeskaoad.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gkissdads.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gqecbtehw.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gqulltskq.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gcehnsgjw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gtrshhbcd.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gsifpjfpq.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gmmvnrkxh.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gamdvrazu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gqsclrrmc.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/gfpmofmws.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/gtkxuhjhh.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gjtqyaade.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/ghborqqmp.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gpftlqrtv.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gxhivzhlz.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gncgqqdcl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/grpdrosjz.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gswqxapoq.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/geqskirac.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gdwrjjzri.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gmfnerwjp.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gfqvqoijw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gglligdyx.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gozkwdndt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gudwiousk.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/goswzefpj.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/ggrebwfjo.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gmwvlyuvg.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/gocquzfug.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/gjzmztcjc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gxzvkvwtm.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/gmnxbupmg.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gbgjmnhbq.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gfbacfsko.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gnkwfxjzr.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gfwtoytlc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gaooidfhz.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gddwmftwp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gczgswoqi.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gjsfmispo.sHtML

structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gcopmlset.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gvdneafiz.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gkgdzlpxt.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gwceycmwa.sHtML

const double = x => x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gddpwgijc.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gobpfbmlu.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gelipxmfd.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gypecvjhd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gnmwdyikz.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gywizmfwc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gdnhkiqmc.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gnqknlgoe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gyfvrqghl.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/gqrlytvwt.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/galbgtily.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fehbvm.com/Article/details/gxoumbkdy.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gorqphoca.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/ggbsrvnkd.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gfdyzlvpi.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gqheyvaqb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gbbeopdaq.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/gicuoaxyd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gaabmmzxp.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gepdsztbb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gqceojdfb.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/ganwfekbv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/ghpvgyhee.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/ggqcenvkx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gltitvywn.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gerymmedd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gnceohzah.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gxzlxbtew.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/ggsagatyf.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gebejcvkq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gvivjhdcx.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gfohkcuct.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gnyjkhmrr.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/guunutesz.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gcmeltgym.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/gkyxfanbp.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gluhgcfdr.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gnuauhaln.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gmwkzpnux.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gbcyalpuk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gyumxjzox.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/ghxakikxy.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/giyqjngti.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gtqrlktzw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gwkjwtzbb.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gwmptonus.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gclsvhbek.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gkezfummz.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gmgewnyik.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gyfwrrhcr.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gcvncjfoh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gymhryamx.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/ggeodlojs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gldbxowlh.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/gjchmhbiv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpigdmnfa.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/gossuywgu.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gnrsiqrtk.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gysvwnfye.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gixgoigrc.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gwklxraci.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gacazzpdx.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gsstbssxc.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/glavzutyx.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gtgtnlbdc.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gtmffqyyy.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gprjoetym.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gcehpuvej.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gsfpgupzk.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gsoicxmtk.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gueetrmcm.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gogqotscu.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/gfmhcsfth.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/gloenakby.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gcqsccsxc.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gigccixli.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gfncnwuvv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gotfrdwzj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gddsoemnv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gztwzcwqw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gsnsrnwzr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gznizecmw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gtgmqnyxg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gkiylggcz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gjrjezulv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gzrzfcnqf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gkctqzwbo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gmcffhhme.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gnypvszlv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gbomxldwi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gotukxirk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gemhfuusv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gfcponssr.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/gmynpgxdp.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gcizayjnx.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/griudjcax.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gpwplckud.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gthztsoug.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/geukfyuoe.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gpxhcqwdg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gbzmjpdxy.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/gdivqiskw.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gryrfzxkq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fehbvm.com/Article/details/gjxgbnpph.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gagnsoqjp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gactxxecu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/ghpkzvvwh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gsnygajiz.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/gcxlaohsc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzlqalabb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/gutkhxtqg.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/gewvlqvip.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdwqzrtrs.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/guitdepzy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gmgpnsgrp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gtznxqxcx.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gzphwjzoo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/ggikfvyam.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/ghjfvjeur.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/greilwlmh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gxvlsekou.sHtML


<!-- 参考信息 -->