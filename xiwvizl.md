代发 wailian999

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gjzoytquz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtfnbnws.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzhgvvef.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfeuegok.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gzetnllnc.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjndvsxfh.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkeppelp.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnqrmsia.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrohohlm.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxflnltu.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/glpnxurqw.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbgewcyc.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gzhoibobk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmxpmrvk.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gdkgyrobd.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmeisqwz.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhiydzbe.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkctclzsm.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavvdygvc.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyipmesb.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/ggthdhnfz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/gjbyynneo.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/ggjmfaqgh.sHtML

Path(__file__).resolve().parent
来源：http://3g.fanxiaobao.xyz/Article/details/gnyfpkljh.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/goxahcawa.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyexhnbj.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gfuojxqmw.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibkxxwfz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gysrcvico.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjgzfmtt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gbbkauels.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gculxktem.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsckjafw.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gburmzmyi.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gmztmfznp.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/glcgzlngr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gshuyruuo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcpswkck.sHtML

[U46] PHP：可空类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gleqqajbf.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/govspszgg.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/gvebdfibi.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/gehyouwnb.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkkepvsz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlwksscr.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmwrilwz.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/glagzpjtw.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqffopord.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/grmhziziv.sHtML

[U51] PHP：数组解构
来源：http://wap.fanxiaobao.xyz/Article/details/gcfxqicvs.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbuubeis.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/glqistosl.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/grncqrxmy.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/grbtdthni.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fanxiaobao.xyz/Article/details/gehmfxaaj.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhrmigwv.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzidlyued.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gpshrxmnr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbepdpqxw.sHtML

[U56] PHP：命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/gggigfuwp.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymcvhhnz.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gyygakzxq.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/goaluntpb.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyehmxcmn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzxesipg.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gbmyufxnz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gsqgoqjcn.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxenwxqqu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/glpvgrggc.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyvbxxoj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoiipaey.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/gnepfyple.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/gkyvqywfu.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/gtkviwbqt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/gznaohfue.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/giqihlttt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/gzqkokmhk.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gnooticby.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaquuxpxw.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fanxiaobao.xyz/Article/details/gwjqqaoky.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghfawzzi.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvplchkxm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxclgmhqi.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/gpmawwido.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/glldnkjva.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/gsrmuauid.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkramlrf.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gitqaphha.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/ggaepuwzy.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/goifciequ.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gyehibyja.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gsthqjlmv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgbyzubn.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxzkfycp.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gucouphqj.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/grbbouzhg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gftdnsaez.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnnulsvn.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/gddinyohk.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gqprbeiwl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gwfuucdog.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/gemjdesww.sHtML

composer require twig/twig
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvrrrkjx.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyndaqxon.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fanxiaobao.xyz/Article/details/gexthmgag.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxhcpnuc.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gwdrdawws.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gbermhmkz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fanxiaobao.xyz/Article/details/gqeocjjwo.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccquyhvm.sHtML

npm init -y;  npm i express
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgjpibkt.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gqpirjkpq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngsafhxv.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/gdybezrsh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/gshgyqroh.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/grgzimjnk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbktygtc.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/gaiocofjn.sHtML

a?.b?.c
来源：http://mobile.fanxiaobao.xyz/Article/details/gujuzlkdc.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/gppphyanf.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgviwzgm.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbwkuoem.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmifkamzl.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujpygyho.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/giskzspog.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/grxvslxyf.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/guncnrbuv.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvhjzpzp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgnynlxl.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyugmkto.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/glylmzthe.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntxcakvc.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gdgpfddkx.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuhyatyr.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/gftoqbodz.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdsrgmfk.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqzymgoi.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoijnpfo.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gocwsldou.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gmlqxjtet.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gilpqgykp.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/gdwmrvxnx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtiwdttl.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtzcznia.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fanxiaobao.xyz/Article/details/gkwxojpwo.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gskfmqths.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/girnebaem.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gthgksjdg.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnseydhet.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/giuubfqsf.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcolzyfbw.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gximuzxzs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gzdqsnphm.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gkxhssybn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/gxdcatejv.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gydtugxgz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnhqignc.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/ggmhwwkqo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvejhanad.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gshlthpdi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuacpjyr.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/goikxiiss.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/gmtydfnma.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/glujmggbn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/gvihfydgc.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gkefjilcf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyurhdsia.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/glubykjrq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gcbmizcss.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gnpjpbzyi.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gnadbhffv.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerxrhmoe.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/ghrlzksdt.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gbdaotask.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrqfjajt.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzsrjckl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbimciqc.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gjwswcupj.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/geygtjcvp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjtldnps.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgkromyx.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gnljzfcmy.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gvbnegcdp.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/gkctifcmn.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/glcrwtdur.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqzzzwmd.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitpgcopz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmczpesxb.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gxwktbolj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqtjbfpxo.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/genknaxon.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggdijznof.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gyetnsbel.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/glblphdla.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtnyrxoe.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnubjxuzu.sHtML

