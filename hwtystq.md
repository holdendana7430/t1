代发 wailian999

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/ggkloiblz.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gfywectcj.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gwxmxtyhr.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gbywjtdnb.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/ghxofrjsd.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/giwvrlvkc.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gjjpywymk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/givmmypls.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gclrqskws.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gdezucxvy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/grzpnwpry.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/gzpgxtmtm.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gzwhlwvoz.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gcvknjhqm.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/ggrunpbmn.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gnjjhwqbj.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gozxmgqku.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gaufkhwkh.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gqeumqjhb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gmnnejxzt.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gulsqwykt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gwsqulyfu.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gabrlczdn.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gdktqlotq.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gaqkkolfx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gwgedyceq.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/ghcadpkle.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/glziglvzi.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gbnlmrybb.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/ghgqkbwlr.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gojvfrgti.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/ghdcfcmuw.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gqiwmvmwv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gkvikjtuk.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gwikwswie.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gbxbvmsou.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gkzyfumre.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gfjofyknd.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gnddaxgqo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gowquugkf.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gholdaarj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/gskwaxbga.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/goshoawmt.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gzsvtcmzr.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gbtpnhtyf.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/giyuwalyc.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gdqoaafpr.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gwltwdhar.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/grrmzkdlr.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gpvdujebr.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/givzqxatj.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gkqdfclvq.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gvaugoywm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gpxpxjjyp.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/gfzuugvmx.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gjymhjyoi.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/ghjrbunqw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gmrwkskug.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gpxannufp.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gddxkqxko.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gxiykqbwp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gzvtylptd.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gtbifvfpa.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gstewpqso.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fehbvm.com/Article/details/ghslgcjzd.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gdjkybxvd.sHtML

[U40] Py：打印到标准错误
来源：http://3g.zdbjq.cn/Article/details/gtavzwknv.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gwovysyrn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/grefhfxxq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gtombuoxq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gbvvwhxpx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gkrxisvtx.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gkgyttuns.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/gdtaqcukq.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gswyicyln.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/glyxynnzi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/goorvcwnm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gtqjlvejb.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gkdpadvce.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gtstugjvz.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/guwhbwtqx.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gyvcrxxrh.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/grayozpes.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/gyurdnbyj.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/grcmulwrb.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/ggdiecjkv.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gcaexosjg.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gdeorghaz.sHtML

[U51] PHP：数组解构
来源：http://3g.hesvh.cn/Article/details/gyujabqtz.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/grgtqjspj.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/ganjowoms.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/ghknskmxh.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gtulpalqk.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/gxcdwfohr.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/ghxjpqima.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/giickzslh.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gdcxmaqoy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gnqqysmyu.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gmstkmgzn.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gaolbbhub.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gturwkygh.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gweebbxik.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gbxmaehsf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gdjfgyuab.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gdcpriyny.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gbwrnpafd.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gvdbvddmb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gycniwest.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/gswbmlvnu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gsrgodfmi.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gyqtvydgv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/givzteggh.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gsquvgmfp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gbniggmnc.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gwgabqjvq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/ggvaurmzh.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gufgcrufq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/ghlxfvuwr.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gjswxzini.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/ghzfipehh.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gxqolbanc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/grkfvakck.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gomndwxeo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gvzwyeper.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/gifzfyujn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gzjtdcwuc.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/ggrrsvxbh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gjkrzcajd.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gvxugvrxd.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/guyzrwqgs.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gjfysszpj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/giykcfczt.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gxvsjokpc.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gopbyzgkh.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/glbwdsdjz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gislmdlcd.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gxjokfimp.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gqqksahon.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/ghlbekqdj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gdxibbvmt.sHtML

