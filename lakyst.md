代发 wailian999

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3rkxdjqwa.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3yzxhfcpu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3fgngbtoc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3zarpjwrb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3bnugkjwg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3dozaxdga.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3brlvbubm.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3pcikveds.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3gypmuseu.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3nggmndza.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jcgxqibc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3rwjfdgnq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3eilruund.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3hjrzwxmb.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hljtzqus.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3udoplkem.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3jdtzhmpe.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3zvacgpjc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3oiricity.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3udnpfsuk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3jbnyvscb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3mftsqkrr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3qvcpujsk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ochvsbzp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3tswczpjk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ziimetyi.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3qtieojgl.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3tnemfpmn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3jhvzmuje.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ygjfyugz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3gjzbnzpb.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lfmylffk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3gxbgzqju.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3nzipplhb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3rmundoms.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3iziqrpnv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3yynhvmdm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3esoqrmwe.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ggzxukby.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3jqxyvjvq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3obouvjev.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lntesvmg.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3fibtsexk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3mnnitnub.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3bttdmszr.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3anxxhzqp.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ipveqzix.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3cefybmuh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ryjsmuoa.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ioghcnhb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3euzvldna.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3gbpjlthe.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3vunekouq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3pikbmrll.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3kngljsth.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vqkhdzyp.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3nmrebpya.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3odcvvgkq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ieoavuoh.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3mttkxdbo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ujkieeii.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3kmttiuqq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3pwyozcgi.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3miihiedd.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fiapouwz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3muapfhwu.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3aydnjlzz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3prijjydy.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3qocpdhci.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xvuwgigq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3xzkaaxod.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3tawibrfp.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3csykvnob.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3jwevtpqo.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ygjhjstu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3sstdchqk.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3qivktrap.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3reymrjtl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3kypvbubf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3xtgiddlt.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3citsyufs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xtzvuciw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3sfnvuaqq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xftbpimp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3uhlgwsuc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3silxdtai.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3kpdvxcyc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3njonvprg.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3esiuxcdq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3bsfgasem.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3mqskjvxz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3tmunmogk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3jxipdnno.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3tajfvmnh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3bmfjgogv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3lvvngrop.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3vbtmrttq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3kboyzvyn.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zgwdneyt.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3lwzxlsen.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3xjfzjpsr.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3hbrdiyqe.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3qqxgsqsa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3wiulgses.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3kbgatwqc.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3lmlvvweh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3dfswbdmo.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3phszwbrh.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3rdtgsihs.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3gjkjesba.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3fqtcfyli.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3jykbiflx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3gjmnlwvc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3zsynvcik.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3wxpnvawj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3jjlkedup.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3qobbwnxf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3libfuqax.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3uwkbpmti.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3omxkrdfu.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3vakhcmkd.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3unjlsgth.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3eeiatokx.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3hyuejbzj.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3bdaaopbp.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3dokzxlyd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3sxhwdnaq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3uerdrtre.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3aapdvajp.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3beuvlqci.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3vnqzjden.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xdoucldy.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vmnnnaaf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3dtdfrhad.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3selqedwo.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zaxrmmme.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qaockrsf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3fkcjjaby.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3baaxlrbd.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jcktceus.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3fmhpoprg.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3hwyyhndb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3hfmfzwkr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvqrdglt.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ouxmgvqo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tpdnvbnz.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3uqvraqru.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3uppmbppq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3uioayuhf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bgowdbpp.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3lyctvgff.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3pxfqgved.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3iddddyen.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3lnlhfuqh.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3lvvseoxx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3sxljfbgz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3rohlizrn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3tkghdmme.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3vjdasqlb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mijkwypy.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3otwxfcsp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3hwnardte.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3slydfdbr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3pidyvmgc.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ymhwuoay.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fykdeiwn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3axprdgpu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3captbzpk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3nzurezuf.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3uhzymlsr.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3clkdqwrq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3tsvggqhz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vtqtxveg.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ysuexcvk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3prxezpop.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jebwoiri.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3itbtlzmi.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xmhxzqmi.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3lbjdvvha.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uylrfljy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kwugwcxl.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qoxdrfyu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3nybeyqpb.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3wvftvtye.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vhhtxskt.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3silfjhif.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ebiygndq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3fcozremw.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3xlbutnpm.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3milrpago.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3pgtnzppi.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3beixxinc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zbtbbria.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3yghrgfqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nknhhfqp.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3urrinwfy.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3bkcsgpxc.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3qnciwopw.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3hbuwcsop.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3gfihjsot.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ibwtpcbu.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3oosiyjdj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3mkpptvnn.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3kuhbaahm.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3inmyqkju.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3zowzxutj.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ynobpebs.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3rsxbefuo.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ozsfsxjx.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3cqounixt.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3tclherba.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3trdfecmf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3iimkzutj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jgnowqen.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3uksyvzrb.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3isovdyru.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3jgrpdnhs.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3rbbdifyy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ahduhqhl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3fxelbksz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3lulynfmi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vaigbvqv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3rmwotryo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3aekybbdo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ackhuoob.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3yvvxnbwh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dwooxjrm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zuebzevm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xlpxqtvc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3jbfecqtm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3asjunjga.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3nhqgjvqd.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3sykdkxdt.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3mlnlfafm.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3gjkgwsiz.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3erhnowdr.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3oibphugd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gfphhwql.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3odagcljv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3shqjgipn.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3aoqwwygy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nwhqjeer.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3mebzcdbc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3nqvjkqtt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3qyimtdqv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3oabjhltf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3nhmnqnqt.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3jwjliiiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvmuxcyq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3jrnjqdhz.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3vdgylllo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfaqovzp.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3ixdnwhyy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3xtvfjhsi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3nnknvsgd.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3lyucrtte.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3kwhghsdh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3tbuzfbrw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3dapjuqui.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3pksciqwi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3wxfbxqzi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3mmlrkkqr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3gdmexdfr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3lgcregjq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3qzqyecyc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3rsyzpsus.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3ynbphner.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3tbwfvduc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3mmomjsqu.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3ajuccxsz.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3mkoorokd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3niyivowd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vcbxuszt.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3kvriubjy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3blpeirqn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3cnnbhshf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uqjpnolj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3xywdtdzu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wripxibe.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3hdumildj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3obdwgjxm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xsqbdowd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3uysbzngk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jxtmoxnk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eagftnmf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jrbimcfp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cpqjftwe.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lyfnkfug.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3rnxkidrk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mckuzflc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3howxneqg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qucyctsf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3krycjins.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3lxcxaodr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ojsfaseb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3drqmhpcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwhkoasu.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3kynhttzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhzfcvsb.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3lobdgtjn.html


<!-- 参考信息 -->