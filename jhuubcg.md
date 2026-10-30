代发 wailian999

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gexbvlzkm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrqbjcec.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtyjgoir.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvoxldmet.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzctoioz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gakmnqtio.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gepknpcrf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gzuapqnql.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvokvsua.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gvgsesctv.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gvehstknw.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtezhgnzk.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gayjesngo.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gyggzwecy.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gfflmcuhb.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxdvwkyy.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gcxfrbwmd.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyikohqo.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gznlcviup.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkatpacfi.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gdksckzss.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnajuusqh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvmrjsqa.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gedalstnk.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gxnarnhcs.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvpqqbpb.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzztkuzy.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gopsfyvhf.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/gshjvyzbf.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpoufezr.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmponbci.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grndtjpem.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gruqukuxf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkgzplak.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjudvlfn.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gbubayybp.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gewtrypko.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbipsang.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpkqvvpm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gelzuojgl.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gshlsuypr.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/glvacnsum.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gsceujbma.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzwayggb.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpwvmwuh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjjcrkji.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiprjvut.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwizggkff.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzfgkqxv.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpesmbawa.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gejnsfvee.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gtcfibnvo.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gqlhvfqwv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gvcpaxind.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyoexxhg.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/gmhzzcvxo.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guakldxio.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gbninbfxm.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfrmnumi.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfackxing.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gctuilvis.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gwfgndkul.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxfkkfcc.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxdhkfii.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gahlxrsbx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/glantiocg.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgvtndow.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqblypes.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gbbtjbwmd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/gxufqgzcn.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gtuouxeue.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gvihdysqv.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkcbzonz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwuebxwz.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gozkqpsko.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqatrqybp.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gcbrgvaov.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeqmcllq.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrehvyym.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghigeiasq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjavphidl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gtqeckvqi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gudxdfuks.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouzulogk.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoqghpoo.sHtML

namespace App\Http;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkuvyxtl.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/ginobhhmh.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gxyweppxw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gmzkashem.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeztwgwn.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomnyixuz.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/gostaqfne.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/goaxpavwg.sHtML

int|string $id
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcfqqpor.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoxvhqzm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gupbunxdl.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/grxsvrqie.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdkstdkm.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gaygmsvlz.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdileexe.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltkfpqtj.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/gqrkabqsl.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/guhuxnprs.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtbspwgj.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjfqapur.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwxvcwlx.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gdejwgpnr.sHtML

$obj?->method()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcanlgcev.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/grgkvaocs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpjouojh.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgxbbugo.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrenzasx.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwncpuuno.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gabnzqfys.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrhsckod.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gvnhulcto.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxcjejld.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzmpbeha.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfkbogxw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpigxjqlt.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtxocadv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnlazfoc.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/glzjtqnqu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/gzrsqvhue.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyftnfpm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbvpniyo.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gardrrons.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsvltltg.sHtML

[U65] PHP：会话
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznkebykv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrlmompz.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnridrndy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzsqjpdl.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjowzsux.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fanxiaobao.xyz/Article/details/govedvxwe.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/gkguxrgvb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/gdofhxwst.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjzlikzf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/goxpxtpyb.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqobqmdww.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gpqopeljp.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaifvozo.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gchpkcvpr.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gunmrbltr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyewptor.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gferummsa.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/gdobffxwl.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtyltbzg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjtxzzjx.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/golknjqlf.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhyqmbhp.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqmbhici.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipqlpcvn.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgyywbph.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjgctrqi.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gfflvnjbl.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhaalume.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/gppmireqy.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/gwmktnatq.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gencaycak.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fanxiaobao.xyz/Article/details/gohrammvu.sHtML

[U81] JS：初始化项目
来源：http://wap.fanxiaobao.xyz/Article/details/gjkyhjbpd.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/gqjqplcry.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhcepbgm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gduisxnjy.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/ghlkpxrxc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/ggihvtnns.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvtinepv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/gvujfmhdq.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/gzhtgperz.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gmcymrcse.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/gwafmuybo.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/gzehpvlat.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbxiyzap.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrinjtfg.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhxzjohx.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gxvsgprax.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gkpizbwfr.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gtdhiwavp.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/gwybifmto.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrsmpyyf.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/goyiywuyo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gclofblre.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gazkteoqw.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfcrnizr.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gbpzixcaj.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfacjnzg.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoatfzku.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/ggqpziqvl.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gvtqcfzcj.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gfnxofmju.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvzedgmk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gdydiyyue.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gagkqfrtx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsofluxp.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeqgnedm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/guagstfkp.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/gdcwvfcdi.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqnqetzy.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gscdqlsfd.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwropwou.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/gocadhfqk.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gaunhvnfw.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gegrduyhd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/givhrtdsg.sHtML

[U103] JS：定时器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsungzfkk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/glorfflod.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/grzrpfjse.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gzzsolbor.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnvbaljy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnzaqnvx.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/grghgbvwm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavsmeavb.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/glvjtuazd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflmbztmm.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/gubumzqcz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gchcilzwk.sHtML

[U109] JS：数组分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gegctzeyl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhmmqzox.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiwfmosc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsyswwva.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqvefqdr.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/glhrstikc.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/givqmwmtw.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpavspymx.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/grblrvoes.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gzwxwpqoa.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gyxahuaah.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbgniphi.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/grrovborv.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/glbzeqkii.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/ganswfqwy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsmauxnm.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gplkfgbmp.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqdzeymp.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsrtkwww.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/gyndmdizt.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gsodgsdxv.sHtML

npx vite build
来源：http://www.share.fanxiaobao.xyz/Article/details/grwxlvonb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gbdbraxzz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gnluzgflj.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicgtyiio.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyaiprnwf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gsougqzdo.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gmntpwdwt.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gmokybnow.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gvzcpcrus.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/goccsxiaf.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjupqnvpw.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnhygtjp.sHtML

Go ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfsxndmz.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gldbfsdrl.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gjosvkrah.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gwogeiglr.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtxsxdyu.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/gttzfgrey.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gsaxwialh.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxksynvx.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gvpgtcgje.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/gbsxikpur.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gfizhsaml.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/grxdwxisb.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjplarca.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gliiknxto.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gtjgujngi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/glozkrkgw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gieixgrns.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdukmpine.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/grzwzadzr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/gldkajydq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gfolerrcr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gfxuortbv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbzseisx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/grdswkkep.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gqstyeeaf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gprbbmafq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gacifgifo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/grnulyqeh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaklqawig.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/ggjjmymwv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/ggkigzygz.sHtML

Q SQL 专题                              90
来源：http://baike.fanxiaobao.xyz/Article/details/gpumlbqwf.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/gwyieeyvz.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbnskxue.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gxyftuhcf.sHtML

U 高频实用片段                         120
来源：http://www.share.fanxiaobao.xyz/Article/details/gtggzzptg.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gshpeznpd.sHtML

合计                                  2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gkjoiruoe.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gphyunwdt.sHtML

使用提醒
来源：http://blog.fanxiaobao.xyz/Article/details/gukerbpqk.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gutiuzmzm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/grbgdxpoc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjbofciv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmzasxip.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fanxiaobao.xyz/Article/details/gyifbmmpa.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdhwwezn.sHtML

—— 文件结束 ——
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqyxcvse.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glppkbkya.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fanxiaobao.xyz/Article/details/gslqwdcjz.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvjcsujb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmtbvujv.sHtML


<!-- 参考信息 -->