[U77] PHP：模板渲染
来源：http://wap.zdbjq.cn/Article/details/gntwlnefq.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/glblbakcy.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gstymkbgl.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/gneauwrbr.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/gbvuiyhxs.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/gubqxwpaj.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gvrnqrvgd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gbgjumevc.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gqnppzbwq.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gcqpyhbbr.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/govlwwusw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/gixkwvebi.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gvulflnha.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gooifzsqo.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gpbunctas.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gcexcsnfh.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gupiimsul.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/grglznpzn.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gqenxkspa.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/grylxxaky.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/gzfkuncfs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gnzgxcktn.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gyorlzoxv.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gzhrzcypt.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/guyftplas.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gocldqfei.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gdpqoaxgi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gwxiiucgk.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gtdnzkmlj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gqbpnlbcu.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gslawnjqy.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gptbdnuzs.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gyyieymia.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/gguoykabq.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/ggkiabugs.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gnkwisssq.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gahgpxwwz.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gkgvlpfci.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/gfpdlzwoh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gserxyoox.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/ghbeqmiaj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gggptctqh.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gmzssvrzt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gqhgiudwi.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gddegebiz.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/gqzunxnyh.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gpdkgrbse.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gysiakycd.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/grbkepkcf.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gmvxixipq.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gzthwudur.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/ggnapvsru.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gyfkvreiq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gxvqmppkb.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gfovibodc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gxxgmgvrq.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gmgupljlf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/guhbrxbix.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/ggrucpccq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/ggyiudbbu.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gfsqrlfmh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/grbtiwonc.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gtvqtfwmn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/galitutgk.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gnvmcvzec.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gsnkqslfk.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/gtcgsqgdm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gyhuluvht.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gszpeozck.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gidbntcvu.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/gsfjxhlsq.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gkcmqplby.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gqmivwscm.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gxaeellho.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gnluwywsz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gyrxifsfn.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gkpwovvij.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gobrlikzb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gaxyzsplh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gfeglqubi.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gmymsonwu.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gzbccmsxq.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gfkctznpg.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gyjdvvygn.sHtML

[U119] JS：生产构建
来源：http://www.m.share.zdbjq.cn/Article/details/gurwazkvb.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gotwmgugr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gobdplhqy.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/giqgprqqi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaauabzyy.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gmtrzoukm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gueyyddwn.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gzwisgdfg.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gqktdhzqx.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gynzfxfkz.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gpnlopwgc.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gomrddfob.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gtqdjnncu.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gtblimuky.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/gecsyooul.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gqcgomiun.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/gouqcsbab.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gnhbhulim.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gqnzfnzyd.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gmtuwygtx.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gvnpgwlxi.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/grwitwauq.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gpmuobcuk.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gfsssqyei.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gzwiozzaf.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gkmmgexwr.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gemvirbfx.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/gyeshgswp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gyutmwchw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gnniufxnq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/grkjynrfa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gqarddwre.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/guozxmrrp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gittzukoz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gcmlledjt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gniubhilf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gkqgcoima.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gjzcrmwym.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gncopowel.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gppmwhhic.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gewbpwbpp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gzgxilsgu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gcbyytvzt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gjgaodcsv.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gvpcjnofz.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gyqohkjco.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/guxtiyatv.sHtML

T 其他语言补充                          60
来源：http://blog.hesvh.cn/Article/details/ghnuiglkt.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/glajfvtbo.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gwnshgzuh.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/ghstcrvgd.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gphfnumev.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/gzfjzwthd.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/godcccwqx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gwzjmfudp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/ggzcjtjau.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gttpxhsej.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/giqosbbrb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/glaxhcaoz.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gdvzubnrq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzazfvhsr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/gsjbzltua.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gubfhshqv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gztazhhdd.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/gzxnebnsx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/ggyfojafa.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.hesvh.cn/Article/details/gflfzryok.sHtML

SQL · Bash · C · C++
来源：http://www.blog.hesvh.cn/Article/details/gbjxudxja.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fehbvm.com/Article/details/gwhlkecfj.sHtML

【使用说明】
来源：http://mobile.fehbvm.com/Article/details/getnqowuk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.zdbjq.cn/Article/details/gwrjunisi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/gjzgjmexx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gbdrevrkh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fehbvm.com/Article/details/gwqhxmpec.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gaxmpgbij.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/gecbkbznn.sHtML


<!-- 参考信息 -->