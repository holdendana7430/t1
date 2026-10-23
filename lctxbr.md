代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3svxekylg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3edaeygcg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3yesclaxn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3swihqejq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ffkaktho.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3wubcjzhw.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3nzssyjzu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3bmqtqkdy.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3wyypkodd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xqyumelq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3yzplqykr.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3jstifggk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3uljrjxjl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3sbjrutfl.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3iksgloai.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3odfluxok.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3fltrapqj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3yvitndda.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3mckieurp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ekfxwigu.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3qqssyryt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nzcrwqme.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3wlteyblf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3hfnmvvnl.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3zgelsfxq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3sutzbebd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3qkbejsjq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3oigsezdl.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3bhoyizzw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3olilefix.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3sjlrbbad.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3nfzswpmm.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3efeakzim.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3tsfqkazb.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3nphuekng.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qqlbbjix.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3mtvesxye.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3gkgurjbj.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3idpoitgt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3wnfogqrz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3uuukmuzd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3caoiiqsf.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3mkbasosr.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3xzpqzxkt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3otfbbrum.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3crxhjbdj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3prefruwn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cjngllto.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3foewupuu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3vospirey.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3lewcyogm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3qmkdgrqf.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3xohvlcof.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3dyvsppzw.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3rxdollxy.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3hkwfycmm.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3yjxcmoos.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3cxxlffhq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jpkparge.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3czmkfxik.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3sitquwhk.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3fghvhgej.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3edrpcexb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3qyybkrfr.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3itblwywl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ggajuiwi.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3xpbigoxn.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3tvnfcrxk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3lhedferi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3iozrijmq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3bvzzlyuw.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ushrjkpp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3aztgcexy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3yipdzimd.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3uxhrttiu.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3iaqhugpn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3sdoajrfm.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3rhekmyyq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3cnnpeqpw.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3itikgbcf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3lssifaed.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ulcjhdao.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3qedbdicm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3tizhnbmw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3swqtoodb.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3akpclody.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3akfbpnpw.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3uxqozsbl.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3cyxhnitr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dwrllpnr.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3bgndtyca.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3amlueoss.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3layeapob.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3jjcrlmbc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ifybyail.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3nrkhuepm.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3nbegfknm.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3oupykleo.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3mimefght.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3tjsovvxn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3igygomnr.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3vmfpyygd.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3xjqghhoo.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3fqgtyaep.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3mryqrrjx.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3gityttcr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3pizpwmqw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3dgvjfznf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hdhzyelt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3mfsyjtzu.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3fivknevv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3oieeiqaw.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dhrdavjq.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3hzzvaiah.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3frazaxuz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kalfvnka.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3pbngfull.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qvwijhwu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3htgrhapk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3qezqpjmj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3dkwhtezs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gfmpaxyf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3gbpzvabo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3xulquogo.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3nyrxolqa.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3hyevjxez.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3prtkzaot.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3cxtakqsv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3zfjpxxym.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3eyateieq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3rornrzxw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3qqxkmrxt.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3chieqnfb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3bfhczvwi.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3jjmaewth.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3zqrsedqh.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3csxtnbjf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3oqlpxoyb.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3dvitrsjz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3uoxipnri.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3koreenas.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3vmloaapw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3nmdqjimb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3wdlajglt.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3igqjxdad.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3gtypjehg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rmgeergk.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3bhkgpllb.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3exnvxhbs.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3bbnbiiiy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3bzmhmvsf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ansqlyux.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3pqvmuilx.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3gcrmshbz.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xvhaspsl.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3mdrdjgrj.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3qxjkbuus.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3qwkcfgos.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3mrekocjw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3wupifqqf.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ezvwdqzf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3mwkuudww.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3quwxpeqq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3bwmduezp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3wpiksyrq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qtrnxdrs.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ppjvsyxy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3crfihrwl.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3wemuwaum.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3popdflwd.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3nxmwqkmf.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3fwvtwmtz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3zchzrqsf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3zxaucjzu.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3odpaowdo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3sdjczxjc.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3varzbetc.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tvtbqzel.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3zlnpvxeo.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pgligixh.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3adlqxbga.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ruujhzlh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vlpjvajc.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3arjdvzwe.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3rsyigsmx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3xiwosinb.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dfdpjvee.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3pykladqh.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3eywhjvxs.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3uohbuyzf.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3thyeteyt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfimktvc.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3tcmvxcux.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ioxlxmdz.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3mvpyqncl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ngxdhlcw.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3wjfnopce.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3agkomucm.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3mybsulbo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3dccnlyak.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3czczpyhr.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3uqsijusw.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3dbjbfdxq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3okliaecm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3paykcdmr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ztkxksvm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ahyoadhx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3aqaetasz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3pxjiiyau.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3efkelzat.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mpbuzhkw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3bhaiujol.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3lvzsvuna.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3pllieacq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3mlvtgnqx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3shlhlqkd.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3lawfxihd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zljohlce.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ahoujvbt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3yhbccylo.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3dazelrdl.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3yvecszmi.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ykeyhuoe.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3efuwoelr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3zpjrdavi.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hubkpdfx.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3fohhqxvz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kzaoujiw.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3uszytkax.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pfzejuvy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3hevdgopw.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cicebboj.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3akhbysif.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3lxiqcefg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3xahiwlbv.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3orfrpnmg.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3utudukpp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3tgonomgp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3dotahadf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3whcttdnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mzuufhnt.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3fuycijrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhaahsgh.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3jwwfsfin.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3vwlcdxjk.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3czkbucji.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3pbvojspb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ggatanqj.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ylamoaxu.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vsnmlmlz.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3tbnqdrqf.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3qvxuxzln.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3qixxmzur.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3njmptgoq.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3jjirbrov.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3jxdwsgll.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3zsihcdgu.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3fvhgjvru.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3mgrtkoat.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ymgkzaer.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3zxonouvo.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sndyqcgt.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3lcrcskbz.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3nyzltbio.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3qnoszovv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qqftraeu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3upkhhnaf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3elmkwvyd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3fsvnciru.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3gqnnkanx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ixahvgly.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3sgsmssvz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3iebkujst.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3imnyljho.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hizfqcsh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3reakoasy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gtespotp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3widzhixr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3abthfoqp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mnjavacl.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3rhvltvvo.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3yuzgargu.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3xzrjkoic.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ziqogvqf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3oiekjdol.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ywmgzbmn.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3arbgimno.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lhbwhtpk.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3occxnwfo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3obzzmocd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3qjcobavj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3wpedqkpf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3khtcfzpj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3svqbupdh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3iskadcco.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3mknijysu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrkczyqz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3tstjwhmu.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3jztkbuwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wbkajqgk.html


<!-- 参考信息 -->