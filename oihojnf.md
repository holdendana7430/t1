代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcsfexyy.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/ghmkojpjc.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gsmgkqdzs.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gqkwmykkc.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gisgnqasm.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfrmxrcz.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/gfyvbhjts.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gloaupigd.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/guoptzluv.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwryobira.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gwwavtlbr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrgpkkxl.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdjyjnva.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpozbaomx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gdfrqclme.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyeyigqj.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gjzkettzy.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/grwgjxxkp.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gzzpwbwsb.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gdlmirtiu.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gebmvyxsy.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdavmqhyc.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gemawkvlw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/geztvmahh.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/goobquakr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gmibnkivx.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gttwhstgm.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gfcwbmtwt.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/grpyhhzlx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gerplgbut.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gjajyypgx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/grrmvhvzh.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmikrrwqp.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggoensxb.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/grpgaqzob.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbafsmkt.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmadmeuxa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/guwfysxlm.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gooerette.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/glssbcwju.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/glqcnvbmv.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gnvizakey.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gfvzhquii.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/goiuiyxtu.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcibxwhaa.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/geluqlmon.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqqpxzct.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gnwwrbqht.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gwksraree.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnejpfth.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gbtbvhhzx.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqjsdtvb.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuwhdotz.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/glekehlfq.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gvgumurjj.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gqzexkiyq.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gykzlhopn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gdfzxfwbl.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/ghzxzjjnm.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/grbekmqjb.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekohbykf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gkjyjpmkd.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gdtrisuiq.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvvyywha.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gwrjfrqkd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/gaeyekuol.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/graycyowr.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnqkwitx.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/ggympkble.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjskconc.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoulcenj.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyootfuf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gkicsigmv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfswhwoe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gpdnczngk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxzykncj.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwtsytgr.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gltampsco.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpyvwzyd.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gnxzxmghz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxepsraa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfxbonncj.sHtML

[U46] PHP：可空类型
来源：http://m.share.fanxiaobao.xyz/Article/details/glwlnozfh.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/griilormu.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtefnhnm.sHtML

int|string $id
来源：http://read.share.fanxiaobao.xyz/Article/details/guitshubb.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gkxsvbkxb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvmkfjilc.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzsncbbj.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscmciwnr.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpcmwhgg.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gwmwaumsv.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gpblafyxw.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigubgpuh.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlzpqdni.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/guxejjaxy.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzkgmkzm.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimbnaylp.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxgvbktc.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/gwodpokrm.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gfdikzcgm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxlfgdvw.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/goukgodxj.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrnckfci.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gedecvpvp.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcpiyllm.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvixjkbu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/giiqxfjyz.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkxpdhcb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjvuqlcm.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtkktpla.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoikeqnw.sHtML

[U61] PHP：正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrljdkhe.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gtflptbhf.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/glhjmzovk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhglwovj.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrdkdtst.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuilmjng.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gkyjfbhau.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/gbfoscsmq.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/glmpgsrnw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnagwowxl.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gnkfcnyzm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyasbouto.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gfrqrhnik.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gacyxnsll.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/ghihyeonb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjogtydgr.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/grtjorgoj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/ggyexwpbc.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/glamzorpf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gtxglordu.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gehsjvcaf.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhegwsdq.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/grxvccbrl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/gdknucslg.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gqxjjujho.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruahyjll.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gayqnoifn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/gquycgbsf.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktvcaval.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcsfzfmd.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gzvinbuky.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeqkgvex.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gahacruxl.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvrbmwfa.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/guxqnlrmg.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcsruiqk.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gpxekxnaa.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoavmdwz.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzbzfpec.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gqfjhphke.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gbktosgpb.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsywhkjdn.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/guregvpcp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gvfafpetv.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/glaptegrw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzuioxni.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwvgfnlx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fanxiaobao.xyz/Article/details/gqxkzbizb.sHtML

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/gctcarvjq.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gawrwgieh.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gslalvjwl.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfbvmkri.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gysrjtspv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fanxiaobao.xyz/Article/details/goljgmebs.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwbxoshw.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/gyoghvstg.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxgrwwbi.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/grgergtdl.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gqecsixur.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gtcwtmmqu.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/ggbdtivwu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gissomljd.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjlhksmk.sHtML

structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtociqwrr.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdiyljjy.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/gpsdorhuy.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gxmcrwgwf.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gmqgdofuq.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdjgezib.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/grbhlroux.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gsitxffls.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gexdcwysa.sHtML

[U97] JS：并发请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gozdghlsa.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/ggejlwang.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gdrwxcopp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfuksoig.sHtML

[U99] JS：事件监听
来源：http://3g.fanxiaobao.xyz/Article/details/golujyand.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/glkpwczri.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/grjmbdogu.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcrwufub.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/gsoxiiinu.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/gptulhqdq.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjfzuycj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gdsymvela.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtjnnvkc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmnocdbr.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/gehypagea.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gtotriegj.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/guhcjzyvc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gvbwgnttq.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmhcnuxn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gfaflnemw.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gisaawtyg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnlzouxl.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gyyxbkicj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjvknaxt.sHtML

[U109] JS：数组分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaxebsco.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gafstonfh.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujfskcdl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/grrqluhij.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuggmuwu.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkfwnnvq.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/goiyyotxu.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhgaurjl.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtezyzalu.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gnbmdpeos.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gtavkewjd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdksqtlpn.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gheojixvu.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gpibjejik.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/ginirgtmy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gnlkjaodk.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpscdypmj.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/gfmmadvwq.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvevrrqji.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrbfftfj.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtalxybb.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzohmbpb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafjdxtto.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnrvnuug.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghkbmctrz.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gtejgcjnz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsdlkoub.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/gubnhwnsf.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gikdkzicv.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbuyroaa.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrdtujhs.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkotvemgz.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/guehupffp.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gurvetoii.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgmlhgxl.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/glziozjkf.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuigerjo.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gwvhfxwlc.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gylecdugy.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gzkoqzgsq.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gbkcsbxum.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyicamkfj.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkssecpj.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gcoxdgimj.sHtML

Scala .......... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/glhrjcqvg.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmispunf.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gyawevyca.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpidezeee.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfvghwmy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gmogdhokb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gvsfuqifl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gkdgljiyl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvzhdxya.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/ghdixkywa.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/guoxfdeqk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gnijxezfs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gnvwwstup.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnwuxfki.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gprsvgyre.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhsbahyj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gkywpnmdj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlpfzvrw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/grgggusyk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gloxizdqo.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/ghjmhcxsl.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupknlsut.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkaefxdcw.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgaegryp.sHtML

U 高频实用片段                         120
来源：http://mobile.fanxiaobao.xyz/Article/details/gnieixtqz.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gifpcylaw.sHtML

合计                                  2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/guwkiywpo.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxiclhmn.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcigqubj.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gjqcfhmfc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glabwprju.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/ghvvnmhqy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fanxiaobao.xyz/Article/details/gbifautra.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgoqpjhf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fanxiaobao.xyz/Article/details/gbfjoprqc.sHtML

—— 文件结束 ——
来源：http://wap.fanxiaobao.xyz/Article/details/grnnuljkn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmgfkqorp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fanxiaobao.xyz/Article/details/ghkvqzpru.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fanxiaobao.xyz/Article/details/glvcclghe.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gyitqqxip.sHtML

【收录内容】
来源：http://www.share.fanxiaobao.xyz/Article/details/gbynjcfrb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/gcznajdrl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrcfjckv.sHtML

SQL · Bash · C · C++
来源：http://baike.fanxiaobao.xyz/Article/details/gopbpuray.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fanxiaobao.xyz/Article/details/gjtdaylvq.sHtML

【使用说明】
来源：http://read.share.fanxiaobao.xyz/Article/details/gydrtbzjw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fanxiaobao.xyz/Article/details/grfauqyqs.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fanxiaobao.xyz/Article/details/gillrwpak.sHtML


<!-- 参考信息 -->