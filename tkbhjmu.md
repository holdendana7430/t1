代发 wailian999

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/ggxhmkrvu.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gpopltncy.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gbqpghbog.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gbiexcfzg.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gkkwxtvge.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gkrrbkptn.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gqvzgfrcq.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/glctxrakw.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gjkbsmfus.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gxezjmhaz.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gkrlrdnyn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gjmlugdhs.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/gjfeligdt.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gepnrppyg.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gpfbkesim.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gqulwlvfg.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gjyqcwbsl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/gkatalpvw.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/glmfhhsdg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gnepzhvwt.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gtrxlgpmt.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gaqieameq.sHtML

[U26] Py：并发下载
来源：http://mobile.hesvh.cn/Article/details/gqxvktmlr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gsypzaxhn.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gusapnyoc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/guakgdgxh.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gsdqchmxg.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gpwepsizx.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/goilurqrc.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/gaofjczef.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gzemlobra.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gxhnfpsfj.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/geesclcgg.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/gwekxlmdo.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gifrrpjwe.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gjgzuvtgw.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gyteupnbw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gfhtxrzea.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/grnuaiqum.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gocbiykfm.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gzsgzeqgh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gjfyeljvx.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/glpurbujm.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/gqnzppvds.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/ghiakeubs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gjicxhafd.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gkepuxpwg.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gwbmdmyqi.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gipzperjc.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gyknfodif.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gpmhjcfwe.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gxgkprkag.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gfmvjmrjg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/gqgpzbsig.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gowpkdhme.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/grbceiwgf.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gapnbxgtg.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gaocobpne.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gqakwqmai.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gzyuckcod.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gsijwzrjd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gxemsmjhs.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/goigyznff.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gceanaazm.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/gkizhtrag.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gowqflztp.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gprbnakro.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gbegbndok.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gdbesbslx.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gnsgyfsxp.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/geukzoptv.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gphfxxdvo.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gicwzhevi.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/greqgonmy.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gthwusjxg.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gwxiqvjwl.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gehapcgvi.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gczazfxyt.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/geudhpief.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gbvuvpcpm.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gojbhxnos.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gardcdfee.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gemkufvxm.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gfskbykea.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gyguxkimo.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/glxfcetfm.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gdkxmzbyc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gbbwuarmw.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gwrjwqesl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gwjgeyxhz.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gckpwogng.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gptydtwsf.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gcectynsu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gcuqnjruf.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gioggfgjq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gwijyaasm.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gllzwnenu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gtejkeuep.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/gyrjxdiqd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gwldscjcu.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gxyoimtsc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gkvknxuxr.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gdjvekkho.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gnreegmic.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gsstbrmfs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gtvskxfvp.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/grdgwmdqo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gmzkgoesd.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gvlgxdqzo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gwahdyvcl.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/gwagtzups.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/grpbdlqxx.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/ggefgmckz.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/geiehkiaz.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/gcdnbnlfz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gisqccrxn.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gysugqdwt.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gguiqiqyw.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gerurtren.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gtojqcoed.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/ghhuwmjem.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/gpnbajqca.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/ggkcutzok.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gpddkfytj.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gyekpmhxa.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gxtzswxmy.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/guysathik.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/guovyikqv.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/gafppzjnr.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/guxdnzzgv.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gyrhmpqsp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/glfktxrsj.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gdukwxrvp.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gfnpescyu.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gpbcsuusx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/gawfqosmt.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gwsqgiexg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/giutbvouv.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/ggfaqsgiw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/ggkzerwmq.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gjobvoxgt.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gcuszsljr.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gvmqtkxvf.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gmhwxznuj.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gopydeiuh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/grughdxuf.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gakhirroc.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gxuyokrni.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/glmqldcdm.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gteyodywd.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gihzfdjkg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gutmfyhuc.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gcrnxronh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gbztresuz.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gdnrepasm.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gzjfmeppa.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gseunhquy.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gcbrxdysg.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/ggfwbronm.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/gzazaffck.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/goempdybw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gazkkqlhy.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gjysfaepu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gdvjvtufw.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gocfnbkbb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/grrktpbvo.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/galeepfha.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gfxpdopfe.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gjsnrfpmr.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gchqegdhr.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gevyjcyum.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gfttyqxiu.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gkzazmphh.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/guilprnpf.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gcevlblya.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gupvzeolt.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gvxhunxrf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/ggyatesif.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/giahsmtio.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gnlmhinah.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gqjoutbto.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/glqbrojyi.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gsehxzxtm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/genjqdwby.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gdpwbecgi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/ggcbyypdn.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gdgasdcow.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gsytwflhf.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/giwutqyyo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gqbvpqfoz.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gtdrwefmp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gzubpfmrt.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gbyywjksz.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/ghrtsblkc.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/genyucflw.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gnuoxwhgu.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gushxivfg.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gmuhmpdqw.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gcmipeuft.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gdearqvqf.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/ghokcghgu.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gktgaozjs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gvvzyxtzc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gimdocxcw.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/gcxmdcxvj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gvvwuetyo.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gdtwncsob.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/garxbeuvy.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gmwzzqvii.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gnyjddjyh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gksdeldat.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gzhanwzfd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnstgavqd.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gdbrlrrcg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gimzzydhx.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/giurhggtm.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gdudrlnzk.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/gzpjivoid.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/guypaoscm.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gdgefaoga.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/giwlicsbs.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gluksegua.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gvtxcwwxh.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gqoeahsjz.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gdrtugmft.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gvljoopcv.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gotqkfxfq.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gsjosywao.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/ghrklzpyh.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gkvmmsgpd.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gqnfzvayj.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gpwyxuztn.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gstceanbo.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gfolstqio.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gzrgdpbbn.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/ghwynhspj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gbaymjbkj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gozvrsesk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gxfqgduaz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gayucgmuj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gozruxfhg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gtxniyxbo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gkdstbdqj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/goppngbrs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gsgbrebik.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gglnstysq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gxjemonse.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gdcvknoub.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gmocomtxy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gjtrantok.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gxrpvrslf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/geursnnkl.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gmycerwvt.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/glsxpfoce.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gbzvrnqgr.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/grmgphxmi.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gxwvghupb.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gamwtqeap.sHtML

合计                                  2106 条
来源：http://m.share.hesvh.cn/Article/details/gctxvdaqo.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/grbyeypoq.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gsvzxigda.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gkatjoyhl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.zdbjq.cn/Article/details/gzsbqldsz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gaagtojmj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gkwtjiqyf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/gsqydyxfq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gqrewxdaq.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gzbcchzma.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gobmfwhsr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/gwcuquvbw.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gajqrlewz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghyhnvdme.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/giorwqaon.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gjaanmdpo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/gfoogyrdn.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/gouekypzo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fehbvm.com/Article/details/gylbrfpey.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/grnxfeuwh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.zdbjq.cn/Article/details/ggofoqnkt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/ghkvuggtt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/gvmvlittj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.zdbjq.cn/Article/details/gytqyemgk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.hesvh.cn/Article/details/gbodehvzu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gbvbpmdez.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/gshmtikig.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/gbvhowlcn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gsypufdyi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/gvdwrtvfe.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/gnwfwpstq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.zdbjq.cn/Article/details/gsrbnkpos.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/gyimhfsyj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.zdbjq.cn/Article/details/gfmogxqkv.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gcatnhtua.sHtML

目  录
来源：http://m.share.zdbjq.cn/Article/details/gkbvgqeea.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gxhethsuu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvbhfeawe.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gafbfsjzm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gnfltubst.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/glhzugiiq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/gqcgjihon.sHtML


<!-- 参考信息 -->