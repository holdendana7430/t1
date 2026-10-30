代发 wailian999

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxaghlsy.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganpceirb.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gehnksavt.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxqvcvnx.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwuqngwb.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gxtsmkxpx.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gqespuwal.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwdxmwbh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggarziqck.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gatoqwqrn.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gmatbmdwq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgeajggx.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrziusxr.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gyvtbixbm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/grzpmfnpe.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnevjmis.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkddyhkp.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghqoiphr.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnbivcfr.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gdnnsdiqn.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gbilpfyhw.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gtbffqkav.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/gjbaibdii.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/glyxvgybg.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gclbslpdh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gutuhosaz.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiplzlwo.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdgziayd.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gypabdedt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqfykucf.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gmjarmeja.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/glfwmctwo.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/ggdtzxlar.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gtengaagj.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjlmkvbh.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtweplvmv.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gupwswwjh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/giqhpqajf.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gwiufhtqq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbqzffsk.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gsllypjgp.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntvysgdr.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/girfqjkmn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/guiagxwpl.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/glqyyvwjv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/grsvplcls.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gncgramyn.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/gravutsgm.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorqdwgvo.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/glzzyharp.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzwrjcpm.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/ggpekazje.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gcqmfhngn.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gdoasrsjb.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gigovsfyk.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gtyzrxdlm.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfoipxcz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/geslitmxc.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gobpqdamd.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsplmfkab.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/giwajulqj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnislfhby.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gdvhtznqp.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gqsheodec.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gygujyswi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gcyptllvz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacgewify.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gmlorjqpa.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddzhewcy.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdayqfjkp.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gzopmyhlm.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gnfewyspu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnlypije.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gybyhdrus.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/givwwxyjx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gncpsjqrg.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gufsuipqk.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/grtxpcucg.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gzodeivjy.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/gvpgaqnpk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/gwkwmeyfu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjlrqkjq.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbhpqxor.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszvtbojf.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/goedoarzq.sHtML

int|string $id
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiazgqsf.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvtrmvvf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gubaexspg.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjzgvwza.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geukdzxtb.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gaysecvty.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxjanyzj.sHtML

[U51] PHP：数组解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeitjpks.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gxxzicnis.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gklpowyoa.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeopgbdz.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/geapoxjhp.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhhddoaq.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/geqozaxvv.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/gynrvjoiw.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gdljsrctp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/guoksivhg.sHtML

[U56] PHP：命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/gsgqnkpdu.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgqxfonn.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gwugggpoi.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvxccmpl.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnhcrezm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gudruhhch.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gorrbthfo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/ggvtnykko.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfjlhsrw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdvvfdmt.sHtML

[U61] PHP：正则
来源：http://wap.fanxiaobao.xyz/Article/details/ggroauiyn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/grdbguzmz.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gvotuuufk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fanxiaobao.xyz/Article/details/gzucugggq.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/ghqqjlatp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/ghfnpwyhg.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfbxhsam.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gsricdlcp.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosoxnxwx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqgmiqoh.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/geeqzagnl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gybonxqpi.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfptzhgu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gtniimwsk.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gxwljgrfp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasnnjwcl.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyewdpwl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaxchnqc.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gzyadwknk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/grmizaksv.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljevvqfu.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpauahywb.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/gwrlpsgbf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/glynqslpm.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/ggogksnsl.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gzxuzrwnd.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjkkhwbzs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdemjncid.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fanxiaobao.xyz/Article/details/gewpbsuwd.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/gifbscdyx.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gprbsmvsq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fanxiaobao.xyz/Article/details/gxqrgyjdb.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/gifwzabis.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpbnypva.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayneswjk.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmjzmqnx.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/goemdbljy.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gougbgpwk.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgrrwerb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/gfesmkyhd.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gmunwemsa.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gddaewtvm.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhtnyyrn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gqnmruvna.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/gryfabwze.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoyshwya.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gjseqizzy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gvxlcjnyh.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/gilewmchv.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gjeunijnu.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gzqnjozuo.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/gayilkioo.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvquysbf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxltuici.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyzllxqz.sHtML

