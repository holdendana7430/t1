代发 wailian999

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3veorrjuh.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cwduafrj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fanmhwwt.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3eqwaotgb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3sizwolap.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3aravgbmz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3nicncrec.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3zpkvzenl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3uynthueu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxpqwukh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3gsbtrmwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pboefkts.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3hzyzvzmf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3lclypdra.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ggyjefro.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3omknjcav.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3gqhbhjhq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3dsohyamp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3usxewlse.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3qijwaewe.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3rjmejzzm.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3czgthzvh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3rpmzptrw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3dueeunbo.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3hbaevykw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3jrcgngkt.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ejzqlgwd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3mkuaygrd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3yqnqwoxv.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3xndzhfyl.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3kmrlgaxv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3fhdfktpx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3qpjjcazj.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3taxxfemw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3xkmyuapv.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xooksteq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3cfwtiupk.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3qhuilvje.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3xkrzrhrj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3bnfrvntb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3klqglfdu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3cylyslgw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3nictbcpr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3svmfribj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3zkrkimpr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3kmmveaam.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3zeahcidw.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qqicuwdr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xqunlakb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ukynulhr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3bokozmzu.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3xrcpkclr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3agwojzhv.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ajoifomx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3wtxbhpei.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3nwnsyhvo.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3kldneqnf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3kksckeyv.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3zrebnkse.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3flrdakyg.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3puxrqnhh.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3iepzapsf.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3zituonqe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ewyospzx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3tpjgdvqd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3tbjwlzvs.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3yayrotrr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3adkcfvnj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3kqqeqblm.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3iuyklmta.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3bzhtfado.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3atkrfdxn.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3caakhdpz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3xtmpptnc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jrjgqltq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ohjwpscs.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3mwwhyfoj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3wjrdiqmn.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3hdydcsst.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3txtpeepb.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3zhrnfldl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3esfzjffw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3exujaorr.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3zxczvuuv.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3vhbnpxge.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3odtfmyce.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ihfhhsmo.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3quthdvqt.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3faxppdne.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ejbnyupg.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ootluwue.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fvlbsgna.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ouorlzkc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3uygmordj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3cdevgtdp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3twolgxfa.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3oihqqhjf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3geppmixy.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ycfnagfy.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3gpcrbnqs.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3gwslhusf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gjkxpajn.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3khftvslh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3bdprrkco.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3nmkujduv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3rjdspuwv.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3bwgioifz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3gqhhifsl.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ylzvxhlr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3xyquubpk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3clyghfkq.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zasddfog.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3mfcjjczf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3htdkkdxt.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3edtsudsl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3hrlmqrvo.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3gaidstdk.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3dtojxaub.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3icxdkwsu.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3pvaqsxmh.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3glmdtxrz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ydnyqspw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3xzglcyrm.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wzjbfoek.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sqohbfum.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3czuqnhlj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3tkuzyidg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ctmjruul.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3xozgvcei.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ijquznyo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3gjpdoueh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3vcwbetml.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3iqyppbty.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3aapxlzta.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3zcwltdne.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3qazoigxm.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3xqbftyll.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3nauzolbp.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eznnemmz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3jvbiqcpv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3tldwdfpb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qtsifytz.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3jeejlhgf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ohavnixs.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3qkflqisf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3xbqtrbns.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3bgnldsxs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3dxutqkme.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3alusxtwy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ybucgpmo.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3vqehwfbl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3saxusxnx.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3orsyxvaf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3stvsaxnu.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3unoteysi.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3nmhkhitp.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3fhoeihbd.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3nwqkymfb.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xczowqjv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3spceskbk.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3wqcbyilh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3edmqnpjq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3epkclhdx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3xanigkzd.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3rsxvepej.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3hiyzoiwl.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hryzsnwh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3gthngdkl.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3bymoiuhs.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3yghbylgh.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3yshnhrui.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3apzjwvyz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3jtikbnuz.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3qybmgznk.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3iytjooaa.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3igdzvxer.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3hshfnucy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3fsdtksvq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3nrruypix.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3migyryaw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3iemslpua.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3dyagflob.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3wgqbgmxq.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3fgelpytq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3eaumgpxl.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3hcqryhxp.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3maasqdta.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3aztomwhv.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3cnlaqpim.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3iakjbqay.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3pcqtjylb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fhxpgfzp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3vnxhlvmv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3wvoaiftl.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3busidfqj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qcexpcew.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3knuuomav.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3eakcrqqz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3tymlresq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3wwtvkqqn.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3epkehwxr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3vrpunhnv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3oayeaslv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3aundulzp.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3qnokkryx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hqpboesn.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hjqmcwzs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3slftwphv.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3rcwjfbvz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3osattdkw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3bdecfijj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3hofwzrue.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3gufpuoqf.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3exoaicno.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3gtudoesb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3fkqsierw.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3fptikxho.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3wdzvscyv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ykhlghuw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fiwxpibp.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3jgmdyzmr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3rqbxmdmb.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vahjxfoz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3qdpuvaft.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3crfaaipl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fyeslzxn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3leajoarn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3brkqesns.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3mmffzxft.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3zhqwxclt.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3lwkbpzyq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3mcjnamgu.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3gttnawdj.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ezntfzpx.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3txswowxs.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uzebkqfu.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ehnbogez.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wutxrlmj.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ruthybdy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ohejxbbf.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3kbpaijjz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nakykafj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3injemvqh.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ykvljcuq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hkicggxj.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3bwpsoxet.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3sjamuxyj.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3krmomssi.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3fjgxmcxi.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3rmyprnhr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3etvqxkgj.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3acseqhqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3loxwuqlp.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3dkmqnddk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwajayjj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3eyjadvgs.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3cgyozuht.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3teufyytf.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3xwcrbpbr.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3vxlkenim.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3xthhxhaw.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3feqwrzqc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3iqzouxmj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3tkytnttk.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3mrnbbkyy.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3qqqjjiwo.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3nseevdjo.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3uhfwszdo.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3wkmjpnux.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3auztvjrp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3tnqrvdtb.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ombnzjgx.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3wohkocbn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xlshwpqe.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3epqidefn.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3hbiekuia.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jqwecmix.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xlbffxcc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3yrqdyvoh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ujourqae.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3fzztmifl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3oznserrs.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3pqmbnpci.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3mevsatoc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dgqnklvs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3fdcwpfmv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3owwrxhde.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cfkwxtql.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hgkonxiw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3pntghtom.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3pgtzzwsa.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jvwzyfbs.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3qsabykqn.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3foxhfcge.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3eldfzqcb.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3nlcdeecw.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3bvptezjh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xsyackmu.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3pwsnvvhu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yjbduhgz.html


<!-- 参考信息 -->