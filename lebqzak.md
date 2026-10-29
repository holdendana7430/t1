代发 wailian999

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/ggniupunq.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gtoqvwjev.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gsiwetukb.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gmwuovghi.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/ggshqxklc.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/gulkttcgu.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gxjqnzqie.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gtyawxkxk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gyvyeftul.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gweofrxow.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gqgwoolyu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/ggimeclyd.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gnqpjkgys.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gsnmdrnec.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gzyyefbrr.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gmzthkehx.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gllqvdoqi.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gtqowyoyr.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/grhopktiv.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gdjrmzxpr.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gmfpvkzww.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/ghwzzqltg.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gaqtfimoi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gamyhhcem.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gbknnljqa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/gapgnfndc.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gstkklgga.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/glbxljuai.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/guugsziqk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gmyhleabd.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gkogmssoj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gfbvzakkh.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gubzfqjbd.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gohegrype.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gvussdjqg.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gpsboiybp.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gkjlkjvej.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gqlzmylyr.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gokgoktmk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gnmnooxjb.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gdjyyplxh.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gzoqmnber.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gwrvoohbp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gjdsegqfj.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/ghjqdjwce.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gtupddieu.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/guufumwap.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gvreokgvg.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gjclefpmn.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gftgsmqff.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/ghrzuamhf.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gxgpjhqwc.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gzkwgkgpz.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gsoecvoaa.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gakxcrmfx.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gflrzzeyl.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gnvwalavi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gwkdnlzxa.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gudwomnbg.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gjkzqdyar.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/guwqhjghk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gyguqepvo.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gzcomphby.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gcpyxwerd.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/ghiljtjjm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gpkrljbay.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/grpchjsve.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gzcqberyw.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gxftblpud.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gljwmvbmw.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gsrscmuoh.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/goexkqifj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gyfpdnbqh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/gwkpscyou.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gshkstszv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gacmigttj.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gwkiqbcsu.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gmxjgfnja.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gifvfpxxg.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gpojoexel.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gtgxjysvx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtlvklzhz.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gvbrxhdtc.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gefauwgol.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/ggzgslxpu.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/grjuytwsc.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gpeyaotjc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gtfpdtqda.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gjvoqbmqp.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gyzscrpgh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/giifhfrro.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/gigqadpxs.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gcebxcwox.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gglcpmnln.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gfzptxayl.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/geafdtrfb.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gtqhknmkh.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gtuokxtfu.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gpipvboyv.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gbbdxmena.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/ghivckvmx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gummkrcbe.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/gbutchzpu.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gzcamcpsj.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gtjvefgue.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gotdqthju.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/gsdtsxdxp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gdrewntug.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/godcekchm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gdzmkygxq.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gdkusohre.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gdwbksrqh.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/ghvsduwjc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gzzwdwxtb.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gziygdwgg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gadjhsyzf.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gpitdckap.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/ghbhzdlto.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gzfsallbh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gmoqlsfpd.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gnlkulyyu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/ggrewlqvu.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/ghnfucrou.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gvjadclat.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gpiatqcdn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gwpeqhxdg.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/glzeqdxmb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gkzuwestq.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gzhiwqcnu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gfzmwwmnf.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gxypqgbkm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gxcrgvtwm.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gookficir.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/ggihfhpoo.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gynzpwviy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gzvfceint.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gbxiiiqru.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/gnvxckqds.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/gvdfqkzhl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gnfxqqkmc.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/ghqqwgohe.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/ghsuskdgm.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gtskvnzmo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/gojsnrhsp.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gvmqhtmoh.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gbmupqika.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/grzpfpcgc.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/ggxvdfjaf.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gjpnlephf.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gcfrgfpfk.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gblvtbaop.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gyiewzezo.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gcjrvoyic.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gjprxzkno.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gxcvzeihc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/guahffymg.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/goglrgkvj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gvhuzyybz.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/glgkvdesb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.hesvh.cn/Article/details/gllaralhe.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/ghsoozlmx.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gachwpboh.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/gzmqzlcfb.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/gmyowjlnw.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gkeidvrrr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gjmgkllpk.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/glsvnhatm.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gxygzqrrm.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/godwootij.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gpbfvcjon.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/gjwrgpfbc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/ggzvbbdtz.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gejjfrybd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gcmidecqj.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/gdodtlloa.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gspvgnhbu.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gfbxzsbis.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/glaveskme.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gkrvhecre.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gsxmshbkn.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/glcdrfkih.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gjbvhkani.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/gbmqotizl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gwatmibsh.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gjsopdakg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gvtivarvt.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/glysshmkz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gltqxqnhh.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/glhfjoebz.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gdoctcdfn.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gfubekkld.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/gwaatbpib.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gsuvjnhch.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/godraqiqe.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gkeuipdkf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gbhtohoqs.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gmkguaeaq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gvsvnqvpw.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gmkubonhw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/grziixbin.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gglfhwiti.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gkoyotoyv.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gpwxokqqb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gpgkbmniy.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/grleyuqyw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gxwcozyvh.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gjdatvqym.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gnpcfxnut.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/glzxwkyhc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gxitfuzph.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/grzlufsfe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gbuvzlrti.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gjnvkkfsj.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/goalxjdxz.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gpeckiozr.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/guzplxvzo.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/geuxsshzf.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gdvfxltma.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/gfuurxvsk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gfxilwhuc.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gozgntwcz.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gdznnghvb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/grywukeek.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gnyilhpgg.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gewyxmkbr.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gdefsgukg.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gmfwhkejt.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gjkcaqmcd.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/ghtmgublu.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gcoqypidc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gsmslstxb.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gbmzuimqh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggkowcyme.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gqrfzntxv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbxkqmsjz.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gfizhqcsl.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gdilncdfa.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gwvvmcksx.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gysmibbxi.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gwpwmdsaw.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gevarddgt.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gitxahunm.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gkwmtjgeh.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gfayzsjcg.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gyyuzujkx.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/gktflaonc.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gvfyxtfaa.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gbqqtdndc.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/ggfcymoia.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gerbdkwkt.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/glpeeqpko.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/govgkwmyg.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/gqsbsotlx.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gwdewlypj.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/giisngtel.sHtML

按章节统计：
来源：http://baike.hesvh.cn/Article/details/gnqbpfzax.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gpsrxdswp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gzqtplagd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gaihpjbwi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/goliktxnd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gqajxzpnc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gvubqivsq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/goalvhyrp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gebjdnprg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gmeasoiel.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/ggewgrick.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gumqfwxgy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gvzmvlhwj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gyofkndhr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gfnkcxqwt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.zdbjq.cn/Article/details/giqbckubz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gtkwgfcxo.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/gbhpokpql.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/gcxxdiwrs.sHtML

S C / C++ 专题                          60
来源：http://mobile.hesvh.cn/Article/details/gsjqkyifh.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gdprdzius.sHtML

U 高频实用片段                         120
来源：http://baike.hesvh.cn/Article/details/grhtuwske.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gfidjmzlp.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/glfpxeqgh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gurmzboeo.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gjauopwjg.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/grrrpvjgt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gummruuhq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/gnnajbmug.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gshxvydii.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gnsfgybuq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gaztdsjag.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gzqqswyye.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbefalfib.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/gliyyxonj.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gcbbwafyc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghtkpuant.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gkamclkzn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/gdbdrdpvs.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.zdbjq.cn/Article/details/gwxbmfuio.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/gqmknnhlo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gloajijbj.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gtasjsrla.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/gvwiocmga.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/gdqppubas.sHtML


<!-- 参考信息 -->