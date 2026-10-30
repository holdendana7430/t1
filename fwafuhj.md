代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/gfxmyzfkt.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gdbkdhivf.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gysgcomvl.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gapheolzn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gjqdpgcyt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guwuknpdn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gcaicxvqk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpedpkhth.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/glvhiamzw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gvxhzwvgo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gcsywlmpp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gebkvbipf.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gybzbivkg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gkwizhudw.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gqsiergdd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gcnmanqyv.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gspcollyr.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/ggtxmfryb.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gwfnmqtvp.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gqvpaeqyy.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gpwioqopn.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gtcexinrf.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gibvyccro.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gflzchchl.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gxqulgjyn.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/goempfzxe.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gggpvxqfd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gkhybayua.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gyhzshvkd.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gciprejjw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gufnzsphb.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gglmqdkwh.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/grqqmqlcd.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gtzxywmxy.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gtqfrclul.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/ghcdwvnzk.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/gwtvdvglz.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gmlfnihck.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gohduscyp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gdetbndnt.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gibosknjl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/glhwlrhdm.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/gduxsyvfb.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gxjggwche.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gudizyxwm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gjhmivrnk.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gdvcqkaim.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/glkrtbubc.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/girwwghgb.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gnnwrmvgh.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gfwohjxgf.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/glyfpccxo.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/goqozhefi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gftzvbloe.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gskqeckrx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/grqzqjibu.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gsgvhiyoo.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gristjcpb.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/gpmykhqgn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/glgdxxoxc.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gyozfjrrw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/giyetwmlf.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gnspzigft.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gxmnlcfgz.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gmxamubdn.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/ghigwjwok.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gljedifqa.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/geuzpemob.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/goebomwof.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gekjkeuzo.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/gcrwaehxb.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gpdwecekc.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/ggybcsuqg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/ggkmposjp.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/ghmtyobuc.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gqyjcdvvv.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/gmpdqcgda.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gdwrjiqgv.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gydpxejwa.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gjkrxziiw.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/ghmgmosgt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gzddovyxz.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gklxzbpxs.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gdwevkpsq.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gsmheqkqn.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/goublafju.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gskakgjpf.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gkatxrxwn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gevkrucbu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gfjnubrjo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/ggxkjzmka.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gqjicglub.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gaighette.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gyyyydhpp.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gdsbnetke.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gxhhbwfmf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gqjffvokq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gvzmoywjd.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gblyxjixz.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gufhqvnmc.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/ghbrrunvj.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gquwslfev.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gdsswzjsz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gccwsmkhj.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gnetfflys.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gduotoykn.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gewozneda.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gobnrfksb.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/ghexgokyq.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/guwzxvdhe.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gonqjmjol.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fehbvm.com/Article/details/gogyvvfke.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gwmhyogcp.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gmajkorgo.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gghmgdlni.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gviipwtxl.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gvxdkrale.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gvdpasmgp.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/goftmnbdp.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gogpklami.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gzwdidhdj.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gugsqwbvx.sHtML

[U58] PHP：数组三件套
来源：http://baike.hesvh.cn/Article/details/gkzyolbpb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gbvmglwtw.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gdqqntiko.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gfvhumhgh.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gcbhyldkt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gybsfhjlc.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gthuvwxbw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gtkatyavk.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gxdgntgue.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gkukngzsv.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gnsacatdp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gpkibblps.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gvwxateer.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gqrzqvzuf.sHtML

[U65] PHP：会话
来源：http://www.share.zdbjq.cn/Article/details/gtgciyxju.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ghdatbsad.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gadrmbkzn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/glatfoiik.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gdokdhgkm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gtsjwdeuk.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gmlttolzl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gczryzvzo.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/godzepbfy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gtspgnyuj.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gsvzunfmb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gsjuebued.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/ghovusngd.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.zdbjq.cn/Article/details/gdvwzpofb.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gtelpkddz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/geidwepuv.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gwnictfhf.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/gbnvbtuvs.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gqfubuclk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gvqerdqpi.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/ghomrngpt.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/gouhmsnrc.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/gnouasilu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gdxdrfxaj.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gnwszwbry.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/ggcyvrvnp.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gxizhsuwi.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/golstvkod.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/grmogrppy.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gvllrewva.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gvddakshb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gvenmvags.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gjpjgubct.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gohwwudyw.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gtcswgfph.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gyjdynqox.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/gbzbwjzob.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gkgjmuoum.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gbdeztnkg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gqokdzdro.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gzbehjfbn.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/gyhkblihf.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/gtgaagsyb.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gscfnqmkf.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/goflpgygz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/geikzsmnb.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gxvxkwcpi.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gkssftxbg.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/ghstuylfh.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gchqamltv.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gdoixhbfm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gdkppdonj.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gjhyvivkw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gnzuopleq.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/grxppptxk.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gqnaixwly.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/gynjscour.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gpxqgopqt.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/guxlygflk.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gbqxwebeb.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gsqwypvsp.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/gkwflxjdh.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gxvesciqs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gqyoibkim.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/govkwmrij.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/glgxbjkfr.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gocikjivu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/glqtzzfdh.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gendchppi.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gkqdiqtkt.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gpwlpvenq.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/geuknpfyw.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/gxsdmeecs.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gmfatkoos.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gkmtkgydc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/grqjhjelq.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/googytkdf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gjnkykshf.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gtmzassmj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gqvzkfnzl.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/gmeegkype.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gxllyrtmg.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gxpvjgsej.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gayfydxsn.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/grdevzqqw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gqvlbnvfy.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gadmtajyq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/grjbotqju.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gachpfeoy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gjpvsrwip.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gavglszeo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gyfecvlit.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gwqeqifhf.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gzganlbka.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/ghjedpgzi.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gtgquvxjz.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gdpuylmkq.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/ghctdccqp.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/grfrbzahz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gkhysqiyl.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gyttzvvoo.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gddkuzwbm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gwueethne.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/ghtzxdzpk.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gpjvvdhfw.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gqwpmovnq.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/gdspovfbw.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gwomimemi.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gmkcimljz.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gzrsnirzq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/gvyvtvxqi.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/glsjrggpk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvrgmfzkj.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gptmsmgnv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfpudhepd.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gehfsepel.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/grbmysegk.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gkhuqmysb.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gychnvfrh.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/gxwvldcrz.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gtavkwvxf.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gcshvkhrp.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gqoyqrxtz.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gixuwhvvl.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gcvbobbae.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gzqwxjrkm.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gwbyrztsk.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gdgzkfqfz.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gzcbbnpiv.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gjteeespk.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gdiyigtxa.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gpwhqfavn.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gimfbzdgb.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gejwksjex.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gsagqsier.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gbhgwqcmq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gmtvgumfi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/ghqwnidet.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gajaklubd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/ghbpgzyoo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gwjnrrijf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/guogxdyid.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gcufxpwvf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gjnlnhmix.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gccicenhr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gtjqmuqot.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/glybleerl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gcsmqrfld.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gjocezovy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/geeygvggw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gxrgfxauc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gawwovsth.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/grtbnvonk.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gvojzonhj.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gmywuilyg.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/gwnlwoyji.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/gyjijjtli.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gvbbggdyr.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/gyzjuanjh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gtdzzbelm.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gjutqnrtg.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gqrhvijei.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gxtvdzlpz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gfxhyfkaz.sHtML


<!-- 参考信息 -->