代发 wailian999

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/ghubgfmqq.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsjgovrh.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/ghvcykltw.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysrjmull.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkioxevm.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxpuoejo.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgtllqck.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/grnzocmbp.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gutkntdvp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgiwtaol.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/gpuhbevtm.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/grjjsyrif.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeaxkrke.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/geleptguh.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/ghmvmcwff.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/gmdyflerx.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gbtxbfvxz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhqjbado.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/gihgrbfxg.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/glsjdxfui.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbazxrlkj.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjurbvpym.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjnwerqj.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgzscdll.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gptpxamje.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrwsreut.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwmplqqo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlqdywxy.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gapabivwe.sHtML

namespace App\Http;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrldpjho.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtzgqgdc.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggztyyody.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gaygxjrzu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyolmjxs.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/grvzakpiq.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gwagzlijp.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/gpfsyacgu.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gqldfugdw.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gysmslvyg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxmasihp.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gnilcvodb.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/glfodualk.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaujuino.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gxonsolpg.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gcluqliaj.sHtML

[$a, $b] = $arr;
来源：http://blog.fanxiaobao.xyz/Article/details/gtgngaswa.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwroeictf.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkkynyyi.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdrkgobs.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvzcwedf.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmgoypak.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gprtdksor.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/glksgjeeu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gtkoxjlqs.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgbbnorl.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmodfwboh.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gjaojildp.sHtML

"值: {$a}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcilwhba.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsrgiszk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzovalgxp.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gmihwysrh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/goqqpjezu.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvliamypq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazunkxju.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/ghfivmpez.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjgqcovy.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrcwmphz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/gvvtbinwy.sHtML

[U63] PHP：文件读写
来源：http://blog.fanxiaobao.xyz/Article/details/gorhawyen.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdbnwdvs.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/greqfpodz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxwanzka.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/goojgmvbf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gtymtkmdv.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/gcpbqfpul.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/ghudpoccf.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnvvjvzl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxjeehds.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fanxiaobao.xyz/Article/details/godzjjvhz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxndtpyv.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjrumzfr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyypknwk.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwiplfhb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/gweiwzvme.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gndnpffmj.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gktzqqgao.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwmueogq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gifalpjkz.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgnlzblw.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjndxnaiq.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcqkjmdf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsferjmxd.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/gcoqyhntv.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gboghgxcr.sHtML

[U76] PHP：简单路由
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcsrlwvu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdybeivm.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gbydckasy.sHtML

composer require twig/twig
来源：http://wap.fanxiaobao.xyz/Article/details/giorvfxfg.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gcllnwgwz.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcupwhiky.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstvalkom.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/gyultvpyi.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdgpnuxa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gzunkoumd.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gekekards.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdopcdfu.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/gdatahrjd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/grcrspztr.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/gddynnhkw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/goasujobk.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gorxibbht.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gdazutphi.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/gzkoddaci.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gduswedtp.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/gbywjwsxm.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/gcljbivtx.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/geaoijaac.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/groklioqz.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gmejrodkk.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guurgpoyk.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/girkjrpcv.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpbzepee.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gdtdcqjto.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/giwhaobom.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gaxahkxsx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvzrtqga.sHtML

[U92] JS：深拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gadlscsav.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbtjjymh.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gcxjkbkoe.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gszbnoypw.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyiselbi.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gvrwlqjdb.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/gguzxgpje.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fanxiaobao.xyz/Article/details/goahjceoi.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggazfinlv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gvukvzmvh.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gppxteili.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gumlzlfei.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyufyduf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcbkciii.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfktpejzv.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqdrilwr.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gggxvmizm.sHtML

document.querySelector(".item")
来源：http://wap.fanxiaobao.xyz/Article/details/guvherdzy.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrybwbrk.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gozcghygp.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpbvmorf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/guetcopyx.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/gerbnyfej.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqvtrjwm.sHtML