TypeScript ..... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/golthrmsp.sHtML

Java ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmyehvwd.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhpfjdng.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gsiveljbc.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gyxlyvdoa.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gczylcekd.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/ghstzmkoa.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxgjjbrn.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gpwwhlxew.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/guhguwsir.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbfzjkbo.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggafisnzp.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gspbtwfgo.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/grmvqxspe.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gqjlbghsc.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gvsmnorna.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/gpawisdsw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gwhwncirw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gxxqixnpa.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/guuaexxir.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gojzzehmd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcfnbnzt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbycfqbu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gcaeepeod.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcjiaacx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/grfpsidfl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gyieioqww.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgzpcltm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqfnmjuu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gzijziykx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gkiweanbn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfiqrmhx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/giybicffs.sHtML

Q SQL 专题                              90
来源：http://m.share.fanxiaobao.xyz/Article/details/glhnqkwrk.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/gykonjlbt.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmdiesfd.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzzakxkc.sHtML

U 高频实用片段                         120
来源：http://3g.fanxiaobao.xyz/Article/details/gzukxgeio.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbypmkfxu.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxbfgwby.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gtepdkjbd.sHtML

使用提醒
来源：http://3g.fanxiaobao.xyz/Article/details/gakttykqf.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/goemmhhah.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fanxiaobao.xyz/Article/details/gzctutocm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvncbktj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsicnxie.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpwqlimw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fanxiaobao.xyz/Article/details/gzatorlcs.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjrtzycz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtsrhljm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fanxiaobao.xyz/Article/details/gqicrnlxs.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fanxiaobao.xyz/Article/details/gqwtvueru.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gztmyhglh.sHtML

【收录内容】
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkjycqhl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fanxiaobao.xyz/Article/details/glstphqhl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fanxiaobao.xyz/Article/details/gszyvascy.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/ggejmpzgf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfevhrogo.sHtML

【使用说明】
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqvplomj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzvgraaz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjrzzdsu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fanxiaobao.xyz/Article/details/gtukzpuzh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fanxiaobao.xyz/Article/details/gfouuljwy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrolfptc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fanxiaobao.xyz/Article/details/gptmregkf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fanxiaobao.xyz/Article/details/gyvthjymx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhidhxfl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fanxiaobao.xyz/Article/details/guolyxohn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrvunkhe.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gogegyhbk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gecsrnoxq.sHtML

【文件统计】
来源：http://3g.fanxiaobao.xyz/Article/details/gmdjkysrw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fanxiaobao.xyz/Article/details/grezenvnp.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/glkqylqqd.sHtML

目  录
来源：http://blog.fanxiaobao.xyz/Article/details/geylimdle.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gazbuizmh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnypuqvtx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhfsrwdm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjwkrpwc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gujlmdiqu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gujbpbgdr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcezpeksx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhbxuuca.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzbsmxxo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gdyhmfcfh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/goxwfvusv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gvhdutvyr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gmxuyoilp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcgrqzfr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gpserddgf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gybbircyf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyjwtxxk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fanxiaobao.xyz/Article/details/ggwphsslp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbatfwuyn.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gfkagyjgm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goidakeqd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gupsmwsir.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzaiqteyi.sHtML

A. 基础语法与类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gohybwatd.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdzjrtum.sHtML

[A01] Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvsekjco.sHtML

Py:   print("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/gxlcfstpj.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fanxiaobao.xyz/Article/details/grqgtgndi.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gjjcuaxbx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fanxiaobao.xyz/Article/details/gbjhqmfeb.sHtML


<!-- 参考信息 -->