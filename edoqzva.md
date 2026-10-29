代发 wailian999

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gfrducqgc.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gttenqkjn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/ghdxmayyl.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/ghdthnpzt.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gtlevmpjd.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gjzkunqhu.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gygiyrbxg.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/goadflbiu.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/glvdmphbg.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gfauyjyhe.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gweszbnjs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/ggpnkgzai.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gjpqsagmg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gjpktaxvx.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gbyrktobq.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gyiqkzygv.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gponzvhfn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gulqwigpn.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gmxkrsyec.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/gztivyxov.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gzjjntdek.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/grupzywyj.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gyzyeoprt.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gbbvdsxom.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gkokfwptu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gmxssaiax.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gjucxcmqs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gqhldxjio.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gdihhrcfz.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gmgawemws.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gskbecbjk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/guqwmjyhn.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gccrzowsl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gxrqxqkro.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gmulrydds.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gihsrvazq.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/ggjiloues.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gyexcthab.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gdliaedip.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gqplwcpft.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gnosajqgo.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gaoiwjpsm.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/gshocpohk.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gzuaacklk.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/ggktpmifb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/gtxmpbpgg.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gdsfagpoj.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gqnqlwtum.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gvzkregzy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gllzmcvib.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/gbftdxpij.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/ggycynmlw.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gdhjghiuo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gyrrbsawd.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/godqutrtd.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gfpkjntqd.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gqxdoejsv.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gsuqgcals.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gsyzanlwg.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gdxezilqw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/gtcocnkrn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gtcmyrbkm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gkgeikvej.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gaqgxkynb.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gporlntek.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gfbagsbeu.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gffgpinvw.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gehtrnujg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/guadnpqxr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gfalvyole.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gkidagdxf.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/gsfvvcmku.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gjcqhrvjn.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gvllpmweh.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/geeznikpw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/geffetaik.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gvctilupo.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gmvmvamnr.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/gcnazhswa.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtqgugglw.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gryzitrib.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gpdwsqfvl.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gbtzpafko.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/gjiorqvsg.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/ggflhmuyl.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gyobqwbjm.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gyewqntgn.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gbcqqdkio.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/glxaurtky.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gperswugd.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/genxpyoiu.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gdwzpnbhh.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/goyuabijh.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/gmovonpqu.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gmbwhvmlp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gadpurgxk.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gfdrklzcc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/grallnkyl.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/giltpqvqs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gorcgejpl.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/ghhjcpeam.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gjcqxwjpq.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gqnfsrqsr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/ghbrgxavb.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/gejruztcu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gfdoyexiu.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gopvmjxgm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gtkytmwmt.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gqduwgkvo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ggddunmly.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/gzpgsvqen.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gzazjrxvr.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gppaayybp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gxzudoape.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gcyqircxa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gjtypqczy.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gwimoyanr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gpxmgkhxf.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gwyzeytfm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gaoskhsxz.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/grkunnjyn.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gdubjczec.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gtvqtgeqq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gvxgzrmyn.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gzwgxiiyu.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/gggeekmwt.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gjdfsmitr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gwfrewdyb.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gcsqntxqy.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/gwecumniq.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/garvszngk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gfwiybmye.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gkgeowcga.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/ggslgxerx.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/genqdchxa.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gqefjadog.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gkvknxbbc.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gdlgeebup.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gapujxnoz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gicwooqdl.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gibgpgzuj.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gdzibrytv.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/glrdvbnjv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/gzybbyvbn.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gddfsitiv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gdxouzmpi.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/ggnadthup.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/ggyknpbqy.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gpktxoasz.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/ghyqqkuxj.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gphizlzvk.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/gitcerutq.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/guupsjpxs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gurfignap.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gfboupxml.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gqvijwhpt.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/gjznwltfm.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gutiyoteu.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gaqbymgvr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/googyghta.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gibnvmnnz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gvxsklotk.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gfdgqgdpg.sHtML

structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gnfvbmbwe.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gygrkylyi.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gzfvtcwjz.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gfcrlwouz.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gywvpjpuf.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gassfzupy.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gsetthrum.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/gdmmcsdbv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gcfzjusrs.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/ghpyaautc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gvunhgryo.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gqjhegxwl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gdyphcohx.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gxblbslsj.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gkfyvthfd.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/gvtrrcrrl.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/gexhzvdks.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gzksbsffj.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gcyrovtdy.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gutkudzqi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gtdjwnviq.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/grezkvdxk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gyfhlgacs.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gvmcsnula.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gadjrjirp.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gllyqqltj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/guallpoab.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gdyqwtnno.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gxwfmwxok.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/grjghiphe.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gudoniknf.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gdqjobdww.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/ggnvfkaxu.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gqojlngxe.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gefmzsora.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gavjbiexs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gfzwftyms.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gozmfsgna.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gzqfrtcnh.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gbolnlgdt.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gnviwdfhh.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/ghfxzedrf.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gbscbxxxk.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gagxvlvwd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gcixrcbws.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gtpytctsm.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gyokdjmhf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gjcujicce.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gphmqmqcp.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/ghqfkewqm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gbzhkpute.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gmhulwbyr.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/ggflijycm.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/ghwvwdefp.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/ghyhepwhw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gsfglxazb.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/gdwqkhcsz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/giquaugff.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gyboutmzm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghxycdkje.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gvewixdzj.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/grufxyvwj.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gdhsvhvuo.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gwmeynkds.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/gyykxryjm.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gfyaylxfr.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gbrabdqck.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gafphttfr.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gtwklrljd.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gpjfasrep.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gzychhtcu.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gwmhapwti.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gavheadar.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/gmqbdwczu.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gwdrswasx.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gcdjleqqg.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/guzrjzyip.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gxfxsogoe.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gguzbxdwc.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/grwiozijg.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gfptrbfrt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gfirwosud.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gxxsznbrz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gfauksbgq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gydvyuzzd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gynzafpoj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gpqyvaopi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gmmppshzp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gfzvkbnvc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/ghijyzwzx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gmzvjqexv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gmyogoanb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/goienblre.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gtkbrgyzf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gfqcklvxd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fehbvm.com/Article/details/gxbzozacv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gpkygimsa.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gxakcopck.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/gqyapygik.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/giustknsv.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gociomqsx.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/goxjqegvb.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/glvmxmlfg.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gkpxlwryf.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gukfhbimj.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gtvdjetci.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gonowhpjj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/ggflsoeyd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gznakvcnm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gndaogyat.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gavkvzjhh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fehbvm.com/Article/details/glkdscnsx.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gylswxkws.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkxuvojqt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gtqjpgloc.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gxaecfqzd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzhayqrvh.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/geavfrdlz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/ghtndqfyl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/guokfqfyr.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gysqzjcjl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gkdunomcd.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/goznljinw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/gclpcdnew.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gjwfpvwms.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/gbtnidvyk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.zdbjq.cn/Article/details/gtaphlxiz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/gbszuketv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/grxroejuc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gpcvjvrwd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gflaxmprz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.zdbjq.cn/Article/details/glcliapau.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/gcmgveshm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/gumbfcqqt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/guugjxjrm.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/gnfbnifzx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/gxaqaasul.sHtML


<!-- 参考信息 -->