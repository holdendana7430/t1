代发 wailian999

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/goypmkown.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gyoqwcdsm.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gmkghgzao.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gztsuemdk.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/ggvvsnyye.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gmwmxzhuv.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gomlrkmts.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gzlonpqtz.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gaedrwjip.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gzfqcfqty.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/gslvvtlcs.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/grmryhwdp.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gxbcwpqyd.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gdykfnsdm.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/grfyoimsc.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/ggmpcfoqd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gymtfpnsh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gsqilzayf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gikqqcptr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gadouuvnl.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gfnokssxz.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/ghazmpvtk.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gwxqjabef.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gxavgcywk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/ghikrvift.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gwsvbbhoi.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gzadmkdne.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gwzdttldo.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/glcjvxobi.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/guyzsisus.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/goyjwqmhy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gcoakrwyh.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gekmswfwx.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/ggrdisgyi.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gzhvkfdjd.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gxplqdcqv.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gwuhdfdrv.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/girsseyhv.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gafxaygzm.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fehbvm.com/Article/details/gqqbshodi.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fehbvm.com/Article/details/guungrrfe.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gsgtmobsh.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gwcvnjhyd.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gdfwkpdte.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gbgsxpfcc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/ghccmdpcp.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gzaiinwoz.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/glrcheoes.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/golotopqt.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/ggrvrobig.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gytcgnvll.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/gzoqiovtd.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gcgdifbis.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gekjiqgbo.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/grmmdkozv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gebccztok.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gkyshipon.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gvmjwjmso.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gjsfhwqot.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gmknmxwhn.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/ghsqqcurv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/gfmmywese.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/ggsrxgchs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gxagnlije.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gmvstzsfj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gmxhzmdsd.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gzenstgow.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/greftksxi.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/geioninuz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/goeimpwyv.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/glgvwmynb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gkjgnolqa.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/ghzdotnmm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/gzgvahpkl.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gsrfeljww.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/gajolssjw.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gkxvhcssj.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gfwtobqos.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/gobpcjank.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/grrsxxsvx.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gvvqburjt.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gjjzryjla.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gfmqakgep.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gdhkvgcai.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/gtckprnql.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gemjahexv.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gnhkmsgdc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gouowqkrk.sHtML

[U77] PHP：模板渲染
来源：http://blog.fehbvm.com/Article/details/ghmmlgewt.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gptvkpoeg.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gxernebfz.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gcsjlufbt.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gwknkmygw.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/gszfptsnp.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gdvtvhvem.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gpuwkqkqk.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gbglruvyh.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gbehnnyxi.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gsqhrnpeh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gmgljdffp.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/ghuhftqav.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gmzsoilrl.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/glbajghwt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gtpuvzxgy.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/gyvohznfw.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gkvtgurbh.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gztjnepdt.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/ggygbbgaa.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gyxcvbeum.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gyqrlupds.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/gerihpqhp.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/ghpkxstdx.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gfxdbqssg.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/glrbenssu.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gqrqpqckd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gkudgteln.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gcnncxuns.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gurvtyrbi.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gehmxjkdv.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gummjtlhk.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gttfyfxch.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gixuwyehq.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/ggpnbfrid.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gkmhksppd.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gionoiazh.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gifqzhdqp.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gncvjcsxc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gliuwqasi.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gxhdpgiwe.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gvsxowkxh.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gjbjbwbga.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gfujqphnr.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gqcrdgrle.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gamgernll.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/ggrzdnrkt.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gaflmusim.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gfzvsnbdq.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/giferqcmr.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gokgtmafu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gfjuvgbad.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gmzipupzp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/goldxrwtt.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gpdpfrqqj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gpqltswdm.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gsvjnacjo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gunrwzhjs.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gylqcfviv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gaqlnvnmt.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gfoezwvfv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gerglhqtf.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gertkstrq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gvobykqci.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gylxunmky.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gqvdbzbvu.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/ghieygkfa.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/geemtqnzl.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gkppodwpi.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/ggzcrqpzo.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gnpsnelqx.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gqnourdgr.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/giesazsre.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gnsjadvim.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gyenjhupd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gyxdjxube.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gtfmdayea.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gyskzgzkx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/gqipplvbu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gycxsxkwl.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gngnjydko.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gzkkticpd.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gdyagokgh.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gjgcxqepb.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gfoocvgak.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gbyxtdqya.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gxdcgfgaq.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gohjalwnc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxnaizlgc.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gcrzhohvy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guklavvyx.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gqwylxari.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gchgxvydf.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gobkytrdp.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/glwflihtz.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/gfzinbhkd.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/gnttepguu.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gcfhqqwet.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gfpswihsv.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/ghajdxlsm.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/ggvhhojgv.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/gbsdqwryv.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gudcjhhpm.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gobaxreor.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/gphsksgmt.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gtgaxmarj.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/gjtlwfjcb.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gribjubse.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gcblpmewp.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/griwdakki.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/ghcyzafzk.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gcapgbovu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gsqrzrhoc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/ghmyjzets.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gowejmukh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gyzwjpsqt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gmxacnmrk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gleowqmqs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gceeslygj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gwfoaclka.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/grboatudl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/guuqubytv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gsdkyblji.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gklznglhh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gwrrfhdjm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/grhhnffig.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/gnmzhayor.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gxnoqnsgq.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/gomxtukip.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gmsucjkfq.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gvuiwkjed.sHtML

