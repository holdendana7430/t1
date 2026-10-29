代发 wailian999

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/grayifkyz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gwacflqdn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gkibmnpmy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gvjnfyqqx.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gbsmtyjic.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gllepgqod.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gvqwmnbuw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gckkhejxf.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/gnqqrwvty.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gwcduxtnz.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gifyhqinw.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gulllgvpb.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gyalkvdoe.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/grjkvturx.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/grdhsebba.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gblrvhcjy.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gvvuuukgi.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/glxflkceg.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gdoojtncn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gktedxbdi.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/ghhhszfyq.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/glrerbcwd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gdwxkcetz.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gdvtnqweb.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gbtfscial.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gzqmsklhi.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/ggayuoeay.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gwowoczpw.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/geurrtgjj.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/grbkhaxtr.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gcxgaxbhw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/glqhlusjg.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gvxanctcx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gohoijzxe.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gbtvuydke.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gsyzeqvjp.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gktjqmkps.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gzitkkcjy.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gheticzmj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gcyowisjg.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gmjzhpxqh.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gobwbrjsq.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gehaorzhk.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gqeezxhqo.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gylexvjju.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/ginbcqqgq.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gnefvykeg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gmasufyvo.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gonrwatjd.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gxhwgyihz.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gsagzyarm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gylgwclov.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gxcbrkcwt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/guwcxkorn.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gxriwyclu.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gmigulkts.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/guaelrxxh.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/gfslmuuzp.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gcjxdwmyf.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gaimpcfyq.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gbekcozse.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gfkqgueaj.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/glguyomll.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/ghyuizdwb.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/glsmhkjcz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gtpkuwugu.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gxezmluan.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gboppbflh.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gvekpztcp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gqmqnxikz.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gjiveqmed.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gxrweptqb.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gjwaboaez.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gjyrkovyl.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gnlrtlxud.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/geajuetei.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gqvkiubfo.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gaqbmclpj.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gjfjmrzpx.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gdkxpqdjz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/glokqkaqv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/glllrcfaf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gnuqzoniq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gvytnhkpi.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gszylqlix.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gufdpolun.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gfhncfpkm.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gkpadglop.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gycfgosah.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gxjvrfzzq.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gcskeskfw.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gtfhvxqrt.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/gjzjdnxnv.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gnqfyeryy.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gdqisvyxr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkknktkxh.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gfcnwjqzv.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gggffqcxf.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gmksgpxsx.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvruhrirr.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gfxxjppxo.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gsuonjpyq.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gkwbulhdh.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gmshgvuaq.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gixgsmhvx.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/gfzwxeffp.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gzfyixsuy.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gvbditwlc.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gpeeiaejh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gvmlihbcw.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gpjegtjbo.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/giubzhucv.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gubmmvejg.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/gthkdpswo.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gfdbcxwst.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gidohtkbe.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gnymqwzym.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gypnqufjz.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/ggqgryfrc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gmqpqcgyd.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gpjgrvord.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/ghxwgxuah.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gytxfwlni.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gnbnwgnxs.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gvbzoavhe.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/goflqskvn.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gswiatelj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gdfygtpje.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gldzetcdn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gofcornky.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gcwtwwpoe.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gjpuhhqkq.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gzmnsrifz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/ggabzngvp.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gzqkrbsvh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gwiqezdle.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gqfpxkupe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/gaqxohklz.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gyvtxplin.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/guxswdgcb.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gdbltnfww.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gvmlhbbgc.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gafiuhazm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/gnljyoyoe.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gfltbypxx.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gijbcvauu.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gactrnwbe.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/ghsdtptrv.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/gdlqnvzyp.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gauydhlhr.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gyamfklbv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/ghhjoxycy.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gzpzqfkke.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gdnajuwyn.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/glrjktxjc.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gthtccatd.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gmwpegqgc.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/ggukwxutv.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gcgrodcyz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gcufatxjc.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gjmbphdbu.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gxxppkxqx.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gqvwuksir.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/ghneqjjak.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gdslidmcm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gqhlqjuvn.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gdkgjwgqi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gkykuleot.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gaoozmhur.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/grbauuhft.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gossxvskn.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/glhhnwzyd.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gdmskyjlw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gekcgxpeo.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gyeiarryu.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gdbcwfqfv.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/glqpcpyaw.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gbfnkxucu.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gkjerenmh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gocpskmal.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gvowhyyjl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gytffjnln.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gfumbwstc.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gqmisezzp.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gqqwcpqok.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/giuolwxks.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/goqesmogr.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/grijglgjh.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/glrbfvvse.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gcgjylsad.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gkyxjnrvg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/ginngrfox.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gtixtnwvd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gnjphnoym.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gavzmhezh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/garizlplz.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gqcjtrfso.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gpklibbst.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gtgyzebcz.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/ggjdhsgec.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/goejhdsug.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/gbdnoafow.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gxtndqjjk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gjxvltium.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gevihqizz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/gbbrcjcmh.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/grfkstmic.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gebjcsiga.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gdkwmdhfz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gzxcamjlx.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gcunmvabs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gdpmhtjzp.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/ggedqdnnd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gieffyemw.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gndaytbdh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gpmbihppd.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gllgvvfmf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gcxjhwdil.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gvqsgbbbr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gotsrfoyw.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/ggoroneqi.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gwrxujuyt.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gsjfccwqn.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gfeuuacha.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gmxxrdxik.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/guadtcoyi.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gyffpqzyr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gctfjlyqp.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gqtwfwenp.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gqreipqtf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/glxeczybv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gplchfvgl.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gqluzlulp.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gopbpsruq.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/gtaxmbjjs.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gdxudfipd.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gxjzsqrfl.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/ghopetqed.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/guckzrdsn.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gwwgtyvdy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwuyimuzi.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gjfhxtifq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtoyjdqml.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gxyylegyz.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gkzwzzjph.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gzuogwwur.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gxytqykzc.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/ghbduylhn.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gmffovydd.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/ghwpijbga.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gmgfkidab.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gmykxuujs.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gjbtubqoz.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gvsxkyugo.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gjhgsbols.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gpbzwecnj.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gxxnruqkb.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/gwjsfbfkz.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gdxljfchq.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gnjumjyhx.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/gqkqxwovx.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gjosqaxjd.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gzoliyrri.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/ggrzqkupl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/ghporcgwh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gfdkeefnw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gfpmtnmql.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gydhwggzc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/galzsdmeu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gudlqaknx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gcgimtvmw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gtndrfixn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gthkmbbyo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/ghdjlezvi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/ghspoaxmv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gkyajoifc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gnqzeuetv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gqdcxahpf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gwprkorcj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gujqudwsy.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/gezsepxbz.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/grukurrux.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/gbcxywger.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/getshdcbl.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/goxheescx.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gmccdvwpe.sHtML

合计                                  2106 条
来源：http://m.share.hesvh.cn/Article/details/gdyprxgmn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/glrkwfczd.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gzppelzau.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gnfoykmar.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.zdbjq.cn/Article/details/gpeieodwi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gwexsrotc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gdebzkkpn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/gcvuknaed.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/gfqrukkla.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gxkapibph.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmvdzewqz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/gacsudjgx.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gejgxnfnd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkdjuhjwp.sHtML


<!-- 参考信息 -->