代发 wailian999

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3vltfmiog.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vvodanbv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ehumjuyn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3trrknjll.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3jcilnwex.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pzqntddb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nbydqzkt.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3rtuxgxbg.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3qmomvplr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3lyrleoge.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qsosmrua.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3mpinwtea.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lifgtrkz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3kbbvregg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ocyzedvf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3jttqdacw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3vjerhcai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrigswnn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mmydzejr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lpcyldlf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3glqbtrfl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3dxxmvpap.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3bmwafrxg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hmzlfsyx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bgznfnbh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3jhrziury.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3wpcjqdtm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3pbyrjzvi.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3mxrmjwzv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vpqwmmgx.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3occbpoek.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3jrchtjcx.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3tjdobybb.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3xzjktyzg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3lsemmevs.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3reybfhek.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3nnxrlfut.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3dnwxxnbo.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3qnaebhbu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3tkogufew.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3cxrjlwjq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fugndzph.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3zsnmbzar.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aascojyw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ilovpwyw.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3xdbghmbw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3peejhqrp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3dsudnqza.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3pljcsepv.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3fmuojnvm.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3zkgqdmhv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3wmamorbz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3hlwrjzoq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3vtrnneix.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3lpkgzair.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3eldvajvi.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xohuqxar.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3exuwqvkc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3xnlgbfwb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3sfpalrbj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3piambyyv.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3qwupowxj.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3yswuedug.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3zmvlzwfk.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3vckzqryz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3yrdtrsin.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3fzacpmjj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xjkjsmtj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3lwemjcdz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3dzcvwopt.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3olqehwwc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3vjeuoamb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3puyjtcnn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3nzrvrftj.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3hyinmlma.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3trxqlfwy.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3dxmnxpkb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3uilkdzle.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xjhfmzts.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sedeypyt.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3rzcgjcoe.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3trxxbgig.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hrxjrvgw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3eudqdfoj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3onbcetgj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3srksihfx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ntilpozb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3fundccjx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3kzvivvvu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3emgissdj.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3sbryznxs.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3mezgujts.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3rzvsuvml.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3jkeofiwn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3sxlxjrgi.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3mtakctco.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3yzbvxxjo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ocykraee.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3qjodcusp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qeogxlpz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3uhpkkiwr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ocbjvyul.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3drhukthy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3kwueeuec.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3chuzornn.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3vttsjkfs.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3wopqqpjk.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3kyqssloz.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3crnoemtl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tfgdqvya.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3srrcluqw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3weodvfad.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3eflfsxoj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3usfxjgnn.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3agglipvu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrdhavpp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3htyycolr.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3vhpxfkvf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ioilyxmk.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3oqokebsz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3lohzxlxk.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3tqgrajwa.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3fcgwgaju.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3uhvhzxmh.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3kholnzjd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3eluccgdq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3wopsxgxl.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3gajdxpnm.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qvqvxowb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3nigbnthn.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jigfnkhj.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3flhclrqk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wpxzlxce.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3uwzffgej.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3uduwrtdn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3lfygigcy.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ojejuuxj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mtnkbjau.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3gzdbazsw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3lwdbweul.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3olenfnog.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3idimqzdz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3mukrlsqi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3oukhblpv.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3chcqowey.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3nbijhwty.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3refqwfxa.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3xasewhxr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3savwrccj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ywqhcvyp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3gykibupm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3erfwnbmo.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3tvpnzhcq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3vhjpkcrw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3vpuorvbw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ucsfjffk.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3iezrujhd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3jcufagsx.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3wsvygrrv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3qewqqjbf.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3vjsyxdiz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3xnefmhei.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3wctinxqa.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3zsplahhn.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3bixaxvwm.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3tkuftjar.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xsalgdfu.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3oyhwovnw.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3jkdusmuk.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3dxjzpskf.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ckqzhqvz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3aotpnvqn.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3zgrnrgvw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3adcllypm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3inswklny.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3gnztatxc.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3mdftstdf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3nmngpfly.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3bbtypvsb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3reieuhkp.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3nyskppkj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3gekbjbzp.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3tvmsfbri.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3ankxmmiy.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3dtzlwpik.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fezbrfrz.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3xvdndmih.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ioshuyzo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3sogxpjkt.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3unjbwgkx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3oormvcir.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3klcxkngl.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ykosgslx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3uetelnny.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3esxbrgzn.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ubvityvk.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3yuicwrzq.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ygyrqdtj.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3avjvpjul.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wwtfbprk.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ybhwagwd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ugczoddj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3kaiybrpf.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ieqktskq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3rxhehqbo.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3bdbvrgfz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hxvyqnvz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3hadtajqo.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3bswqjvnq.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3iqbzgyow.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3wfkqgxyt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3brkvaioy.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3wfryedjh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zenpjfvy.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3krukfevs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3bnkcbhhc.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3qzfoynfv.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3nwidnsgw.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3cmmtgxss.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3rtblkwcf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3kzohoalt.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3icidzgul.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3uxvtahtv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3uudwqaly.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3eepljrmt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3sffovrvp.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3hvzvfgyi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xbqjrekw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3oygyomjt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hfhtzuqd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ndkuryzm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3yddudvvc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jgopiuct.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3brqzdttj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3fgnevbci.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3listvraj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3cwftqfle.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3gzngyrfd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3afmytnaf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3zwuootsy.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3cnlmfebs.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3cdcbpezd.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3dehxndjb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cuxilahr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3hytdyhxz.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nabqvrew.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3xofwbxce.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3codfsevx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zmkpnbqw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bfxactxx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3vygqqbpp.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqpietbq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hdsstmsa.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3lzzuxhao.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3fudgeqvz.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3opzufbec.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3wocsyzyq.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3wgsqmedm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3inbockix.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3kgfkbqik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iyqjzawy.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3yehcyeht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vveuyvgr.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3jerqxayo.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3glpdospg.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3qppcuqbj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ceuzrnxq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wifkrgxg.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3hltouina.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ncjouejl.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3gezyuayh.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3tvwquotq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3uevamgyt.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3yvkczdlo.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3btfabajf.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ozqduuqb.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3sangndrf.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ijvyyfnk.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3zhxvyjih.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3budrgxum.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3tiiupzcj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3feqecuce.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3fluixggc.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3msqryawi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ffnxpfsu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3homxvxrj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nyybzmfl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3rprsgmbm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ctiapkkf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3pwxmvszm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vyhlhkry.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3eailgect.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vzvsbksm.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zpecmqod.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ibwwjwod.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ntcztndk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3luhmrnxm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3praiiquj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3lapxfkdn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wtjgwjwg.html


<!-- 参考信息 -->