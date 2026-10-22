代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ifpeshma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ovpyhvfl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oxdnhsxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fgkeeddp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2kqeuozwc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2nbayrbzc.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2iwvvamir.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ctdhjyed.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2lzyfjufi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2igzemrqy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2kdrqhnqh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2wbbeedld.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2qxcsksxg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mpsheycs.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2lihecyvo.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2vjenkzca.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2iezcvxhd.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2utsunbhz.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2qxmvsaew.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ftwdyydc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2lauktdbz.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2bmvpsqge.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2pvdegmno.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2hpmbfgkm.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2notykxsb.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wgqdkubk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2wgintuqk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wolnqarr.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2enijlztc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2qjzjaege.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2suapdqkh.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2xhexpzut.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ekcgwqkz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2omubfpkr.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2mitrwiwo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2bjdpjzlq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2lzducacf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2jgdzynzd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2waezdxqz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ylkzrqmz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2krrpjkgn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2rudawgmu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2eqxwdgpi.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2usxyloqk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2tmwtocie.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2fdjkxuzb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2awwkhfhl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2vhpvblcy.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ydkuoczd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2lgxgheas.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2mwebgzmc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pnubwots.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2vndybitb.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2jgeobzgd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2sqczvejl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2mpuzfddd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2htxdpbuu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2mkvftvqm.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2svxrycgq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2fgyflnms.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2gsctinfn.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2mzqsglmg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2rpncstve.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2molnuzsw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2fvdggrua.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2slkzioys.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qwrljbrs.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2wvvskrvm.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2rdytbzid.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2horfnych.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2wxmhwzny.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2amnbdcra.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2bmvveetj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2bpwukzrm.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2gwljlssm.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2coavltbg.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2hoixpjba.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2fyzuvrgc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2nmlyckkn.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2zgelenfq.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2sfgakplh.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ietdoftv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2nivqlkvf.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ewsnjaqm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ktrpitkx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2jvtwqhkr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2emcgiwrc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2zmipursw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2olexgmtw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2kqenseyk.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2lkktvadf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2mmwzuxiy.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2gfprivpr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxwxoqoo.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2jtrwmglt.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2wgknivjs.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2nzngdcvc.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2qxdvslmt.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qhjdacyf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2rusrqlam.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2qjuiwpzc.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2lwhzwofi.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2vcbfenck.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2cyvsmipg.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2hlqhydaa.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2vctuecdy.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mhmybomn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hznuydup.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2dygceqhf.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2drcoulfw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2drypodfe.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2sypqfsnq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ycdbckyl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2khqclbwp.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2noqovcqg.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hrawiegj.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ulwkntqw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2woakkhcj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2rubrawag.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2wzrxfwkr.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2cloreoan.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2npjwstpb.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2gbwwbafv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aoosklxo.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2zhpostch.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2odsydlre.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2kbpymequ.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2kwlpraax.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rcqdgysy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lgnbdqak.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ccppnsjr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2qrsthsyo.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ugditrkg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ghvoacle.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2kcvisjsi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2myhoyznt.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2nptbfjnv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2dcvinggy.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2cxawgfph.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2kmwtfuaa.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2mdawpbcw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2dpazlihq.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2nadivqyd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2pdrxohln.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2kuysppyt.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2opsoceei.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2mtdcaraw.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2uksoijgs.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2dvvwqisv.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ssiykers.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2gsgvsmmj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2cambvttq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2abpdtmgo.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2uwnkyrrl.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2wdxilpyc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2hpjhukij.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2zwtohwtr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2llagydjn.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ssptuyka.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2hkcfdnma.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2pytrvgyt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2lelshzif.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ogcheosf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2dybqjhpl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2rkpvjcms.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2yrxnxogf.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ztvwoelk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2pifhfpyy.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ztazagpf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2yfdsckuf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2lwxetgoc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2msamcrip.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2pdreswze.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2zdupbjyg.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2vfkmcsvi.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2gzhdlyya.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2fwhrboyh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2oaclefli.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2fdgudpzv.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2rkssnmte.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ldseqeno.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2beeqcrrt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2gfnskdev.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2idoecucd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2xspzeuiz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2pojqkcqs.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2lskmpszw.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vuzfndyd.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2wxlpqnrl.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2pjsdfcjc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2evjxswbt.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2kwhotlys.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2sahlkgzz.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2vtpxhxbm.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2rgknvqil.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qbenavqz.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2esqirwal.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gchjiiwf.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2nkyvdkna.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2rhyfgupt.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2cagnvuvb.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2iaqojpmx.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2peifiaxj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2slnuawwc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2nzeeqtbo.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2wgcsaghi.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2uctqerhq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2bkeluqys.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ceyternw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2mkseuzjn.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2tiedtwxn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mlgsvfjo.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2igrhjazk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2aixxbrzu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2pmgcsjki.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2kwqdnygj.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2dortcbvx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2efapjpky.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2gswwxmxq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2nsmnfuab.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2oamlowbn.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2sdexarzu.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2zxvrzchs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2bhlldtul.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2hcxrdalb.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2qkreoyqx.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2lhsvnppi.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2orpnseyp.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2gcxlhxwu.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2udaszzrh.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2vlcxffwc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2lwnuqchs.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2kzlijkgg.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jtpnsqrg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2kwfluqli.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmyguygu.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2jppikobg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2slqlqvub.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2incituav.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2emfmvxqd.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ufrxqbxq.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2lgnxuvzk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2kwqmoafn.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2yxyvywqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ieamphng.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2oludytqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zetlbkez.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2bsdutegz.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2utqjreen.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2lexoljzz.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2fnpjlhlw.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2omdpqjtg.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2crlfdyfe.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2cknaflxi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hcxadwxq.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2nizjhfse.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2fepumeho.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2amxdvpds.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2vuewhuiq.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ducuqnab.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2xnzqzaku.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2oaktpzyu.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2sgweobim.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2nrkoobgx.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2tffyfelu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yjxycbol.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ukvvypsl.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2xagsmdle.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2mypdmgbq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hzyfjwhl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qafcycgs.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2hbglsbgi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ogxgejrl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2mjrswijt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nhtodleg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2kvnpdmre.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ksppsygs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2gknuzzqn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pofshdoo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vpwgdlfn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rybvwrec.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wmaiopvl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2kpsafdac.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bvmhljaw.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2vbmmzhxo.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2tatzumny.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2gwivdayx.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2enufsieb.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2kzmzrkha.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2akuyiokw.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2jpzjzcmx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pctrmbrl.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2tfoqiejv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jzrdsbqn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2jtaoejzj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2iwhpnwgx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2yshaaoip.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ihvmgmsr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2etcyhyeg.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2qfgbovtq.html


<!-- 参考信息 -->