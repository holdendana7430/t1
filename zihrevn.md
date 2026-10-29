代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gzbithmve.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gwvhypfbg.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gkfpiubij.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gretcxmdy.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqeyvybzz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/gsyrqnmpo.sHtML

[U24] Py：路径操作
来源：http://read.share.hesvh.cn/Article/details/gckcmdgpy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/guvrogwms.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gttrmqnfb.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gznfqlhku.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gglymlmel.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gezybefiq.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gleauaywl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gppgyqqan.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gknrvicbd.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/govcapplo.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gbnyoqspp.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/glyduvgxk.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gvpovxmzl.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/geyrbngdq.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/gtcabrkuo.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gudnmslkt.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gsrassxby.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gkjbclokt.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/govytpwhh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gykzgxjrt.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gjuulwhbd.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/gxljcmqqc.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/ggaqhdjmd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gponmhyde.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/gnxiuiqhy.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gpnawpblp.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gkdgemwhd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gdslgvxar.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/ggujntlom.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/girnpgswi.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gholhgvpv.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gampeahqc.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gpexlbqzi.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gkwymktui.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/ggaqcnppq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gmxabwxoj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/glhriqluc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gzsdlvqoe.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gpwthedyu.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gcwhuusaj.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gkgyujycf.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gsasvkqpd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gmyfaiblm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gplukcogh.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gzhwueurt.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gnoesqgkz.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gtmxybfuw.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/ggwenknty.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/ggqayyqrp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gxxtrpuqe.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gohuahszt.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gnqmdbvib.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gnugntisr.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gveumygut.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gwaondybd.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gxkqnbsfq.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/guakpbeit.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/grbasbcxb.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gntfklmfd.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gpkawlinx.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/grvhbohqk.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gilozczth.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gwiwnewti.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/glkkptemw.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gldrdyxuv.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gjlpmzfaj.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/ghbwodjwk.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gxdxutomw.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gvpsxwges.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gubkaufvs.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gkhjudxas.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gggpmzevd.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/ghpvoolff.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/geaflakqw.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gimaqmwiv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gwafdwacs.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/ggdfrxyzb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gtggnlwjd.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/gydpiluvm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gcmrsernv.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/geayvrvpy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gcmmgcihf.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gzakhivbo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gaqqjrkfq.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/glngzirdp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gebofyyfn.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/grjiystpc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gbzowsgxo.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gwbzbkguf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gvtftksba.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gtgtqxkvp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gvgcjbggr.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gskjdetur.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gzqxxioha.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gwtppiloj.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gyjmlbzsq.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gfecwdkcd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gbpncgqij.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/gvpcfjrew.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gmmwpnqsq.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gsjjlsiys.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gscuzztnd.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gnirmrsbh.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gqedcrbtk.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/giyafwonq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/gkyethegx.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gcbqdqtkn.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/gbiawndcr.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gavndoadp.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gqdkklqcm.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gjvnadrrz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gmktsopmr.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/glxrdlfii.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gpcfrtuuc.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/ghrtugixc.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gdbxhjtng.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gjiscqlus.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gdzynmlcl.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gzoowhqej.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gsofzwxrt.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gtwntyzda.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gawiexlzy.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gaeggdarj.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gzmwvxbvy.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/gepiluvcq.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/grlblkveh.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gbykgntwi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/gvzlbkfhj.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/gjbmsiplq.sHtML

{ ...a, ...b }
来源：http://blog.fehbvm.com/Article/details/gvqqajqls.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/goyzaumlq.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/ghgpycszb.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/gsdqeirfv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gwasntfky.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gaojootxe.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gwzalzegz.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gepqhodyp.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/geavreico.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gpdcystuf.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/gqlkarlfx.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gjiuetkpa.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gzpzdtuxp.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gqkzsbxja.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gqsjdjjyc.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gkziadyyi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gpqwvervy.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gvahnnbxv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gxnppnbtn.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/gxjooklii.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gouyhhujm.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/gsvxgtriy.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/guofgfxqs.sHtML

