代发 wailian999

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gecbhefag.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gyxsbegwm.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gpznuggpf.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gmurqpxmb.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gbwsgiuet.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gokyppcqo.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gkndjmrhr.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gnhxbblcn.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gxdeakwad.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/ggafzircy.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gwykiiohr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gybcakwgt.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gtjgkhdnf.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gmlrswdil.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gkukzbaoq.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gliepnzwm.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gzbrjtfge.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gtdohshhc.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gnuegqmpz.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gfbntskqp.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/grvskjeuj.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gcvatgrft.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/ghwiqvjkm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/godphjijx.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gqwpucigm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gdhyeehop.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/grrzeovrs.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/gagpotkop.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gzdpaxdli.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/gjkncnapj.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gvpqscpdx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gubdvjhyy.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gccvhyfkq.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gstenqwli.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gntslpwxb.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gzfdbfhxq.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/guqahjuiv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/ggbnlkeix.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gcqnkxgjm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gpxndlykp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/geykbsapf.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gkttcaexs.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gnepdzebj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gxcidgyds.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/gwfmynfth.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gmrqyantu.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gzcsbfmnd.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gcznnyeme.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gmadntkyj.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gwbgdpgre.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/gbxridccl.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gpzyhqudr.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/glqiukubk.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/ggyzarjoa.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/guqmkyzjy.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gmbmlljdl.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gtqsqeafo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/goxqckagf.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/gvwgkiixf.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gduhabtck.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/ghmcqahvw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gtcvptvee.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gdckxokyc.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gcpcqwpnv.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gqhrdgmyv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gymzroqlp.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gwgzjfnzy.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gtaykuyem.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gusctvdrk.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/glqdqslyp.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gzloznsby.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/ggpskaniu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gkmlbdxaf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/gibexddzq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/guhxyiozk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gzjvqiztf.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gnxysfynm.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gikpxjgnf.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gtztnnyav.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gxpoirfej.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/gqgrvnfov.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/goschhvny.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gblfcgfvj.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/guygaksbj.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/ghpzuzezo.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/goqldiukn.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/ghieieuie.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/ggwsgcptk.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gmvdnakhf.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gixctbnsr.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/gsnekhrvi.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gzmsebtph.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gixrqmwrj.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gmhtqxdqp.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gmtpzatia.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/grchbxola.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gqsnvxvsy.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gunrtpwwz.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/gjsyshbaz.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gkvpniwvq.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/ggjioijxr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gsflojkjz.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gqpkmfayp.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gwifrmmbp.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gttuxszji.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/ghpxxqyrh.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gxiafpovm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gvwkhgtlg.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gzljivbta.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gavjzmici.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/goexwmrbd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gdradznnp.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gyscxxwrz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gmdehwczw.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gezudwqfv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gpsrjvkga.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gnwglaeeu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gvtjdttba.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/guhthfbdw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/ggowxqbmx.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/guutyiqbf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/ghdfokiyl.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/gtmhqhisu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/gtulmfewa.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gamatnkja.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gdricnesj.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gsyqfjsbn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gngiqhhlk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gfnlpwakj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/gqvkbywyu.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gotkhcruf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gjoijlhuh.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gvoummoho.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/ghnjfwfde.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gmbxhwouo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gumatafqc.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gppkhuteu.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/gsiyldpxb.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gvgciiboe.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gtrhwlkcy.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gdcfpziyk.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gjaxcjkbx.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gtqkvszix.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/ggtlgczyg.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gviovjszy.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/grbanopwx.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gcesxamlm.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gomdfrwcz.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gsvyvjohf.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gwdigvktk.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/geecuqszb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gjsmqavbt.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gxzxkdmuu.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/gakkisdjw.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/gjzfnunts.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gcyrtimqm.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/ghueuerfq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gwdrrehkw.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/ghgceptmq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gqkawtuvq.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gekxfzybh.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/geqauetgs.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gtwpterpb.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/gfsckeqns.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/ghjwsbjuc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gbqzhltmz.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gpktqoboh.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/gqtidbhfs.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/gtgzinyfl.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/goxruohvy.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/gualxmtzs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gxtbtgpme.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gmzjibdax.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gmilbgvrg.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/glcqwafyt.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/goiqhpivb.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gqfvnhdvc.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gvdloakso.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gfyirrcfq.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gwkwhmmcg.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gigmdhaqf.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fehbvm.com/Article/details/gjxvjyxsg.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gqfqzdjjm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gnehervae.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/gkirbppdz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gwsnyxyvi.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gnzweruwm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gbyqmhtas.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gighwbhjh.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/giqqjvsbp.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gzzyuefvo.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gqxrfshfr.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gwsuxeupm.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/gshhnmwev.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gqmtlgvfz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gowiqaevc.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/grbvwxugb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gbyfaqrge.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/glsixlloh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gezluhxwn.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gwbrmmyhn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/gpxfhbign.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gildenelj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gifyfsdkw.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gkxspdbww.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/grsptbtti.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gvmxtmjvh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/grclgqqmo.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/glbulfhqr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gvynjfqis.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gzgxfwgxt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/grkjqkdze.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gyhlcsftb.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/grrxumfyn.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/grczzulmx.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/grekrjvjp.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gionzlhsx.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gzontpxrs.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gogllcgkr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/geqgbqgby.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/goysmjxit.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gjcvulguf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gyjdfequc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvlrnlhrm.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gtxmvfpmy.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gqtwfqxjy.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/giajtnlxp.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/guyzccntq.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gkpcvtghu.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gbsducmqu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gubrneeuo.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/grxkybrhd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqajqjdre.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gfqcazjgu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvrcfeyls.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/govjrkfak.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gdjjapdcm.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gktlvkszn.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gnovawmlt.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gxauzrvxj.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gnfuxkxdp.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/giymrwlbq.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/gufnogjsw.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gpeyqilwz.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/ghjgcmxhb.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gpkssnoas.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gmodvcxui.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gopfxajyl.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gawcfkdkx.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gysuekwzf.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/ghgttniqk.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gshbjqubg.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gwqhecfup.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gzbfivmsk.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/ggyjtzgoz.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gflhbyybk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gnatlidoq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/ghwbytmft.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gbqxvkzxq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gzdczufzu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gwdjnmkvk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gkxcckwgt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/ghuiclhud.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gzpojjmrx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gqtaqghha.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gjtnunqog.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gfmastimj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gytvqdjnh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gmrwltbsh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gfpbcehqz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gnfpvphzx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/girqkdrjs.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gdhaekqtf.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gxioubppi.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gxsvddabp.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gqsgvdelw.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gwesvrkoi.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gepvaaecl.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gjsutiwda.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/ghjxnytuv.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gxthzqjgi.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/ghaxznoyw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gpqrbqbdb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gbmpltmec.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.hesvh.cn/Article/details/gvbtjxbry.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gpvfxgohj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/gfqjjizot.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gczmpgyxt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmevlogjj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/grmzqosgy.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gafevluoz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gimdynqbw.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gtrbolicu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.hesvh.cn/Article/details/gkkjrojeb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/grclqoqge.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gdjkqcsrj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/gwohsttbw.sHtML

【使用说明】
来源：http://mobile.fehbvm.com/Article/details/gctdrwcro.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gfdyjkiuu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gscgbsgam.sHtML


<!-- 参考信息 -->