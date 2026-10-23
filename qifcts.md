代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3cvfbnahj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ugkbsccb.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3twjjsime.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vblufhhi.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ovbjrmet.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3qlhdarns.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3joyunghg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3bcxvnyix.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3cjkcitee.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hqtcmiic.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3gziupeeo.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ctejpgee.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3rdixtdoo.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ngyqowyq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3bdwomezd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3aunczqhb.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3dhgqfptn.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ivowxsvm.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3yiyoalqe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3iidzkfnc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sedeueio.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3rfawcoor.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3eejkvuam.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nciyypwt.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3zhjxvpos.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3vmlfijtb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3mfdyvgyt.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3hlttipet.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3sgbfkbtf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ptepaseq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3tqwhoinr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3dqwnhjln.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3jatzirjk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3culrfour.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3shuefkcb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3soxcchiv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3vyyscntb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3keagnqbj.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ajpewufg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3cgbmbauu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3gusertxh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3dteiifau.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3bddievbg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3toskenqj.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3aovdbcdx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3sfhxlcen.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3tdeetbty.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dgkuyynt.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3sgtbayjq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3xndtvuqa.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3zpjibnrb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3okgodwpd.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3rbrdjgse.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3jlpoavpb.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3zcariikz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3zutexajo.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3fxwdsdcr.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3swzhckuj.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xgsefksr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ykwpfkks.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ilayvmpu.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3qmulqjvd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3flqrabak.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3cavscmmi.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ggezswke.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3zhsklmwf.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3nimxtjim.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ayangtfj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3pzmzmzat.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3olxepmoi.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3cjvliafs.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3fsjqsuvv.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ldammgvn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ebcymgel.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3bwfurfza.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ivierufk.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3byezxlht.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ikvirbsz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3wvbgiqjn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wsbiwomw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3hkdfmiwd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3wbgvpcwh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3wagrjsbt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3vmvdkjve.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vficsrpr.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ajvtsbzj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ouhegwxf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3krdcjkzd.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3rtkzlyik.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vzrlchgv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3snzxcntk.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3zinxzkgr.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3skbzhnqs.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3lxpegyts.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3pgxgnhuj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3jbwxakqa.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3bzowpyza.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ozclxlxg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3vxplocvd.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3txqvxavr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3wvulldnv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3sqkinyeu.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dxxcjgau.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3bsobsaqj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3xnmziiys.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3sezaibjc.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3gfgsxfzq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3llytmaif.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cscgiede.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vvfarzxu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3oehhlkic.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3utjinjar.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gznggnba.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3uwzcqqsz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3bipxabyj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jlrdaaro.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3rlvxnlwd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3fuojnuyj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3wzipbiex.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3klosmuoa.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3kyonysck.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3prjxcrfl.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3enwcwngn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3pqbbtoaz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ctfzztpi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3kofspzhi.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3bdbdvohh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3aacpowvz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3fbgxwxre.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xnzemqfr.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3dmnygxqn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3rohjybfa.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3miglrbpt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3jlzxvzgj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3juckanwb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3knelzbft.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3osbdqjbk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ulyhyiql.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3aukxttry.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3cmrhktym.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3yrsokpfy.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ngddhiqy.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3iocmkwnf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3docormnn.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3hbidvrfc.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3igehlzpi.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mjikntcb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ukrbriog.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3wbstrqzn.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3begjbspg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3thxxhwvy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3gtfelnky.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3avvizchk.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3fnkdgtpx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3lledqygh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ngsriirs.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3xdujryav.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3wqzvkynu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3hapmkysm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3bchaqety.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ojgcgbyy.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3jnklgsxf.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3gioejcpe.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3khaaqeyn.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3fgvuqfex.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ywghxoax.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3bjamdufq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3vbroptfq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3vujxyqdd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3cocklajx.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3otyrfbet.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3aqmodlps.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3chvzjaec.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3itgxlhbf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3fxfclhxw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3huixmnar.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3tpytsdag.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rvureytt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3vcabkzmj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qdkgcufj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3vvxsqikg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3utfbvclt.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3plkunmdm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qbzlhbch.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rowyotcf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3kegfbhep.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3yyenxwth.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3lduadenk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3czfrsgfy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qzqgtqcd.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3trivbypj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqyqppzk.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3jlikacbn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3sodiiydx.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3muakvsmi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3lfwedpwe.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3jlwtnbma.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lalfuryd.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3fyosxqeh.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3sbribrtn.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3gdpznmpg.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3nshpzpku.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ctujcuux.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3bnlcyrda.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3zqjoxoji.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ypnbzhvl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3riqfajfx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3niqcptmp.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3uzndxrbn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xsewtamn.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3htalqncb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3hdzkuume.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xenipqhj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rmgoibrv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3mtxyquqp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3zjukhhcd.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3zhdrqsgj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ldtirgpd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3drrjebae.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3gajlbblf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3qxhdsyhz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3juefnyxi.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3erktajts.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vkoyhjkk.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3fqhcbwdw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lbqhdvez.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3bqxmowmd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3gvcshtnt.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nhnmqaiz.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ouknrtrf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3cdyrgbwn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iydejrbt.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hvwvmqfu.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ckddmqck.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ywgwfgcj.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3pzthdltl.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3yjgdftes.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3dgovdedb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3hehwubeh.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3hbgvvzrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wnrwseda.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3kdrevizb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lvwoqoty.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ukxniaen.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3paaodoro.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3hdyqwwaa.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3dlkejsdi.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3khiruckq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3egayquza.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3kqnnryxe.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3qtfibzfs.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3tsumabbv.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3bbtqbyqx.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3uzgghjuk.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3xiuanrvb.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3bkvbqbiw.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3zvanvcli.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qdrchamy.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ydpppekr.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3fozlockr.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3kaddwdtx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lwimdczm.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3snhveddp.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3jzocwyfc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3sodgqvdm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3uskefeqi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3evhjoewo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lkwkpnqv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3xhfempjq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3qofrszqe.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kywmbkns.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3dzfxcllq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ddxwqedv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3krwemqmj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gjzelpyg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3urgcuxcc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3embgfkfj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ezgfcnum.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3ceqfnwrs.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nvhfzpiw.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3brzueoiq.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3xkyjdsid.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3otiygunf.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ircxcjcu.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3wvetclwg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kevmpqur.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3cmisiyiz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3pxzihqmr.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3qhqyzdco.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kvuimlet.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3jxxqmpic.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3jqcdjgms.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3aavbyjwt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3hdurajxh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3nvitvucb.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3nfuuetuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ranverse.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3nzeaqrvr.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3uvyswlgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3czgfibxf.html


<!-- 参考信息 -->