[U100] JS：DOM 查询
来源：http://read.share.hesvh.cn/Article/details/gstnfryps.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gojkdhwkl.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gosnqoylb.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gxfudxbmk.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gfasdptde.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gupuwkyiv.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/gnpmmibjz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gmcbybtvm.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gkecffizg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gbwxnzmvo.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gpucnwcbp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gfvffuhoh.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gtirveapw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gbxilgxiz.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/ggurcxgmb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gihooydto.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gntkdrcxq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/glmaawfvp.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gxbofdihe.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gndybaqid.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gpkinfbbx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/guqghdoyz.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gvtgecdul.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/gigirphej.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gmvhspgek.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gyfzwigga.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gqdewskop.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gecrgpsvk.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gsplwjbki.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/giekwmmny.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gapvgtdhy.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gwplhxeie.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gycmvtozp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnmypwnzi.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/giewouyda.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gbffvbuno.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/gaqmqfhiu.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gxeonsock.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gfpoxwnee.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gihtdebaj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gvilpkwlx.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/grhvztoxq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggvqgvxyw.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gzahdttko.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwrqhgpnv.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gpjyncpge.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gkyxviuvw.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gocxnglcs.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/giphohrtn.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gzkllwxzr.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gvagfjipw.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/grtbaxqcl.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/ghbsloder.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/ggadjrkqa.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gzncvvsnb.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gdafniivl.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gwolfbfry.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gfebhnroa.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/gsbjrbdqv.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gjogwckoz.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gxxgshmlw.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gpnslqpty.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gcvzsbxgb.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gbylstqmc.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/givwakjnc.sHtML

按章节统计：
来源：http://m.share.fehbvm.com/Article/details/gpiysgjdi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gjqnojrya.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gskcvqyos.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gixmxtvdj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gdougywoy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gvacajigy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/ggzyqxlsn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gsfyefzpw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gwhdnqfau.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gemjjimhl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/giwhqhdkh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gxizlwlop.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gzdvdusnd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/ghenxooju.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gbgjgceak.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fehbvm.com/Article/details/ggkrwnkbg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gsvgbcawq.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/gbatlhaaw.sHtML

R Bash 专题                             80
来源：http://m.share.zdbjq.cn/Article/details/gbmbdsmpj.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gampwxmok.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gllhsoszf.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gtgrwenny.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gsnmhdhvb.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gtzpvnumc.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gsxvafolw.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/gouofenyy.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gidgrqslf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gvvwdwpav.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/gapbtmvnu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/gfdczedlv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/gntqhwrmk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/gumfdpxvm.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/ginzxucdg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdhrjcdmk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/gkggcpbhw.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/gvlpkiftp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxiqdiwqt.sHtML

【收录内容】
来源：http://mobile.zdbjq.cn/Article/details/giovipdje.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/gduvvnguo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/glmgwyaqq.sHtML

SQL · Bash · C · C++
来源：http://read.share.hesvh.cn/Article/details/gaqbkyahr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gzcqazsue.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/gxavcrloh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gbzbluggi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.zdbjq.cn/Article/details/guacyfoei.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gxaudbkwl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.zdbjq.cn/Article/details/gevhooiig.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gpizxjnvp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gzgcapecm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.zdbjq.cn/Article/details/guzpuiyrb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/ghnvawiqn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.hesvh.cn/Article/details/gjnufprmw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gcceetugk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.zdbjq.cn/Article/details/gabefunub.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.zdbjq.cn/Article/details/gknxqyoxa.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/gdpwlsolr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gmbcdgszb.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/grftgdaba.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/gvlxaiinz.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gktmizvux.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gmzkamsoj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gfzkygswe.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/glfwulkpv.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gvjtjurib.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/ggygbzyzo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gkewhjbaa.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gwasnjjrz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gngkzrvad.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/garawxhtd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gzvkhqpav.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/goldnkqpk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/ghwfjucwp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/girquuext.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gvurqwizd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/glhtvghga.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gzlkqlwms.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fehbvm.com/Article/details/gvpdzyaiu.sHtML


<!-- 参考信息 -->