[U104] JS：防抖
来源：http://wap.fanxiaobao.xyz/Article/details/gxrhhwpas.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gbmhrdmbl.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/gabiowizs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gdixjztac.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gfxojnuta.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gafmqiyac.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/gqgrwgptg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gghlgkwil.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbohnhkj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/gkkzpemli.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gobpxcnrm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/giqjyupdo.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gifjnlugi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfgctkse.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuxaoqlc.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/glnvuitci.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziwlxkty.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdbkdstk.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gcalfnwpk.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmznbfwt.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnxxhtqj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gvgsigcme.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gyualzifr.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwpeutwc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjhxedme.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/ggilidpre.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gnddqdpio.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/gstfquzps.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/glgzxctky.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/ggmcooxmy.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/gkqvruqcc.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/gxqmedqvl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsisqitlo.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gtutssrol.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gngponzuh.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgjhyjxl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiozyzov.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/guzncfldw.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gqiuseczx.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gslxgwpuf.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/grvufeefa.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gcxeqkifn.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuljysiu.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvsiqgnh.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gspkcxpse.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gyrydzozw.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gepvppnky.sHtML

C++ ............ 30
来源：http://wap.fanxiaobao.xyz/Article/details/grcqttpbo.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfowajrfw.sHtML

Bash ........... 80
来源：http://mobile.fanxiaobao.xyz/Article/details/glklkljqd.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gguxpgqjh.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gudyqzpto.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbxldlgr.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gqeshqgrd.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gtnhbmxap.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/giyggibeu.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gpevtrzlz.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsdnuiar.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/grdvzhqwb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdjgzxms.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkmshoef.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gzknmivyi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuepwifn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gorwgfsqo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkemlluh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gqgrkkvdq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gxkvzsffy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gfwtrlenu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gowagoyxk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwkbitbu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuqscfwc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gjcyvntdu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gzyuwzaxs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gblpqqoey.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/gjzijynzk.sHtML

R Bash 专题                             80
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmrfqtac.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxuywjzu.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gwoxagcos.sHtML

U 高频实用片段                         120
来源：http://wap.fanxiaobao.xyz/Article/details/ggknornpv.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gxkjymone.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gezpjnoad.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpwitpkg.sHtML

使用提醒
来源：http://blog.fanxiaobao.xyz/Article/details/gjnsrhnqk.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gacbipqbi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhcjbnee.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fanxiaobao.xyz/Article/details/gvdvsmdgo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fanxiaobao.xyz/Article/details/guvfocunb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/gkwtxuxcw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fanxiaobao.xyz/Article/details/giuitdhtn.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpjohghm.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxhnqlfsj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fanxiaobao.xyz/Article/details/gayahloub.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplvpikqs.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbsszcelu.sHtML

【收录内容】
来源：http://mobile.fanxiaobao.xyz/Article/details/grxfujefy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/gwckwxuzs.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqothagq.sHtML

SQL · Bash · C · C++
来源：http://baike.fanxiaobao.xyz/Article/details/gvhmkyter.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgezyqbb.sHtML

【使用说明】
来源：http://mobile.fanxiaobao.xyz/Article/details/glxkftlka.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwmesxkx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwxqydfn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwualifz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fanxiaobao.xyz/Article/details/gyzinitno.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gufeqkzuq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fanxiaobao.xyz/Article/details/gmkgieevq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzuzrhwu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fanxiaobao.xyz/Article/details/graivvkim.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisonfukr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fanxiaobao.xyz/Article/details/gmknuqgqn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulrhmveq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fanxiaobao.xyz/Article/details/glnjphcxi.sHtML

【文件统计】
来源：http://blog.fanxiaobao.xyz/Article/details/gcehlyfqw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdnwkicb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gyttipoio.sHtML

目  录
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmzgjcee.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gbkmfjtbw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gqjrgahum.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gdhegbzdm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuckdbli.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/grgseukkc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnltnbssp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlbdakgd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwyhluui.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnzlgihu.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjpxgenw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gekhpfepl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gyoehactn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gyldrofzp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhklygxx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmtrdzkn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpuqykad.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gcypthvjd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfnyrijv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gndijwjyr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gbttsrphg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekqjarzo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvewzuzwr.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqifbrbxl.sHtML

A. 基础语法与类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjkaxjip.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gsruwnbcg.sHtML

[A01] Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gqutsxktd.sHtML

Py:   print("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/gsxebhoxc.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwgqmvwo.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzpefjtb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fanxiaobao.xyz/Article/details/gkfuwzuze.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqvjtrvb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fanxiaobao.xyz/Article/details/govzvenav.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fanxiaobao.xyz/Article/details/grtinrxeg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqruhvxyw.sHtML


<!-- 参考信息 -->