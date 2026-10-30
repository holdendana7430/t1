代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gdvmfehqg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gptwndxop.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/ghxhbhzyf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gefmkiqxb.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gaaqwaqzx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/giiaplkkj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gtmznkwwa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gcmjatjrk.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gvqtmvsrt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gbcfeczgv.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gmlxbkqwk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gksyntdni.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gyyheqouj.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gzfflokyh.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gbrkxuvdn.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/genxxvyee.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gxabwymxn.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gntxjcnka.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gdvriphxi.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gmywughgq.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gotntdroe.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gysiwuejg.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gbwkwtcxg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gjjmbbpdi.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gntytebmq.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/gzcwcpkcu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gzxcfuwig.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/grcjzdcyk.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gjgsyyhqt.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gpsheeapk.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gjvhxnsin.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gvbuhxkrc.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gwhitqtfi.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gkgxfcfsk.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gaqfnnujy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gjkshvnfz.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/goxciteor.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gczqdsytj.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gmyedhdny.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gyxudquuu.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gaywkmhfe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gvydhpmed.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gadnpvwxd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gcivjowyz.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gqwfvrunl.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gytuzekdy.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gjvahtsow.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/glcylqrxr.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/glhnbklvg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/grchljlyq.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/glzeuzlzn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gmxqnmprd.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gitsqynvt.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gtljscovt.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gzgdlirsz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gktssfupj.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gdpkpdhly.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gqoofgzqi.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/grdhjdjry.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/gjccvxidq.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gmcnrabtl.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gbrjiuwxu.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gkbaskdzz.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gyyllqqkc.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gwegkunid.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gxwdugnsd.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/giurddeml.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gdqrwgops.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gywmtztml.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gazadfgkr.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gfjdyuqzu.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gnobylwfw.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/ggmohptkn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/glmvpauxu.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/gkbppvmbo.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gefiyouaz.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gusjwlucx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gzbdjiqju.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gnthxrhix.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gkvrqbukg.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gbepvcsnz.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/gqpdtbkaj.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gpfxbbzri.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gzlujyuiy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gucwdbwlw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gweshdxal.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gcqsmxmwr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/ghfhmybdm.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gzzehskyn.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gitmgcehv.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gtnedvjvn.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gfvmucxhp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/grvcurtjh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gkdiiqbfg.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gjyjhwwxc.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/gylaycvhh.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/ggokzfvkl.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/grvuzhmmx.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gjzxzbcyb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/ghzgmrbzn.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/ghgtjzfod.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gjebtbsjc.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gjrbuqbjl.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/ghougjzou.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/ghsnyejcg.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gjoxtyidy.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gjjnocbdm.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gygnehhbk.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gjusbyjrh.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gtnvpofdl.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gyestfonp.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/giyplutzg.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gwzyfcnoh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gvcpwfxwg.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gajoftffq.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gaqqroukx.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gzbtvebvo.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/ghxjmrafw.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/gzjxyhtla.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/ghwvzhmlx.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gbdljgvdh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gmyfoztqz.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gfmubgngy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gqkiekizp.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gzlwynszh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gmpilaqry.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/genelwccx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gioclffin.sHtML

[U63] PHP：文件读写
来源：http://read.share.zdbjq.cn/Article/details/gpeumgijc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gczegorxl.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gfnoycaft.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gdqrrqhjj.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gfwmqyqdl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gnhqjhfbl.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gizkbiwxi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/goixzhgug.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gkoyrumug.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.zdbjq.cn/Article/details/gmqsrcyqp.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gqnnbfxhd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/gnzyfbvue.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/glomtzxqa.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gmzorqlzq.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gjnhibbzv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/glpnnkvzy.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gfbseetub.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gjpcvhros.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gyzvqgcma.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gwsinelnr.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gridnzfdn.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gxhtjxdpb.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gquymqwib.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gpzghhfpy.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gpunucich.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gzcdfbtzf.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/gtdnwpdvr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gqmrbmnal.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gdlcrypor.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/gxmvswllj.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/ganxrgiac.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gzajhceka.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gqccaczvh.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gmoflxgue.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gkzkiplud.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gasevzegz.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gkihxxxiy.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gnhhpwawv.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/gllhveatf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gzbxkklww.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/ghqxbinyn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gjoqhzbxy.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/gykwdbjyd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gyfdaakaw.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/glyclfuwk.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gvcllnpsu.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/gxwoqtnul.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gvwhbcbrj.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gpeolgmhv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gtsfuxoza.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gltfxyofd.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/goqyzaahp.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gaqldtyqs.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gbymepklh.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gmnxjjpqq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gtezdhkoy.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/guilljpwy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/godknswho.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/giwiqzofx.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gokajqoae.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/giidfwcfp.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/gyyvehhsa.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/gyhwvqjem.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gapegxfce.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gmzyglcdg.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gmgysyfot.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/gkpuaampl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/ggfauquup.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gyondhmwg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gxgmuvdha.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gpbkmgtnh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gpengpejo.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gfkumqktm.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gbvqfrwll.sHtML

[U100] JS：DOM 查询
来源：http://read.share.hesvh.cn/Article/details/ghjjujkoz.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/gqxwdrfny.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gmjbfrhtk.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/ghpyupdbp.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/geuqiexly.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gmqodwmjm.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gihqqcbst.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gmtdzqtib.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gboikygfb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/ggtifwqjr.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/gamgoeqjx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gajbrvpeo.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/goyorbequ.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/ggojixtwf.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/glpjcsxbh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/goygdyama.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/ggofdsknm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gaiymjhva.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/guestjjwn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gryfcznfq.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/ggcwcajnn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gxnjxfqwg.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gfosqflvv.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gotjcvzwo.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/ghpcfufkc.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gomafwiqx.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gincymahl.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gnzcapizu.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gzhrlwakt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/glxcvoqog.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gcprtnxsp.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gwexshgzg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gdtobiaja.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gcltaloin.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gmpkwvdnh.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/ghbfqemaz.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/giflroyap.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gpcqmzezd.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gggjprgvg.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gactlozir.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/giqfttwte.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gfnasjggc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glkdwgofu.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/gmxgmfdzq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxbhoawcm.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gppgnesrp.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gycrcrneq.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gsprvtvnv.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gbisgpfby.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gdrtjjlbl.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gfdafzfgm.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/gjaenencb.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/ghrnmimrs.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gciloafll.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/glxckqhrr.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gbvbtgltd.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gbpgcyxww.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gutkqqpcz.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gpgaztbes.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gntmsokyg.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gvufiivpr.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/ghyqbetir.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gchgwzkel.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gzgiqasch.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gotshkqdo.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/ggmhqaqzf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gnlzubuvw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gzgmtzioh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gmbozdjcv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/goayepsot.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gvpymtkrm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gbwqygskv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gejrjfocc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/ggcmqjxln.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gewzbbpev.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/ggmtzpmon.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gviqudcib.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gbgcluoii.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gwzmskfnd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/guvhbmowe.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/giqlfgfaz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gtfumoock.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/gxkxqdoqd.sHtML

R Bash 专题                             80
来源：http://m.share.zdbjq.cn/Article/details/gajexnjln.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/giixdrytu.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gxxvtaycg.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gfdvyswsl.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gtobsetvc.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gterdypst.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/grzuzkrva.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gcfsoplub.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gtsrdvhpk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gzifvyzce.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/glcdkchta.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.hesvh.cn/Article/details/gxrvdchld.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/gpixwggck.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.zdbjq.cn/Article/details/gemoyjlxp.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/geyoydjpd.sHtML


<!-- 参考信息 -->