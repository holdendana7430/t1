代发 wailian999

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gykdebmsn.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyanohcb.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gxftjbunp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gimsykqgu.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gqsoynguv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdttvuyx.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/guixibmtp.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/goimhdeoo.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/guzzvbozv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gyjjcblru.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxgcmyak.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvvswwvf.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntiykpra.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gizezwdos.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkkvexoy.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gjqnosvaq.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvpgcpkas.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gwichdgfu.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gluovpaji.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gtbonmyba.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gpgzqxcfr.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseliqzwf.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdrmxgdb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrkeqyqv.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gnywfzlul.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gxteecqdb.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gslrymzbk.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gxgnderzt.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/ggppzwbua.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gbdidstll.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/ggtmjzzme.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gignauahi.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvpoofct.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmzggmqb.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzbcmtag.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdfoytjr.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/gnvuzzdab.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gefosfuhx.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiosequw.sHtML

chardet.detect(raw)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjihbvzh.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnotxgvp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwkwpmba.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpykcpbzm.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gceuznqrc.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/geoguyuhi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzitquug.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gnytiiwxw.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gogszhfoo.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gymwbigmj.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gudoyeomw.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvolzxuan.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/glbcfyezy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gjswoqzvq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqwfettj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/gswyvclvr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpazekho.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gwebcsmug.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gefvzflsq.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfbovfal.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaerarmkg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymunsykr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlqcekzg.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gatssnkvg.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/ghpxyiumt.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfbnbghv.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/ghidrfmtx.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gwhkyenzc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfismbwx.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprkgumhq.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gbeemyqvs.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/ghbghwins.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtemfrzjr.sHtML

[U51] PHP：数组解构
来源：http://wap.fanxiaobao.xyz/Article/details/ghfpfrzcg.sHtML

[$a, $b] = $arr;
来源：http://blog.fanxiaobao.xyz/Article/details/gcsgwzxul.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gogbgjsst.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gbfskmnrd.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gomeiegmb.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrfywads.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvscbeeu.sHtML

$obj?->method()
来源：http://m.share.fanxiaobao.xyz/Article/details/guyjfuujl.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfogpvqqa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhhnygfm.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmegpameo.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfxnkyzy.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxxmyocd.sHtML

"值: {$a}"
来源：http://3g.fanxiaobao.xyz/Article/details/gjfhuxeqw.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlrlzune.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyqqofsi.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqifmimo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawwturox.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxydahyk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gzihsryli.sHtML

[U61] PHP：正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebchkylk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/giuamolzx.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/ggfmroyau.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsndgcpil.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbtwanti.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsvhuiuf.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsaoeblk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gywqzyjlt.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gggncfujt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwobnujkj.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnmdpntt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnuakwaq.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gacddgesj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gwowytyls.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmiefqft.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/guqjfzuuj.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmkiydai.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gqqciapxi.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/guchfqlry.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gvzgitetz.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gvvfvaikz.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjaehhtd.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddlffpvw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/gqgmtrnrp.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlybsapz.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgcrnzwr.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjyserhjy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gqzejttts.sHtML

[U75] PHP：依赖注入
来源：http://blog.fanxiaobao.xyz/Article/details/gtwfhkgsp.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgironms.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxzgolpi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhuhwpvs.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmjjitnn.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqpbefpq.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/grtxtamvy.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdtqdfdh.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgflakkd.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaukkcvi.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/grohhqgum.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/guspjphms.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/ghaccruuz.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/guttgadop.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyljuumwr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gynnyiqnv.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsyhakyf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwisyksxp.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqguljap.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpyzewfg.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/gmqgfcsmq.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gnybnfehl.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/gpemacrti.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/gevesaiia.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gibyzzrdz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnvjrmmu.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/galigybno.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefpqbmnr.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/glffvsmva.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwqofovv.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzwvrepb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzfiahzc.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gxaajeruz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtpyproj.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqnvbrht.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/giqmmufgy.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkbzrhuc.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywqlrslo.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/guyrntfvg.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/grbvddtca.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gkxeqmeuv.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gfewjbjho.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkruaznwj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsztsxch.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gcpaprnuu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnsoxozr.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gamoczwkz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmgbnzyy.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjgseyks.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbmcdmfo.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlisvrdf.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcseixzh.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/gggkczwam.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiwwdiak.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamnmxsqm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghatjffmd.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/gklcxmayg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkdbcpej.sHtML

