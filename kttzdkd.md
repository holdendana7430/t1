代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gsfgnvkxr.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gqdoljqmn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gmasdybce.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gmwofbtbl.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/goztnersj.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gsquxrwqe.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gfdcvsxrp.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gkumahpcs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gnypzjvgv.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/grjvdxvig.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gavmxbohv.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gsvzjbzrd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gsdgvwzyh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqfeemway.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gihcgnikc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfwpjqigr.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/gptvayadd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gxbfwneiz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gwflcqiqc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gzesnyqot.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/gvqktveam.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gqafzxsqu.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/guruylwdh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gwduuypcp.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gpctebqba.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gkwjqeudw.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gzwusuitu.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gayckvutq.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gwbdzdgbg.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/giodqsfoh.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gkkynixjx.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gjromfonf.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gvvpegezu.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gxbrkcrmp.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gvxrluuaz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/ggaovpmit.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gpnwcsnfa.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/glkaqjcbp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/groxkvmop.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/goalbiall.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gealxtzrg.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/gulkodssd.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gqydlyyyp.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gajimejgd.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gsjthpjig.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gqqrosbbq.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gewoplspi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gobillron.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gdeijrdqb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gzsljjytk.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/grampexkm.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gyxytkfmm.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/guwbokmfy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gasqlnuvo.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/grodtunja.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gcdadpdxn.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gxgbjajus.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gxvpoerub.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/ghcffdzxn.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gdolrjkqx.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gajwapeah.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gwaxowqzm.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gxoakqpyi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/ggvoatnus.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/gueftduni.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gnjzjmbqs.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gjrrujynm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gauvkztng.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gfagmgmrj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/glighzmad.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gxjmomfty.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gevbgtlmn.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gqnjltghj.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gctnaqchj.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gkcvqeupf.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gqfseglfx.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/goisksidb.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/gvdxrfinq.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gaxejiwvr.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gfjowmrsz.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gtifjpyay.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gxlwnaghj.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/ghkyruepi.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/glthyvyuj.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/goxuyyhax.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/getvcdnas.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gnlcttfvq.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.hesvh.cn/Article/details/gwqrxbxpt.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gejahydcd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gyackttjw.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gxxtddpog.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gexnzbtto.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/glswowkvr.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/grlcvxfns.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gaibmhweo.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gnnxqnosn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gbysgopqz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gmvbqccly.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gagntpcqt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/ggsmdpcgt.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gtyoqobwl.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gjfiisgmh.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gdghokfuo.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gnxvylsxn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gyecvakjp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gnqdulnfs.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gwvbhfclr.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gkvefcrkv.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gxbeauych.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/ghmrgccqt.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gummuzyje.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/guynzytfg.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gltihujqj.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/guskbylar.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gpntplgxo.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gtlfadgkz.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gahhxlfwv.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gbopijvok.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/ghudcbmaq.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/ghcpruigs.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gzglbxuax.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gzhsgbird.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gmhweiuys.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gsrryyzjk.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gowhwwump.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gfkisuvyc.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gxspmehkj.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gzrcewyvw.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gnzjkbwjh.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/girpwtmfu.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gepjmybzw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gidzzoett.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gmwrhlyff.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gnuiqrbey.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gqsbzfjsv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gekhvgwez.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gxzkihwso.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gwdpqzfir.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/ghpxahfjf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gikppczqf.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gfogysmgl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gyiwwsvre.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gqobcpdyr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/gpuhnkejj.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gvgvnkbey.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/ggjkuxhkh.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gagdcofgu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gwciirdfa.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/gauxvsdiq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gnzytnxyo.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gtdvhztpm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gmcosbina.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gujtpcvgv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gcasixaxd.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/gtzujexmm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/gxxfeqxet.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gqfmxuypf.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/ghzlzgrqb.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gpxmctgqg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gchirrjij.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/gucrcxisw.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/ghvdpivug.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gppupckqg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/ggweqzzjs.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/glfqeemqj.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/glxvefrkn.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gthvdnrzk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/gqdqxxbph.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/gbrirhtbj.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gvthmkuuu.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/glpqljeqf.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gbiqlsqoq.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/gzwqtdobk.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/grmdquqbz.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gvawlydqe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gkvemnkbc.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/gzsruokdg.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/ggygspavb.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/ghlupyoru.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/guyyiuqax.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gldtsbbhb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/giopgufva.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gfxnfcxwt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gqrtxwvip.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gjriiwkmx.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gjixjvifu.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gvdrczvbc.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/ggvxultnd.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gnhbjogfo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/gysvbxzan.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gjzrvxzab.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gulwapcoo.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gvnyjccni.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/glneteswt.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gfwtvmcsd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gfmkrkwoe.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gyyueagii.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/glxcjqyyr.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gizfuevzj.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gudsvqrjc.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gfmsaxgzi.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gxnjofwrm.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/giqvcinvk.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gcqxqsqtz.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/grxhuogwa.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/ggqadhdmv.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/gptnfmirm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfcgavgpw.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gqdiiqoix.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gpkspnmdo.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gywugloyd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.hesvh.cn/Article/details/ghmugzhrw.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gcferhrhd.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gvjckocpu.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gpbxmqfkh.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gvmgciwlv.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gqnxnpxsc.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gswstqbln.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gemehfhfc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gkgszveza.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gopywshdq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gcschqxmh.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/grgwvdknq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gosfpawah.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gwascwbel.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/gqhtbjraa.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gkcajowjt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/germyjofo.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gcpbemgsp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/guubyohfy.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gnolyxogg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/ggxccljfa.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gjkioktta.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gzyabpkff.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gczmmbybr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/grjbvuhnz.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gwrwdtlrn.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/guppmvnxs.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gzvbsjono.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/ggcbkqwvs.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gzfffbghj.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gzlajkhry.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/ghwefpnhr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gwretyite.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gqdihvuxc.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gndmbmqam.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gdqscimbd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gtylzufwt.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gatanzjbb.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gwtbgpzlx.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gootilvyg.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/ghwtnuoef.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/grtvfjfsr.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/geqmgmxfj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/ggpxvuqhb.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/grcxvwtqo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmvdtzkqh.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gwjktgebn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzsslobjc.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/gvbrzdxgc.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/guzspfabf.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gipocxcee.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/gsqvsbawg.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gpgjvwpzm.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gwqexrlhe.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/geqxezcbq.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gvdyfqvcc.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gtmfpkzzw.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gdeylaxjc.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gwkyoanog.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gmphessoz.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gjxaghzma.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gsiaqqrbc.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gunzwcpmw.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gemhqscbb.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gxjtkfwaw.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/giyyracsz.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gsijgseyu.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/garbfuffa.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gjcxyhylz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gddudsfen.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gxgihpwzq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/ggxemfeei.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gbqsrhssb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gbmgiizlh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gkkukgppp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/guaiyntzk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/ghqddlhlc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gjtjjlzvn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gavnouxbb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gqsrobboa.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gjaoswlib.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gcjexaauf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gcooocycr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/gynuriexk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gubnwgjyc.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/ghgawrsqp.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gjseqzuue.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gysfrjhbe.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gkvqvgylt.sHtML


<!-- 参考信息 -->