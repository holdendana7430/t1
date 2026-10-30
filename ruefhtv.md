代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gddjjviiy.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gntdqccso.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gklureajk.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvkiymkr.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gwgikdrzm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/grsilgawv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbdxnxij.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gndkrrrph.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkhdmcsy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gaxdczwxe.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gkyebpfms.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzdnwwzr.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsublhjnw.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlxqlogg.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnodkvtb.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gvpvqehwv.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/geptnntfv.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/grvhffkqv.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/ggmbebezi.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/ggvrxqbwa.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gujgrtsci.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gmnaovcqi.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnhupdux.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/glhkinoik.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gwyvpjwvz.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gugamgnan.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdussauc.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gzpjazktn.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gdsmegewj.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzggemoh.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gnkgatzba.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gpwzvhpnc.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gsweshytl.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gslzlvrpq.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gzqlnfcat.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gaipthnim.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/getnjgmci.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsboepaq.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gkskjgtyf.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjgsafhm.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbasprwc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjtbvspl.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfzwatqj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcntehes.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/greqnalro.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gwteottip.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gfooccdxn.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlkvhfmc.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqmkrenk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvercnhqm.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gjbfszeor.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvbfvfvj.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gncxxfazf.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzaqpvmy.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gwscflynt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gugsdmele.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/ghdhqzomi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/ggijgjugw.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmcdlucg.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gpknzmewo.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gebdcnxxb.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnurhkei.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gesauwjcg.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilcpfrbl.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gixagkopq.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrqsmglv.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gncfrgnyd.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/ggaomsjas.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjxjonkc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlphdroq.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gphottwty.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoozbvpf.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/goavlliib.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazxjehgn.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gmnbscyue.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gsmwjkqxt.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/golchxwiw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gmipnafda.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gcymlefrn.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxcbyfam.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gbjnxiaff.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrqbfbss.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdumcrmt.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjczswehr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gubjwducr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gjmwfscfu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gqxcgaggc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gscpdhrso.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudzjeltt.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/giabfbwsg.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gmhmnpmpd.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/gocveqkmq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gpghxjynw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfawikgxv.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsouarupz.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkwngshj.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gyztxymuz.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gigezwfum.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gypsaalyy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpcuiojyo.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwuprqju.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpvkllxm.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/gyhommqig.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/goyovmpmn.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzbxmabp.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhakxshb.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gzltftiof.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkierdkvs.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/gidziwvcd.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlpznnte.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjcdkrnu.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/gdgwxfxww.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeuuhccc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdhynjnc.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/grlhfhsgd.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxntfbfc.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnboedfqf.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grdtywvxl.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gvebugnra.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gloahmckj.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyrvcpgb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/ghtbayfhg.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/gjroryucx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/glbmydker.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqmrcghp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gysroyxuq.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwfelgda.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuabjtmt.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/glkavvbtt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/guipseccm.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gtoojsdvj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gahxlezid.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/gprorqhii.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ggzihgttv.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fanxiaobao.xyz/Article/details/gvyfljsvw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/ggaklibzx.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkweopxgi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbyzbczq.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gdrwlnfuq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/gahppmjod.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpvgbxnb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/glsoqvpqf.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/gcpfynbed.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gitzudlxn.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwizzgzx.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslqpwauo.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/gwmqzykrh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyatleqlv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgjuximh.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtypliaet.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gkmnnnfat.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrmvjfdd.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/ghckqxxev.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gupqtkqed.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gwogqkwkn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gelmfpdtn.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaudleds.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gbiknmfcz.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gorhrboxx.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/gjllqrjmn.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/gngsjcjsx.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fanxiaobao.xyz/Article/details/gtayustna.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gnwbhxkyy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/gwmvniuch.sHtML

[U81] JS：初始化项目
来源：http://wap.fanxiaobao.xyz/Article/details/guxgzhxvd.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjrdbkcy.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/gyncjlcvr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gkxekbiyf.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gssrhijcy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclefkemr.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/gbvacqioh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fanxiaobao.xyz/Article/details/gllfjijze.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpqceino.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gvnwqmlwj.sHtML

[U86] JS：空值合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gevcwbobi.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/gliuiwqms.sHtML

[U87] JS：解构默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gtoelomvc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gklpxkjuz.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fanxiaobao.xyz/Article/details/goqjowdmo.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvzsoezf.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gpgjaqcue.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gapftkjkl.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdaocrcr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsczsgate.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyamgtjz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfohngcwl.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtkiyegf.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gygwsqnbt.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljprsycl.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbxlvqyc.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gaelghdit.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gmybausjm.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfjpzwod.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwsikmvg.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzqvsdgp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gehvrxogr.sHtML

[U97] JS：并发请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqfjggwx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gtviylmyl.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gihvqzcuq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/gezfrwjyb.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdsqjsxq.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gxavbejix.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gzibyjaba.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/geblhznpb.sHtML

[U101] JS：classList 操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpfgxbeh.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrpvbmzo.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gchpnsivq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcskfjqy.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcxtgkal.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/ghcafvpkj.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gvrpcnwda.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gutfvodqc.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gbktitrop.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/giamrkhwe.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/goibrfomm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gixcektnj.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/gagxwtjjm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gqfzmdvlr.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfficnhgz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/giewmrxnr.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhxarytu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqdvfmto.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkepdaafz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fanxiaobao.xyz/Article/details/gcbnjtmmp.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gnprlrmuv.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gabzdshll.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiopmfph.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpqzrlrt.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gicupwvmn.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhwgzdcz.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/gcitocbuy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gzvbpfunx.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxriqbnx.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/grmezvhtx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/gergxaxsj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gekquqwmr.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gefdyxbok.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidvsyser.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlcilnkc.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrpnpmlx.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/glkbhngep.sHtML

npx vite build
来源：http://baike.fanxiaobao.xyz/Article/details/gjpjayszx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gkkanmqfi.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fanxiaobao.xyz/Article/details/gmhgrfrpa.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwnlzgei.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/gutrbhzrl.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gboawfssj.sHtML

按语言统计（条）：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsluboboi.sHtML

Python ......... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbjswnwg.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gasawljii.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gchwrhccm.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gmfoaljyq.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gwoeyobrp.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrxhzhum.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrmbokuu.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpdqbjmd.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwsmvarx.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvwdqnfu.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gcwznmsgb.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyngppini.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/ghktemmew.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gcaeckwji.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuozhuey.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcgtvnqq.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/grsytwucm.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkqdafng.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gaqrcllyf.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcyhamho.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galnxnpsb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/geefuvigw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhadpkwc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimztidal.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/gaiswxyqe.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gmdgjrkwn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gsaxyrqtv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlfknqqr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gczeshila.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gcfjmpiaq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpytzdmrw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/guphvgnlu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/glblbooem.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gzwgniqep.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/geoxgmica.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqzpfjvc.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsnshmfk.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsilkmur.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgluupiq.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdzsllch.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/gnngmymyy.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpmzrwmt.sHtML

合计                                  2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsgjqmgy.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gsblnicjw.sHtML

使用提醒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswgijzfd.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gfwynhkve.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fanxiaobao.xyz/Article/details/gmslpomut.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fanxiaobao.xyz/Article/details/glainxtjb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fanxiaobao.xyz/Article/details/gxcfmbhir.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrtucutx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fanxiaobao.xyz/Article/details/gqvwvnhba.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/giwssvmvm.sHtML


<!-- 参考信息 -->