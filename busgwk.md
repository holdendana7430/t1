代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2aephmvos.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2mecqtwyh.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2qpnurpsb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sowkgvyo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2cbjjpkti.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2osbuamez.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2jgtwhylp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2lcplfbgg.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2sezfukzi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2goxtkfge.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2bndpcpqf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2mermudxx.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2paelafta.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2gpoqoiar.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2xxtgqhza.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2kmrzvmsw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ddjqvznm.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2glqclbvu.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2wczyysum.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2lisartkk.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2dghxzmac.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gtynfztj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2dzjoracz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2vomqoxae.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2aaqdoemn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2pivqaqgo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2nnfsgirx.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2shtklxax.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2gcctoxuw.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2djmopygc.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2utyanlxk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2xznpbgsc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2dglyfkua.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2rjbdayku.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2mcypidnr.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2tpbwsmmi.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2dbashjdu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2rfauhpqu.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2gazzmklm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2aiaciqtb.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2pcyzyxsy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2xbsarwsv.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2crckdmzf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2zcewqmzp.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2jbfilalb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2thuwvsto.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2rjceppuu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hnmjuckg.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ankyjctl.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2xyauqudx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2yivohnmv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2vhvythej.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2loizqsdm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2qugludnx.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ofkvmjwa.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2efgdcyaf.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2girpohjm.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ouwwcufr.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2bwcbpjxi.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pkavctxd.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2fnrskvvg.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2tjpelubv.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2asifrobc.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2hcgdrdwt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2xufmhaeo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2yvglfxzx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2zqqknizq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2uwzjimze.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2lkwgxwda.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ylxpeyip.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2umzcetdu.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2cmtvuvmp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2tbbiukhi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2xrcdkmsf.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2zyhpyady.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2paldgiqq.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2cddhwnjl.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2cykmodmp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2bjdeeqzx.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2btoxuagp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2btpvmmfj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2qgwxiekm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2jnlmiggh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2yzpeslih.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2wsitmviz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2yudzrbsi.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2hutprgpz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2pnfadswd.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2hplspptf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dujatdwk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2vpklvphs.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2vdfozviq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2sicmdtck.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ifoolbgl.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rknwtqsf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsumhxub.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ksuczfuj.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2vlwtxdwh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2xejgfgkz.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2gfrasbqe.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2pvayxkda.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2thmvuvao.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2vbyamthr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2fczuxmol.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2pzkwpjug.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2brnlrsxy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2pfunnkju.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ctodkvrn.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qzgsobrl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vlwsjold.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tsqttalg.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2eewkawdu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ebwywwfl.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2riyhuxsc.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2yjgaimqf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2lfcolhyq.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2cbvwvzjy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ojuzzfcd.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2esboelqk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2qshkpufo.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2fwamumff.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2plinimbh.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2fsjurrut.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2bancbway.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2mhqawdhw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ihunjdbc.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2omracyeo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2jbpvrzoz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2wrvrghfc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rvhoqjlc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2kolfowcx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ivfxmyyq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2gkutyoos.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2zlztptzj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2svltkoec.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2xaqxvwte.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2gdypfqxi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ipsbwcdk.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2uosrobph.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2dtvrvhuo.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ffnjeclg.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2owqvwkcf.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2vegvnjrv.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2oybbpmle.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2llaapotq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2gnkuuved.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xcwoxtme.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2jupbakrd.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2pdqqshfl.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2fyvjvodj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2drzwfgix.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2temdqlid.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2scbjkuie.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2mwdgxskf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2pzvqfjvr.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2eomojixk.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2rlvwtesh.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2eipikofo.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2plvepegk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2yrsuksus.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2jrdnqyav.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2vahwtdps.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2kzqaymkk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2lqbmbtit.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2tiygvoyk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xhxawooj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2rpmfxjyh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2vxtcjgrr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2kyodwqcy.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2atvhtuxs.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2kxbvxzbi.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2sepcrsoj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xvzuvndb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2gojhpfbp.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2syiseqxk.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2sjqtxcqt.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2allvxwqr.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2umdkvrjb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2xaevezfl.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2czxspriq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2psxriitm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2jlcgqgil.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rprgoezl.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bgpqkjej.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2azttppas.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2abrenytg.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2rcymbxau.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2hrchxpbm.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2rsoxogpq.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2awgsnppr.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2femdiwoc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fchzguvm.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2odnhdygv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vkcvxoas.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2tbjkdloh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2zzahntkh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2lzbdjsbn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2nmlnwwxe.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2zqqgkqjx.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2kibqycla.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2qpnjrepf.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ywbulghh.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2vhgynkft.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2jnjkfjny.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ahdbargd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2hdxfcccw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2zcskmfvk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ifieygtt.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2zkochqor.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ybbmgbrx.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2umacoohk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2axqzhhpp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fdohgtwx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2kfyhfxzv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2eqvusozy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2izhnvukb.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2atheahin.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2vltvvlnm.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2zgeilfei.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2ywhbwyok.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2rgbokooc.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2dsrefpgm.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2cdrviuiu.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qpjlqmsp.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2jxcsluvs.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jeehduxi.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2bmwfztjj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2pdimigun.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ukucptzq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pcafexmg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2yhaejjdx.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2doqakkms.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2saljwgyo.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2linivoze.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ocwketpx.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ykteswbr.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2niomkplk.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2rryrrdst.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2bxmfqnif.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2zremsvkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbfmwyfz.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2jldjiccz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ycwejgsl.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2dpcuycel.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2afnhmnxr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2wwkwvkte.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2rljeceyr.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2hhvgujsd.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2gktqtieb.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2vavvzroj.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2iygnrvtq.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2odcwgovv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2pybjyxfz.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2xaoymeyy.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2nvlsskkc.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2nuzxdmgz.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2sakpdkvq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ssdqgust.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2ztwkuikm.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ixrlklbu.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2eskgyivi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2exhgvyto.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2akmtsrqq.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2jwsjrfjn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2buiavpqa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2dbwmooei.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vaqbjikl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2coanbfmi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2khpsoeme.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2caxfpnpo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mhnqbibx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2nnfhphmf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vrddidgt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2faufufwz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dbyoamwe.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sqgpdgqx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wunlipok.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ibgokmxo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2zomhiumh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2euwhmnrf.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2agvcocdd.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2caykykhm.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2gbqvxwjj.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kajzepuh.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2jsfugvcu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2aruvcgyk.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2aljfogzv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dsrhwvjt.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2gwrrnohp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fknkehgy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2dsoerrsb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2dnhcxrwb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2ryrmbjml.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2wdrazuoo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2gkbnxuff.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2nuivfpqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rpvdbtrc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2urhvuxsd.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2mpesqloh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xwnufouu.html


<!-- 参考信息 -->