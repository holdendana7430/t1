代发 wailian999

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gokmtldnr.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gkupnpeuf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrpfceok.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/ghpudrhef.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gzixsbwtp.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzychely.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnordcobc.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdshftrs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdsqoafc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkisooda.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfbpwuht.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gubvqniug.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gkzctikzg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbmxmhqc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gscinloma.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllmotsow.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxhlkmej.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gffwbopct.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gdefmnhry.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gwdrdxfqd.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/ghtuygdhk.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuugimrz.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqgcjlvz.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfuqdtmz.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gulnchjjb.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gryccpdpk.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/guznypdbt.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gsurfyznm.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/grruprkdi.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkssyvpgh.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/ghqsoklbe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbyshfun.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gvhnxwovw.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnmwqbjn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhbhahme.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghebicglk.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gjpasepzq.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/govfjeged.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejtnurkh.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gguxhhcal.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gssbzacos.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gtgfvruor.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gleworfvv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gxgmkmkpf.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/glhdidkbh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gynyiwgdz.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/goimozwol.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnonhkzy.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/grehbchpu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gstgiiach.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gkshidvpq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gleqtnhnd.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/guwiilwmp.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gxlgpdacc.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjooufyv.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvumafbv.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzhzjehfi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/ghatydjyp.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnnploul.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gelddbfbv.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gczxruoyb.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxuurzoh.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gukltmpjs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyigxuak.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjkmzatw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssvuuauz.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gtmraxjqq.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/ggceitlmb.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhyoldaa.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/grxtgvjdz.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gaezftebu.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gimhxespm.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gltpaqyov.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gbefymnkq.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtnvpzdf.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/gllonkoxs.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadtsapin.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gereytvua.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgqlrdcx.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gynegpvgp.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvxtgbpt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/gwtcqfqml.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeyzwwgu.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmtjrqnj.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gvsvhiotp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gbaqtozpd.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gkvxclmmm.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjkzadde.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gwwbuexbg.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbwdtxda.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvyhrfjv.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gsomqzcej.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gjsmbdxnz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gsqdgnljd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhfdjfsd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/gvrlvxwly.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/geauqmppd.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gindaphuq.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/grzqsvrvh.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gfdrzxlpu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gtlcnktnw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdwlcctdd.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gonfjkwry.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gouxkulcg.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gajhlylvw.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/glkqrvwln.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpinpqhto.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggapwzpkk.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqjdmbji.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/grzbewhiy.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/gndqkmser.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gqkcekjuj.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfyfbdmw.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gakkjyfvm.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnivrvjb.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gahmxsgfp.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhahttmu.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtklijsq.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gmybqyyip.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/gpfmelvby.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcxadxoe.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhxrerfj.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gexkocymh.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzphoeuf.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gcalhzsdj.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpkazade.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/glpekgome.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gpswiwbhe.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfotdwssm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gjqhjasmv.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gcmrasuqw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcjkbgku.sHtML

[U61] PHP：正则
来源：http://blog.fanxiaobao.xyz/Article/details/gnswcfxlh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gucmwcowy.sHtML

[U62] PHP：日期对象
来源：http://wap.fanxiaobao.xyz/Article/details/gspbtfelq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/geqhxmwgb.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggemcfyww.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaejlwald.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgkqtawk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxquaucqn.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/gzfozdzbg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzjtpmyp.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjhnpofd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/glzswatsv.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejjfdpjv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/giepwoxds.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxmeagdh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpzvsmfh.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvgifhdq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glosizesd.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzywgxxhg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcuwfyfo.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gtzeqlhgv.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpxmfagw.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzdldolc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzpavjwu.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gejwephvj.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/geupoxsbt.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/goxmtehhg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/gppjrbkhk.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/gzfcgoxgu.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/giakxqqrn.sHtML

[U76] PHP：简单路由
来源：http://read.share.fanxiaobao.xyz/Article/details/getoxbrbi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbaxtonak.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gnskpxefi.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuoctslt.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gsnwowalu.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdtbbuso.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/grfaaukvv.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gndztmwhd.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbnoqslh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmncvapz.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/gxrdtwbop.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gerijwkge.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gdibucwyk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gppytbvvp.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuginyms.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/ganczktcc.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/grgweneff.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gldodiizr.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/gohisrsno.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gqewgcqgy.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gepwdqtuz.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflmyqodt.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlqigvdk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/gndtpvslr.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gorvmhfhz.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsydnqkzp.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/ghkbkzemv.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gubikiesg.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvkdfqnd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtdiktmx.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/glfizloch.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/grlupxnpo.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gfxtyzrwu.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfusbicsa.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gramizplk.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdwyojyy.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpdwqkqx.sHtML

const double = x => x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaypiyrpq.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fanxiaobao.xyz/Article/details/gnatnkjov.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gqbdtuhtj.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gbykgukfy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gqtgixcjv.sHtML

[U97] JS：并发请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspvjcewb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gyltstcxf.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gzkffaazo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlhpfwoj.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykwuhrij.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gehchjvrq.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzdjhwtn.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gblcfjtbm.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gvairwzba.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmaodnae.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/gxoytjolp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/gpoivyjne.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/geqdzabfb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/gvqdbdncj.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnwyzvvv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/ggpdbvmub.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gdsjinrzu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvcpwtpe.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gvszbbzjx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxgocnfj.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gywxmhngi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiqsshyh.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gyveepywy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/gphqygprh.sHtML

[U109] JS：数组分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpujmaiyp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnrvuqwe.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqgnqaep.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftnzgydy.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gvizskgnr.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/geliaavhv.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gmtjashej.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gibwkdqeu.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gencwkwbv.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpovopsip.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvluswlz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gigebmszj.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscdxuhni.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfexcqzrj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/gsvxvppbm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/glglebwnp.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/grlorkadp.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/grazhkicn.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpunlqdal.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gouqdqvpr.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyapssayj.sHtML

npx vite build
来源：http://www.share.fanxiaobao.xyz/Article/details/glvfpqwqf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvlonhmj.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gglvwhmjd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gejorwfwt.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrcoimfb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/glfjfjsrk.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/gldiytqzx.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfijktcd.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtfwckqx.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gkezekygt.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/ganmycveu.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gdbzcaabl.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpjiroty.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyewkmhu.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gszyecsdz.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdgxgean.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gklypoylz.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gblajkxis.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnbvdfey.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gxysrughj.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gkxwpupan.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gngpjnchk.sHtML

Perl ........... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpodawabe.sHtML

Scala .......... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/glbhndpaf.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggizofwqs.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/goztnrreo.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gkvkyfvci.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goindwtgr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/geydnchfw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfomkdweu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gcylagnoj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/gidmhdppv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcxhxxel.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/goaqdbtcx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gilmnjsrw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gupuvaflp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gjzcglvxz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooqeijzb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gjxztrtuf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxmtjsvg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gvkcxnubn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/gwegxolfr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqfwuuvg.sHtML

Q SQL 专题                              90
来源：http://www.share.fanxiaobao.xyz/Article/details/gpphiilsk.sHtML

R Bash 专题                             80
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvlmsvdq.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfzmrszs.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfihnejwd.sHtML

U 高频实用片段                         120
来源：http://wap.fanxiaobao.xyz/Article/details/gfkdbqhlr.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/givojjdcg.sHtML

合计                                  2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gvzdiblqz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gwszcrvpz.sHtML


<!-- 参考信息 -->