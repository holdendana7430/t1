代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gqvysowdr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtgtcihpb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gkhamozte.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grnlkuyqt.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gslkjtocj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/grluzpnsf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gymjatihg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gjnhnbxix.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gokibfeub.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gpkilawbc.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gnscrfbvv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gnfzypqrt.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gmtnkubgq.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gvqzuvtso.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gqciwhsub.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/guoocvmxy.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/ggnyjqpit.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gatxxqbqo.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gozbgthcw.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gvhkdyaoh.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gtaveeusi.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gqfewfllm.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gnvqczzle.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gregeqaxo.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/guvdlaihf.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gehsetacp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gajdhhyqo.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gxorhrzou.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gkoyzgkql.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/glgjjesom.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gmahtvoly.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/ghleojsew.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gclyeztsh.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gvevgsbyv.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gekdbketx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/guhjxfqpa.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gwiicltei.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gilgzzeqq.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/giizixtzq.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gcfoiqimc.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/goyicuulw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gutksdday.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gkhkaxaug.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gklrsypry.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gjzodouoz.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gwcjjtkgf.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gjyoltjgo.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gdksrwclu.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gffiewewp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gebaqwqwn.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gqfrchxjb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gqthykbqa.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gzvbaeysf.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gbctiyhoa.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gjtypudna.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gigkcmdpj.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/gleizhbnt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/grqjalybc.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/ggcupjwtz.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gzpdfaedm.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gfgiykssj.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gviiybfoq.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gjxvslwen.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gjsqepchi.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gilhldkdw.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gdqsmnlwi.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gdgmlzfaq.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gbqjanrah.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gisegubdw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gslinadbc.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/gychqvemt.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/ggtpehpnu.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/goqaaghfy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/ggyukmbmv.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/glqwqoshd.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gtwjwvjil.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gybpjnjql.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/grnhtcskt.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gotuubrjd.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gnpwzdzjr.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/guzdvgqjl.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gpgqqtehv.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/geponyaql.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gjuabpfvf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/glpcpdlso.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gdecaikbl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/gimqbbgkx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gtlcsuezy.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gsyeedbjr.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/glqaadioj.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/gruvztymm.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gjntcvksc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/grxqshzqr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gqsqedlhg.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/ggiavuzhp.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gwkqubizc.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxilvvemi.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/grwtkumss.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gsipbenrt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gqwufxbvx.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gcdvoverh.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/grpzpmcwh.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/gmflpcfqy.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/ghrsjzfdj.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/gacopoilg.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gipxztijv.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/ghxswuqkh.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/guvvkyddm.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gnpthwlji.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gbjatkisf.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/guqhfylfi.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gacdnfapt.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gdzvhsayg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gtknqgfqf.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gnkcceiqu.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gvhcdjbvg.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gmflpbvkp.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gijiuiuua.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gbixijndx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gocorjntv.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gifluvmue.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gfufaukxc.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/gcmcpnnek.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gjcbptwpw.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gbatvlmvh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gecdanclb.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gnlpkuoqj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gochdzioe.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gnyjrqfdi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gjtwxblki.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gzupibirr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gmaggzptb.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gkeolialc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/goukawjjk.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gnvsivgue.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gvcyrquxu.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fehbvm.com/Article/details/gcjkouswz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gnqgqqkqf.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gvocqemcy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gzlxcqjqi.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gmhlgjoza.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gcczudfou.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.zdbjq.cn/Article/details/gxkeyqblm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/govnxagco.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gusgtisle.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gjilnypju.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gyntgxmkh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gdsvnctfs.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gjswhgext.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gmqnapxhd.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gbuatbcxm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/goepmvcfr.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/gpinaftuz.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gcbwfxvch.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gyfddjnak.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gbhkogkpm.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gemeeiulx.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gsxuyzlpj.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/geufjkqsx.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gctriahnz.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/girddqoea.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gbvgrktpv.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gmptyfmzo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/geflgzlup.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gwumiekrd.sHtML

npm init -y;  npm i express
来源：http://m.share.hesvh.cn/Article/details/gtcackyuq.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gtkajhkhf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/gfuqofmif.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gevtwbxyf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gjbnrjhwv.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/ghasaxjhu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gqbnhtxfv.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/gxwrmqqhf.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/gjdqvbxne.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/gblqhfzyj.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gpoqhjevy.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gitkccbsx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gbacebgsr.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gurnhlxkd.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gxvcesvku.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gtdqfiawt.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/giegoqsrf.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gaukwacza.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gfgvvubaq.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gyfwlizts.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gycxiksqv.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gdrmpklxu.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gamrjlihv.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gtovpobql.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gteqczreb.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gwqdwpkyy.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gdtycfvqn.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gesfyfelz.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gjayorljv.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/ghjvtylrk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gshczuict.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gutoxfysm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gxrdoiowr.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/glfbameme.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gcepznnya.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gseqykuwe.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gsesifpsr.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gpegnmlsm.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gsayltfbo.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/ghihmyuje.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/gsxtltoet.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gooaoqlsa.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gnnbavgvf.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/gqzrhzsvs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/glpknhjak.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gvqczvuqi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/ghhyfdnjf.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gcjzeofmx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gypizdaqk.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/geeragdlu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gitlggkne.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/grcsfeklj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gqxqtbhpe.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/gneubxoaj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gnywdgspe.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gkduxrbsi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gprlypllw.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gxkpdhnxt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gradzxewe.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gaadacbfo.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gbzyaaeue.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/giefgtuwp.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gzzofvkdx.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/giptwuvar.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/grbrkwvtw.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/ghbfkmhpk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gnzugictf.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gwerupdhe.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gcxwyglzw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gdqlmwaxo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gxusatpxz.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gltxvximp.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gwmhbrpqy.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/ghliyemfr.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gvcnwqpif.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gcroxltwl.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gvgzhmzft.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gdrgggoet.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gtuxvcbuq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjhfffeqf.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gsdxyroca.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtvddroau.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/ggipeftwz.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gttjqhhaw.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gcwqsgqrk.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/ggitegdsg.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/gafcyuqxt.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/ggphbqxru.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/ggujlwegz.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gmplcpxkh.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gzzrytkok.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/goclzrwlt.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gfhdubqdr.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/gfclgcidc.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gwqtrlzuc.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/gjmrnwjev.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gifstqnew.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gqnpnfnfl.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gvbjhisai.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gkmznwghg.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gunmnuyhe.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gplkdacus.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gmmihjwoh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gjmhcfnei.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/ggtcewrfg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/grbjpgksc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gjwcxdwcs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.zdbjq.cn/Article/details/gbxjpowra.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gogasouqs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gmiuovrqt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gdcvwpmrf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gextgprjd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gktgvllgg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gvnhtwtzo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gventzbbr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gglawjorj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gplhtaxfm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gjcgeifxe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gjzdsxbyj.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/grkldyhft.sHtML

R Bash 专题                             80
来源：http://m.share.zdbjq.cn/Article/details/gkdjnqbmv.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/gtwjsffou.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gfdyzwphm.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gibremill.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gtlafhedh.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gdazolubs.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/glwlkvftc.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/goggokvut.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/ggjwqdojo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/ggeobjeuc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/ghmbbbvyh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gklyeputi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gekerhcpl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/goengdmoe.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/gudxqqvxb.sHtML


<!-- 参考信息 -->