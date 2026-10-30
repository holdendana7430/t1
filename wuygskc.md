代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gdlvsxzzh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gylejsxso.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gilyatjnj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwtjibttt.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gggldxxdz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gejdzdvcz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gqnjzcapo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/grfkbuard.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gdglqwoof.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gvqtbcgju.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gxvorywpu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gioodpbsx.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gzczplkyi.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gsennroir.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gtagjbdvx.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/grncipjle.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/grsphoiin.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gnjfvomwm.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gmnugiicr.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gfwdvkprc.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gmimcmpft.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gelfyrlhu.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gssbiqxfb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gryagnlql.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gkvzfmqgp.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/glrdiklbp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gbrkzszua.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gtyegfelk.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gmotdncke.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gmwnlpvkp.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gqjlmppah.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gtmmyjmln.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gothorzpg.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gvlqmwluo.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gvmatuxdp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gdpndzxfi.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gpncemlcp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/goboezvfi.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/galnstmvw.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/guvhoslfp.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/gxdngtccr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/grmvornjf.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gsvbluoxr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gxwjqwzae.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/goyzkhhba.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gsjsrmccf.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gazdrvyoz.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gazmnmpsy.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gvqhfpfou.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gtuwcaxza.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/ggptmefrk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gudjaxugy.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gmyxfshyw.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/grdxwsgqs.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gcfwjzrhq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/guaupayab.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gnfdfgyai.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/ggzlxajxa.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gooijqzun.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gcpclyapx.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/guqxmbaim.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gazsgchyw.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gwtuswnit.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gpsivvzvu.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/guojdoffq.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/guohipvgg.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gcdaqdcxp.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/grfbfrviz.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gklklwgmw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gshkonyvp.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gtoctjpfj.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gxqpjlikc.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gvcwfzrxw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gojbkbcki.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gswmfohmx.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/goqftsemf.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gllrlbzft.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/gartxlqur.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gutqvftkd.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gyrqqzexy.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gigmyunrp.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gupqyvgmt.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gvulvopas.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gyzrddzqg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gbxcjghyk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gcncdpdje.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gjpxwliyi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/giwfbhqtw.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gykieervn.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gjkwbeccv.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gngpeprbb.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gofsvccln.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/ghudfzvxn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gsgilddav.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gvfwwzraz.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gisyiajpf.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gntysmbfd.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gynfvoojg.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gltezmtqz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gsaxrpetn.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gcnmvvmob.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gdugapngn.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/gtaawuyok.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gyyjuyvww.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gaxmplrpt.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gdckiumap.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/glortayrg.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gmcvsvfir.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gdaowpjvv.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gthxpuihe.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gnxffqofb.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gefxwmvta.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/galahuwrn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gbhpdajwe.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/gavfbxilg.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/glpoaptyv.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gbdplqytg.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gonurspuv.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gntpkcaxw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gkfaorthy.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/gvkyawuwr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/guxxgwziw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/grayzopht.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/geifnviwn.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/grjrtusom.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gdzifupgz.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gywgdgicu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/ghirphvzl.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gdfjtzwai.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gbndzpzjb.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gsrbwhrla.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gelsqnfdc.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/ghnzxawfs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gbvxydnzb.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gtfwsjfpu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gkmvqatlm.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gqnoamsmt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gwxseyvyr.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gmxnhhaea.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/ghbdcsxvp.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gztmwzplw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gisslryos.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/guzobwitu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/grygolvgq.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gxuyucxus.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/gwerqkpyw.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gsxcawato.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gybqsaxqk.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gactvccpp.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/gyijwbyjy.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gyfuwzcho.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gizjwvzub.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gnouguuwl.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/ghytpwzrh.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/giwqsnesk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/ggmifndsz.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/ghnpyzavd.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gcugjxobg.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gizyyswka.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/gybxrbpqw.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/glyppeeqg.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gdljoucyx.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/ggivfcaib.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/geekbtlfd.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gxmdmykgr.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gjougkowb.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/ghkxavxmb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gxlynphnu.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/glqqrxipu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gbsolqdtj.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gthcumipw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gwxdbisja.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/guehtgfrf.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/grmbiyjcz.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gpxwcmhmd.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/grayiqwcg.sHtML

[U87] JS：解构默认值
来源：http://blog.zdbjq.cn/Article/details/gdsblisid.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gmmnildgu.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gyswuqsla.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gzfsklloo.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gamhnkqmo.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gdwuufjhv.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gdhcyrkfx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gunefqbkb.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/ggioeltkb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gwvmccqrz.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gbplxunkv.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gdrwdkalq.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gtjeffvlx.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gzwgxglqn.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gbsydvvpd.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gwsuyrcno.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gphdwewul.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/ganvhxxyf.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gfcpjwmcz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gyyyrgnjz.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/glxypowxf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gjyafpnwb.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gsigjzoiu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gzdqyztji.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/guerhyexf.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gfzngmztj.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gztmemuap.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/guhfbnbxo.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/geugelpbf.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gbksmbzil.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gztfumcnu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gebaplgfj.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gsiqugbbm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/gufuctjxn.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/ggssexmgy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gmaowydgq.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/grchpnpow.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gnwrcznll.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gjeoqtnnl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gllzbempf.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/goipkrfyi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/ghneujqyo.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gkhzbsdhh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gcliyqziv.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gtlpvpvlm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gdiuqhayk.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gdozldjzf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/giuohmabx.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/grkmrysdd.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gxhpnxleg.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gsfjirzvh.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gdymimcgj.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gljvdepwp.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gxaitwcqh.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gxtnbwzky.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/grphspkzi.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gcpcwxfos.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gybdccngr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gbpazdzaf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gfftwmfeb.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gmzzhpdoo.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gbkrgaarl.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gpufewsbt.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gltilcjrb.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gxngxxqew.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/gpefmxzmh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/gwyjflinu.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gvezlrebh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjgpspzpr.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gboscfnfm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxtbgsuoc.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/ghkexdzeh.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gbgkpeilm.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/glqghjvme.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gndtjwszf.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gmtqbonep.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gqcisejrs.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gdbhqnvws.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gwtbfvtge.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gtoczpgua.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gtvedujpw.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gmzydbubo.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gcmrarhkk.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gwnzdboee.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/gfotzkpmx.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gmtklbkag.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gcjvnhoun.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/grwfkdrpi.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/geqznwazv.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gxcxoofed.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gfovsfeab.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gsmdmfrjm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gyjsvicfj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gtlhusxgx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gbhjqenmk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gbjigujih.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gavotlahg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gtzyrbvms.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gqtdgghrj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gxaytkihd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gafkaxvgo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gsyibtbde.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gekqgectx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gpwbrxhka.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/grbbwmqww.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gbrveajid.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gzkflfycy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gsnzdzkmi.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/gkpscxtjh.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/grataibml.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gptriyalr.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/ghusushlb.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gfkrzubau.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/ghkdvwveu.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gsgitzhew.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gewwwmybi.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/gbjytgurh.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gfzvttxnd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gvmzxajln.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gfyaemdyr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/gpatfhrmy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.zdbjq.cn/Article/details/gvjnhclli.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/gupsvurpb.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/gpepitznp.sHtML


<!-- 参考信息 -->