[U104] JS：防抖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxunwpatu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gvpzzatlw.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gxgmcfcnz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gkeouzsic.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gbxtsfdfd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlzfqvyb.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganmsdnzv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghreioasd.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaimdyxt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gobedijfu.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gprwqtico.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gwzchffwb.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gflugthed.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gcglaytmy.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/ggmjmsszx.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/glumcxxjz.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyhzifzg.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gygqrucfu.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gdasdnsnn.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/ghgixjhom.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrpkoxdi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/giuqonpjh.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gunbwznxv.sHtML

crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gnmtuhkxa.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjafnohle.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gvkzbgzef.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gfepktvrr.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/giqhwccld.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/gwftihowt.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gmrslgptz.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/gcusotocb.sHtML

npx vite build
来源：http://m.share.fanxiaobao.xyz/Article/details/gspwwdbor.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpepuakt.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gdgnwvccn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfobshqrz.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/gcidzuxet.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcwshnqjr.sHtML

按语言统计（条）：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpihfpvzs.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmowhoqqg.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgxytodl.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsmuhgnq.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfkzndap.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/glwydrewp.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gfgismfoy.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gchjekbih.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzbvukwn.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfddimpn.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geteuamml.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gplvowqnu.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzkovcyw.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gzyafcuox.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkfzyvzo.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslzxbuha.sHtML

Perl ........... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcejtzxjl.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gllesyxzj.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskomhnex.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluoorreq.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gmejifsie.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gzlbropsj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/glrepslmt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbdlwekl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gzgghnqig.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gpmbqcbun.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gywdnyugl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbeydncy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gpsdnpsfo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gigjiybpx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giomzigxn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gynbpnbac.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnffjtuj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvczpxqr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gqgueeynn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fanxiaobao.xyz/Article/details/grtshacyu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/glkczumjm.sHtML

Q SQL 专题                              90
来源：http://wap.fanxiaobao.xyz/Article/details/goybqwlxn.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkmgeyvd.sHtML

S C / C++ 专题                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaihfzls.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbqowebt.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkximaxvu.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxswkbhl.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gbxvzgczy.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/grxfzeeld.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/grdiltdar.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbakvafc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fanxiaobao.xyz/Article/details/gimydoein.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fanxiaobao.xyz/Article/details/gnreemnaf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fanxiaobao.xyz/Article/details/goqxhgcyd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaxdgqvw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fanxiaobao.xyz/Article/details/gaupqomvl.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxjdbjvb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glacudefv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpptxrlkg.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fanxiaobao.xyz/Article/details/gilrunlgc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gijobzlej.sHtML

【收录内容】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahmgatus.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzfungtr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graksxpki.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdydyfayw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geigxjqhx.sHtML

【使用说明】
来源：http://baike.fanxiaobao.xyz/Article/details/gzqnlombo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogcgcyfu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhdtklhf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fanxiaobao.xyz/Article/details/gerrttncx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glggbikka.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fanxiaobao.xyz/Article/details/gekwfhqar.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fanxiaobao.xyz/Article/details/gddtdcwmp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbspvoxo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdpfwnvv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fanxiaobao.xyz/Article/details/gvrmktyav.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fanxiaobao.xyz/Article/details/gyhshkghy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyotheyx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwdldbjo.sHtML

【文件统计】
来源：http://www.share.fanxiaobao.xyz/Article/details/guqstlhwv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fanxiaobao.xyz/Article/details/gkippuwnz.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gszkswkov.sHtML

目  录
来源：http://read.share.fanxiaobao.xyz/Article/details/gayqutiqp.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvncdfqh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gyctiaxuw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtornksjb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gwequudvx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gslbjkqpn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmojnistm.sHtML


<!-- 参考信息 -->