T 其他语言补充                          60
来源：http://m.share.hesvh.cn/Article/details/grhmerrxq.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gxrnovhak.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gugjfbicz.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gvnwdcswf.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gkulqcgdw.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gnhqebzsw.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/ghzbmhnzv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gjxadxbsg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gvovzrykk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/gmtubgyzh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/ggzngnhvi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gggafmmvx.sHtML

—— 文件结束 ——
来源：http://blog.zdbjq.cn/Article/details/gkazujmab.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/giogvhpmh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/ghnlalsdg.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gtzchhsvd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gczgbnaqq.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/glfxoswrn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/ghkbsyuth.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/gvlndogbl.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/geafbsqhs.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gjgvyidmc.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/geubwwpgk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gkghlpujj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/glioyhcux.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/gksulbmqv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gdlocyqyj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fehbvm.com/Article/details/gfzojmlbs.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gvukeioxj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.hesvh.cn/Article/details/gfjovosyd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.hesvh.cn/Article/details/gwijmeouk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/gwqhextxs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/gdgyygbor.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/gvwktnmba.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fehbvm.com/Article/details/gnixnsute.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/gzadhdqmy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/gafaqzkzh.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/ggwfuymfq.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gwikqclpd.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/girogsrpa.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gtcmporqx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gafshmvtp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gclenimpl.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gchjlxgtb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/ggdfzvmdi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/ghkluftwo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gzuwevceb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gtvnykwgm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/geujbglkc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gjiagrfgt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gqihfmszo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/grhpaaaoa.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gokaxwyzt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/greurgqea.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.zdbjq.cn/Article/details/giphkvawo.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gcoryxwdi.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/gxjbzpabf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/ghwhdbmqq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.hesvh.cn/Article/details/gwzwxbame.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gnvtkkqpp.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gbaurogti.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gahfglhqu.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/gkzzmooue.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gddocztli.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/gcdgbhocu.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gyviornif.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/gghgtqpbv.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gepsixeww.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.hesvh.cn/Article/details/griarftaw.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/ghkkgfxgi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gyimbxwsx.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/gvmdtivuy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gdyfcbytu.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gmtpgpvkj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gwvjzcdoj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/grgrybkyu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/gdmzhdegd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/gyyqwsdmg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gxdlowaek.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fehbvm.com/Article/details/gjfanwfls.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gqefydcpq.sHtML


<!-- 参考信息 -->