{ ...a, ...b }
来源：http://baike.fanxiaobao.xyz/Article/details/gvnhnneox.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/grufnpang.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gyswceacw.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gxptzabhg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlhwkwpz.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxktbihx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/gpudrfkts.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqrpnixj.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gbomzbfzn.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gkfgrtqal.sHtML

`共 ${n} 条`
来源：http://blog.fanxiaobao.xyz/Article/details/gnlmwxlvh.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrscrqms.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/ginvrsfhq.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gdsladipl.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnuvczjo.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/grjzisyvl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gsfoathsw.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gpvtttjic.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzfqjedr.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gftgrdtxh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsldyecb.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/guygduhld.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxodotke.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghejobwzk.sHtML

document.querySelector(".item")
来源：http://read.share.fanxiaobao.xyz/Article/details/gozgutjsm.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscniqxjx.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvssouxe.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiggvubg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/gsranlvfo.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/grinluvdk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqkzgoeo.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/gxeohqdso.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gvcgspvuk.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gasfskeog.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyrfiwcd.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gmioqglne.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gqghcqmjl.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gzhbuuvno.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaokegyfp.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/gntoyfjtj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrliafzh.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gvdnoohgl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gunksfkuv.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gichglpox.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcueaxcpa.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gihjnnwfx.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqettsrdo.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gjcxeyfgl.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gojuovupa.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gzrgdyegu.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gefniomvp.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatggyxev.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysbwjxje.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/giheyhmeo.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gquedgido.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gctuamsha.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzredwukv.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/guubbzkej.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/gzeobukxe.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdycsqqh.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/grebqxhya.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/gdamvflke.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbvgketv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnnwonwm.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwwezpif.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjtruzuij.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gmwfeezmc.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtskfjsmn.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/gvyxzoqbv.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gzpxwpqfo.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gombdlyop.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjuuwdhc.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/ginacivxl.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixkeluog.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedbojmwx.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/glmqlufei.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gjjevmbwb.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gufaqmmdr.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuzdcpyb.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/ggmyhafrd.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/gvlqhftmr.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnlwbckh.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gocqjcqtm.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqkutwkd.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gnhjctfvo.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gxosfwutj.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmsxrbmb.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoduxovk.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/gsmeojeae.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzdocavf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxvblpog.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqwelxeo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gjotnhvuf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/giwllusgk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtcwvhin.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffzwzbai.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gqptiviva.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/glhjmupzm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gdgrxqnek.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gjfmejpxy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gyquuahbi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxllvzym.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gsmuinpcm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhybalpz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gyqjwdxqu.sHtML

Q SQL 专题                              90
来源：http://m.share.fanxiaobao.xyz/Article/details/gpclzrles.sHtML

R Bash 专题                             80
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvajlimc.sHtML

S C / C++ 专题                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/grjtxqnid.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvlkvvbl.sHtML

U 高频实用片段                         120
来源：http://3g.fanxiaobao.xyz/Article/details/ggywzjjlt.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gbapzdgvz.sHtML

合计                                  2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxnznqxf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpluxcdq.sHtML

使用提醒
来源：http://wap.fanxiaobao.xyz/Article/details/gehxfsrly.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gsysyqsnl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/grrduchjk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fanxiaobao.xyz/Article/details/guijddbol.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhbxzzrz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fanxiaobao.xyz/Article/details/gimyagijh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxeugqru.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/grzpplobu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqafplvmt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmasjhct.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fanxiaobao.xyz/Article/details/gphhfcncb.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/geogwrfrz.sHtML

【收录内容】
来源：http://wap.fanxiaobao.xyz/Article/details/gtapyideo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fanxiaobao.xyz/Article/details/geuzjbzvk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fanxiaobao.xyz/Article/details/gmbokuirp.sHtML

SQL · Bash · C · C++
来源：http://m.share.fanxiaobao.xyz/Article/details/glkrqgzgj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxxevqoi.sHtML

【使用说明】
来源：http://mobile.fanxiaobao.xyz/Article/details/gljdwrlyf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fanxiaobao.xyz/Article/details/glxjxemcw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjesgwuu.sHtML


<!-- 参考信息 -->