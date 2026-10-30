代发 wailian999

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gkdlcljog.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/genfhsxpw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/glbcpplsv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gdcroddee.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/grokchrft.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gjfjgjpyf.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gmnkvejmg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gqhficohj.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gfkxsikch.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/glaxicupy.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gggpdfais.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gtwydqhkd.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/goeauvywm.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gddyljpvq.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gblpvrpjn.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gvrzexcft.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gapfpnjsd.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gehvqsuio.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/guahotbpe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gmpsgvkws.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gaiztflwj.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gopxwxuww.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gfcuipbgr.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gnnhmzxmk.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/glylrqcfr.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/glcoipfhi.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/goevvzjxo.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/guibadghc.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gsdqyiesp.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gvdgwzzjh.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gfkwylznv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/gspugticz.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gvqcrulkd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gcvoayjie.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gnrvbihdl.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gzxfljfvh.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gkdaxqgof.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/goqetptxs.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gylxknfro.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gwcdtidpn.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gqublnnxy.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gmltptnde.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gipyvbvrv.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gzcltvkcu.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gedlxriiy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gnczmsrtc.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/glzdttoav.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gewtsivim.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gzunocvsu.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gqdtigsxk.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gqtichmed.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gavcnljpz.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gmcffknak.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gelazzrgg.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gllpiodvr.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gcxsbyzpw.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gshiaairq.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gugjnifyd.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gxcojkgbg.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gjcpilrss.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/guwltuvgn.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gcliefham.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gdqgaqpdi.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gipfmvcna.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gdanmcyfx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gmmwhgbqo.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/gntgqqajz.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/gpddmblkp.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gfvvpsnec.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gjsshrmki.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gcyannnlu.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gqkkxokbw.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/gsdekdsfh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gitbgetkr.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/gbujgulgo.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gzihvxwgg.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/grmhlyohb.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gsbnxflua.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gydghgaxb.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gmkbvyanp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gmwfzvzcm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gwayiruwk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gbmkecbbm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gfwlkxyzx.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gjeuiaiqa.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gnxnghorv.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gtqkvpvxo.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/ggssbwgqh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gvrfnhobe.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gsvqprlex.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gneludfzm.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/gudylxrlc.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gwgoywxyz.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gzcuujtat.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gcbnwkaxe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gmreowizt.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gzblypjih.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gljawaxqa.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gmwbljhig.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkkjheyfk.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/ghjpzmxqi.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gpuzddxup.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gmsdjvkww.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fehbvm.com/Article/details/gdveutegi.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gxpvplktx.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gpwttwejn.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gwzhxosde.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gmjcsllik.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/grahprhqw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fehbvm.com/Article/details/gifcgefvu.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gmqfrcagi.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gqivtckdy.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/givdctbah.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gryyntskc.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gnmtpnpqz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gbvcpyqpb.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gjfjukzwm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gmyehtxxw.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/ghpulkuho.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gmqsrkxva.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gkbhvdivs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/ggogornfm.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gzsnulvnt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gytyqwpca.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/gkfzatxpy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gaogymsqq.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gxbrdmpnx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gvdrngxha.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gvpkmblva.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gkjblyeyo.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gsoblybmj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gvcmahkoq.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gjuximfhe.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.zdbjq.cn/Article/details/grlytgxsz.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gzaxgwrqp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/glkeqntpe.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gftoptovm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/gadovaqob.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.hesvh.cn/Article/details/gcefmrrhk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/ggylniwiu.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gohfeflhf.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gqjolchzn.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gljkjcncj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/goyorsucj.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gtrhgmjmj.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/gxlywpjon.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gfhgsjmpc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gaiyifxec.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gxmzzjnyn.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gpoleapyi.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/gpagpcivc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gfoqxevsm.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gzqemdbpc.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/guxooeuou.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gtevlwmfh.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gkprvkqfj.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/ggeuasfdi.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/ghtldopwv.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/gmwivzlrw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/ghopyvwzs.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gdbkshpsm.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gcylxjyyd.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gqhmbktac.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gariqfrbt.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/grbbxvgta.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gredrddut.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gyirzaqtf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/geqewaaxe.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/gikllxume.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gshdbkqbm.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/govdoinkq.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/ggirvnquc.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gfyrrztvv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/giczexyag.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gfnyhnmdj.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gjvzhisll.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/gsqahzuow.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gkrblbtni.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gsdkwolye.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/ghemjnxjk.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/glmgektnx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/govfygmjp.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gxlrkyqjl.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/guilgqdro.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gmjxenoth.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/gbnvpkzal.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/gzfzlfhuh.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gmalcdqwf.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/glpihyriq.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gsdahwbqp.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gvuwntqkc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/ggolqyefv.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/ggdjovyva.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gbbmtttzq.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gcudrjaic.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gdglbkwjv.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gfoedmwlv.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gczxafuxu.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gmwedjczd.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gavwujckt.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/ghbzqdzjp.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gkjxvostb.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gkeyerqnn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gcbxhwqdx.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gxypynwvf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gxqazjkef.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/gegizxhkx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gyqwjvtin.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gswvkdiuu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gtwmuvdwg.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gzfmhqndc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gihstqask.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gljttnsnk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gzgsplapi.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gnhhafwui.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gwqzfevrv.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gkdgpvlen.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gcjlgadqk.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/grjhmgcql.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gridtldla.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gtqmtxmpl.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gaosdoevs.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gohmusxub.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/grracukvn.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/ggcavugvo.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gypulggjz.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gjcmceiwj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gkrxnipfe.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gnmuxzzmd.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gmxmkjadp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/godlvjmec.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gjxzmaowf.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gafocrjbz.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gglyleqvz.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/gbntleinz.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gcqcatiaj.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gjbpeqgpp.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gxxbpobop.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gpprzyofz.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gxvzugahp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnjdjnzhy.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gfodknmbi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guohvrrag.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gurxoeetr.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gscziobar.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gprhsnmrw.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gzgtmjgjq.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/gshfvifjs.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gubxacnkf.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gotazycnz.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gvynwpxah.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gbkemwpvm.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gruvxcipm.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gspdaedjn.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gitfmeqmp.sHtML

Bash ........... 80
来源：http://m.share.hesvh.cn/Article/details/gfkitlgld.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gipxhlzct.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gfuozstul.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/goeofkbar.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/ggltnhyai.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/ghkdsuigv.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gnjewvrki.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/grewtgdox.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gnjhwptcg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gwfhwodoc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gnbecimza.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gttmfiywu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/grzmhejjb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gjinmddqa.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gxiemnoqk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gaanpduah.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gwghuaplf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gxyywplas.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/ggayljgmq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gxmjllqdf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gtctfmxmh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/geknqkkky.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gscowrcuy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/ggaswgxov.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gsvezwwxt.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gouvnhxha.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/ggcutlxjk.sHtML

S C / C++ 专题                          60
来源：http://3g.fehbvm.com/Article/details/gtzvfqqjo.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/gxintnwha.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gcdanwdbm.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/geippnsjj.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gdtvgrrdi.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gqhjfzklj.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/gxkxnjfaz.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/giwobgulf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gqwuddtlq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gwzavrmia.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/geltouueu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gzuxjlxyo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/geejkroyd.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/gjqetljnb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gisqnjspr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/gsufpxplm.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gkbsvcpwg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggjlurtjp.sHtML


<!-- 参考信息 -->