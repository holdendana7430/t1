代发 wailian999

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gqdtmrsag.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gswroubcv.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gupulidyp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gyanxrney.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gkgnbcwdw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gghfshauz.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/goxkseuso.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/ggopfcaiu.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gtohbaruk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/glgjqzzku.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/gyisixlyy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gltamgytk.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gzcfdczlc.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gkjpytfsq.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gbjmwbwbl.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/guetqlcye.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/gbytzudwg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gprqytxbj.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gyxnwowxe.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gunormpst.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gxpqhkaxs.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gvblstxcw.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/glfvvvsou.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gjkofhaao.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gcaqqokta.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/grankdste.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gjwksiutm.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gncqofdja.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/grjfdgrqv.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gmzqvmlte.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gpxjayvae.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/geweckbud.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gsjsxqrrk.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gjzwuyack.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/gfcazzaab.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gxupjnbsw.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gbbanrdjs.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/grdwwzyzc.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gkutirywc.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/ggntsgxfk.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/garlpzfuo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gycojkmkm.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gmjoemeiv.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gfygrbwgu.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gdhdtpger.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/guihtajdl.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gzhexgfpj.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gkqczvunn.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gixcadteq.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/geelyyyjz.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gjvaygpoi.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gxosgvjll.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gkjwxoamr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gahwgycpn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gfaohlexz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gsskaxnen.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gvlfxduen.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/gmplqyvbt.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/gcrkxhlpd.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gcyzrkrbm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gbtxxsvkr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gfmgztjro.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/ghxmmqaxz.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gksikeopt.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gtqixihex.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gwuceykci.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gtdioqurf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/ghezpmjwa.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gwjzpyohi.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gvaoequtc.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/gjzcafofq.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/ggoschshz.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gxhyzrjih.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gmknjqthe.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gprgmleau.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gnaxvsqjq.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gkxyezrof.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gbxfqkxmt.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/guasiflon.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/grlxmhwla.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/ghepduanz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gbybsgogq.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/ghvpkigcd.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gwohqjnag.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/ghjblcitn.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gzquouihj.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gtcicuoyk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gmwafznlf.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gnbrmnmwd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gxtzdvkum.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gbowvqjju.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/goaliixaa.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gkevasljc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gqhsnmszp.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gwdbnnfda.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gbpqimgov.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gtxielfwd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gdzzdggba.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/ghoefczwl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/gqmoakdnn.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gpytvlulu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gplgmabum.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gezvwxfxl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gnnxzcsdm.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gwojjedkn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/grxwdmoud.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gyfcmspxh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gsvvnfqkx.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/gngvjwazf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gugzfdsop.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/guntexyxp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gkdrxjumx.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gjmnyigbv.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/gbwfyeosw.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gjtgrnewj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gbaoegwbq.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gvqbbhcjp.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/gzmhstbxc.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gvindutqx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gaborpynl.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gmmmwxejm.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/gnsccxksh.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gquojrmra.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gqgaxfbof.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/guujezizg.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/gjrtedznl.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gnefxbebz.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gkgubiyxu.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/gascobonj.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gjdibgzlf.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gbsghtldq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gzpytwedw.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gszehlkcq.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/gublymdpv.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/grxsbnpmp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/ghisitmzq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/ggtshjtjd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gfvpwqftq.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gukhqpbum.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/ghspqmzdx.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gpvpykkur.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gyzvrthnf.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gosnhevku.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/grdixubat.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gdxiuycgm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gqulmqwmf.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gpydjczfp.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gzhlicxev.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gitfiocyh.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gobpjhzac.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/gkrbrchbo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gbjdywtqy.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gbmzgxvwi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/glhstadkb.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/gdfvwwtln.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gxwlhbodz.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gakjwftxz.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gyjipoofn.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gedcvbqyt.sHtML

const double = x => x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gswkbeowz.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gzbjfvkne.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gynjrwtmn.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gxlymamjx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gmjemgzwa.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/gyopnkqsb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/ghxnueqsa.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/gcvjmskuf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/ggvfktnqr.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gnkdvgwhg.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gcbsmpycp.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gspqmemvu.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gifiijxan.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gxuiqnjux.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gntpxlurh.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gcdsuavtk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gqoklxwok.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/ggdwsdmgt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gmeyapcqb.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gboiyiuhc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gikqxfhng.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gxrngjcff.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/guycqcaox.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gegduxdxc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gyadpapfd.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gwgsxrvqn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/germxsega.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/ghidugtnt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gicfbifyu.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/ghllcxtzm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gmqluxjbk.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gtmjovbae.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gbwzggqvw.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gqxikfikl.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gsoocauap.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/geblygqcp.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gwxotjazs.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gkbeodcuy.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gvqmvypts.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/gxjdwsiye.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gteqsatrg.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gnswqnriw.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gvxopnmcg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gawujbkki.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gywrvmzhu.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gtucjzivg.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gnmewgzng.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gwypihhlh.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/ghttcjhet.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gfwgczclr.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gqacokjbh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/godtigrlk.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gmqyajnrj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghmlycpdm.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gqmpyenzw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggevimldp.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gnsokwpzq.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/glpuwfwdq.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/gktiichnf.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gbpbeeisn.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gmwmlnzay.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/ghydnwico.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/gtggbhtcq.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gjtzftbux.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/guiultguv.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/gavdwsjdc.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gqdnpfhoi.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gtzmwjzcc.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gbnbwfbin.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/ggdekmxsi.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gstfbrifo.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gmwoyqxok.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gorktyezo.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/grcjbyhwo.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gxettqrsp.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gfkqdoekm.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/glmaqmszy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gihhyulsg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/glfyronkx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gqxpzmxlj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gjyvyurpv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/gdcepdbcw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gdyhmcvft.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gnhaxzbfd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/goiitcaen.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gfpjpfend.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gchzhxwix.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/ghpmtdfku.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gvgfcjkis.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gwgdhfdgq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gjiqnpjmi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gpvsofzfw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gixefbhfd.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/gcvlixjdy.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gspmzrhur.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gtzijbgzc.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gpmcwzqnj.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/geyazrgim.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/grfgtcfas.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/gylndjqsw.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gkntameou.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/gzoikgxee.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gbwkiasdg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/garasgpnj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gkkkyxklr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gkzktalhl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gjfrdqaxy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gwrujqazu.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gklyvcwlh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbomnqare.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/gdffxwdxw.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gvgsychlu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfptxsdhn.sHtML

【收录内容】
来源：http://mobile.fehbvm.com/Article/details/gippyxsbu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gzrvxdppc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fehbvm.com/Article/details/grgpxcewe.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/gsgjtvbhc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/gikzqpalp.sHtML

【使用说明】
来源：http://www.blog.zdbjq.cn/Article/details/ghmnfcxcm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gpzyjldqb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/gmrdoudau.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/gooqppymu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/gxtfrrdgp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/gwczklxxa.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/gnxdzznfk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/gscnptdgt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.zdbjq.cn/Article/details/giwyjwhrb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/ggjqhkwgc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gmqculjou.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fehbvm.com/Article/details/gjmfpqdvd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/gvyzwacji.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/gxmhjxouy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/gmepszbcu.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gomrbpdqg.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/gaugbnegn.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gknbtmcmn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gczeaxvpi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gkxcbtnjw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/ghunwpmrr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gwtocopji.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/goaeidkiv.sHtML


<!-- 参考信息 -->