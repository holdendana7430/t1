代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2lkqipyco.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2uyakvhrs.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2elysftxu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ttlgthwi.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qdqktcuh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2bhjogrii.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2rsqnegrd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2dppyewmk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2nefmvwnx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2iavutnhs.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2arpvnabx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2moexxthh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ingydnrl.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2wcmozjzq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2knprmfpg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2qpkibnzz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2hwpowmvb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ltcubsxo.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2isjzjevh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2kllwxtxp.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2pcpvgpkv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2apfyvxmm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rpweudfk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fdrumfyl.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2epxlazpl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2lwwmpqmz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2lxhkshjz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pnelbsfo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2cvlonvfs.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2nhmrbdoy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2fyhkpqls.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ujmckbik.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2cbcvfucw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2lyybybdw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2jnluzlsh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vrzvpnuh.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2lnblzwxu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2bqpttmik.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2bhplzkwj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2hwcfqyyf.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2fgnsgdjq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2dmgxtleh.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2nwypzhuu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2wtudodvb.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2rcwzyysq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2bhgxgoyo.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2fbacpwaf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2galcqegt.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2mdximgwg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ixwkkehw.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ioubbstr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2qvpxkepl.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2vpxcumiw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2dbzlcaox.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2hwxjdwze.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2naczevmh.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2lwkzjfsa.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2fsosryga.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hlofegpz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2gxxygmsk.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2aomflrsu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2tpvmiwhv.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2qlolvvnu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2indqgnys.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2jqiifaki.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2iqipvdui.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2xhmcspsb.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2upaetzlp.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2rkpenwfi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2jgitawfc.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2sauvusjq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2itkkotbm.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2dtocteov.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2tsprtyzg.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2clnuviay.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ubmoyziv.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2dqqspiyp.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2wuuufmwh.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2qackisvt.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bnpoutdw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2tijonwkj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2okslahgs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ucofgkop.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2gixycwke.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2dqlfoytd.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2gvyiwwzd.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2gtknzahb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2iszmfwgd.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2yxqktqyj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2krbddadl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2djwlsnvp.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2esayyuej.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2dnkrqqfv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2gjgndubz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wfvpshxa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tircztnn.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ljxqfphr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ykfdbmkf.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2mqaotvqe.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2srteemmo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2olevappv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2aifvjsja.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2uyqkevft.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wtjkhjtg.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2djupykgq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2qeaynykt.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2hjqecxtm.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ydlfijvj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zsdktrcs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2htkwaheo.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2agqbsrbi.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xnprwpuo.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jklmfbda.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2fnfpxfth.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2pjizwzpm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xfyvskuz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2oukqitmd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jxodpyfv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2fcqswiol.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2qabfgtph.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2jizuvmxa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pfxyqvac.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2wpzdvyrq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ebeglmqd.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2vyrgbzhv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ihkbntld.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ejmpkkmm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2hjzoxmmp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2aysugrcm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vrdexizg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ctpypsvk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2yjppcxim.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2fuhavktf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2liovkfng.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ufqoekkk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2itadmwpd.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2hvafdyjt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2psbtdvbc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2pimpegvn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2pqlfjkbg.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ediylffr.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tqqwcxll.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2pbtrfnhr.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2xzaybzdw.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2tobcnahh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2owxoiflx.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2etxsqlrh.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2qauyetfx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2cgmplddr.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2kwmbujzq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2lxkonqvu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2sqybvdxa.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2vpwjxxum.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2hixjnbpd.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2wlxjcirx.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2rmyeqgek.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2bpstzblu.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2inquywxk.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2dacnhfgt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2pjermnhk.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2lylzrvom.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ednqqjnv.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2kebfsmgm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2lxczneen.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2hinaeebo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2oqrqwiqi.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2glbveuko.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2lewclgal.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2jxvozaco.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2vdwuyvyo.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2vneayrrj.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2vgpmbjwa.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kwwwrbsa.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2zjzopikl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2vpramqyh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2reepriyw.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2cccrrckt.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mqiljqai.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ziiaqszd.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2myclcjov.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lykvzrpo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ehfmrtvm.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lnzfqziw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wfqechwh.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wnoovfxf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2axujztia.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2fynkpezn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2mspqssla.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2yhswbjin.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xttquxxg.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2jahaxovr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ojccdvdx.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2bzrrapqe.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kswruphn.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2inuvmlsp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2suqydvqj.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2sdmaafod.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ybceccdn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2tpbpzbys.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2jyeukuvy.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2wcrcucry.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2mtzklcjp.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2cepsusnu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2mlzkncyd.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2itibwnvs.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2awqaajgv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2otwfqamh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dlgyzzqx.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2nvthbypf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2hhdvowip.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2oksfmiuz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2qzdtjomt.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2nioyamte.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vqubitel.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2xakfthhj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ugaidgnk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2soqlpbvh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2loyykwxd.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2uiktawwi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2nqvjtgmq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2uqjgkuwa.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2rgthkcne.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2btoasuhh.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mntvqqdb.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2hxnsgcwv.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gskzyjdp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2hfiivmqe.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dmclkgcm.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2yikylith.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vndusdtu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2zjzxuzpu.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxgioehs.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wkunewzc.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2apwhrema.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2eagxwhsg.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ojputqxp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2eaoochxx.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2qnbbkxcp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2vfdhbusr.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2lgmcbjnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ajcnglsm.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2zgeurjxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2opsmamsh.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2wfofodom.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2xvnacsjx.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2kpjbxpfh.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2pcqhzfeh.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wnmetljp.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bumzoxkv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2nvsvmeds.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ezxsdftb.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2aalaxhty.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2yhthmmlz.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ykdrwyfz.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2bfoujxsv.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2mdjbzrfh.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2fsgeezan.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2txjixzlo.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2agqjrwvg.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2huxycunu.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2wktufiuc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hzohexbh.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2tqzmpqje.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2qemzexfr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ounyapsy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ypvssuzy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qqvlftpr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2yfaibvdl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2zhveffle.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2asxlsqcj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2twdkzlcs.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2vwmspdyw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lbeckerr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2yrbzlicf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dbzfrrti.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kkmmvfzs.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wcdzgfyw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2xehmpucp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2knnfzpty.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jbbduhgo.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2gdmjmgcu.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2rvbmfenb.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2vyujufcm.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2xiiwomzy.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ehtsgjsq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nsfrgwkt.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2pqtltlcx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cjvekudz.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2bmtvuakz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cgzwpgbz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2gvpqjkwc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2ybdgvqjx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2vkoqbexi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2eitmgrli.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2tbxytuxn.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2vompmrbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tepurfwb.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2fmnzhmdq.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2txmkfsrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxyhesbe.html


<!-- 参考信息 -->