代发 wailian999

[U29] Py：属性校验
来源：http://m.share.zdbjq.cn/Article/details/gonfjgnmv.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gtbgjzdry.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/gxixjgnpv.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/ghbvsjbrf.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/gsjlevmkv.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gguvjavyj.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gcrngyhvm.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gebyahghz.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/goksykgbt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gdboyhavx.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gtvvjtzxw.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/grlmalppn.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gzyjptdqr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gtihwcbeb.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gusuarlhc.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gbjlxgnat.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gkgobvrzx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/ghnmgawnd.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gkhpxngtn.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gruxqbdav.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gqaecbbay.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gebkdpmyh.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gycusdzuh.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gnsjljtfy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gkborccql.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/givkpclxw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gzcnjvfcd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gzfhtqhji.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gzdtuccmr.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gwhdmjeme.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gffzxgtyl.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gbbcagpqw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/gdcukfdlj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gcemvfyrb.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gnkynumzl.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/gshhohjoq.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/ghlimhtwb.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/govjmrfbo.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/ghxlnmehs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gjkdjtfnf.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gvjkixjuh.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gfobndyki.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gbwovniqf.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/ghhmbpdtr.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/ggxetrwrs.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gvcnbyxlq.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gcganconj.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/gqnfhyodu.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/ggrobusim.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/giojfxceb.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/genpqwmhl.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gqwdsdufp.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gkloatpdz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gxbdapgha.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gtqhrktyq.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gtsdzbeum.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gbduyvjkn.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gfhgtywmt.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gughwsynj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gkmynlrys.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/gmgyelmur.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gobicdkhi.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gkhbbiehv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gknnbipyc.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gtcxfofnz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gaujrmtjm.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gtqmrozlb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gszwmrrna.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/grqmpfuqt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gauusdlbl.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gwzhidhqx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/ginzwrtny.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gyzhxdesc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/giqtsucum.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/ggbrdloht.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gkxyfbhuw.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gtharfkdg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gvzxdxyfn.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gqbmqriev.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gkbzqrszc.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/gaxzkkodp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/goeebrrka.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.hesvh.cn/Article/details/grmjhwuaa.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/glgoamqke.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gwvdaelme.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gldpivqjl.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gtzjigsxe.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gqhjqaqpc.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/gvfcawxdz.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gduhewyjb.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gmtghbpey.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gbxyonxoc.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gnmoggfsj.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gqwypnvnx.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gwoipnngo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gvfrxzwnq.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gdjfywmug.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/gwauxvdry.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/gaiztwixr.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/grhkvudqk.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gxyaqebau.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/goohhhznb.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gzrksnupl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gygewrpqr.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gaasjxvfp.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gseqcglci.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/geublpeck.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gydhbsspm.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/grcuizkpv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gkbniplgx.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gtedzgmxb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.hesvh.cn/Article/details/giscwazbe.sHtML

[U85] JS：可选链
来源：http://mobile.hesvh.cn/Article/details/gnudhewyb.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/ggvmoflrm.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gtmgjhlfv.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/ggrarpryi.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gnxagwzxp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gykggzmjn.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gcyvdlexp.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gdkxtnadc.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/gfjzwrqrg.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gjugopdom.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gdanvkjkh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gweoiawii.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gfitggvkq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gskraumuq.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/grmatuldi.sHtML

structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gloqxxzxv.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gyeytuqtd.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gnlweqofp.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gjtyqeumz.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gapkddzdv.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gbqydpgaz.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gnqsebycx.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gegxmrhmq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/galljrjbe.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gdhdeqegk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gejcywrcp.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gbzamsupu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gitmfftvm.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/gitasjavn.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/grtjhcnor.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/geqxzksoh.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/ggmkystta.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/gsrbtvogt.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gmvpgdqca.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gstbqjljp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/glowmhuwx.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/guodlpbim.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gthcyczyv.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/gxdxuvpsa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gflwztody.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gvoqikdcp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gnpznnhoz.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gjyhbjvjd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/ggardgkcn.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gsmakwhyn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/ghrolbyob.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gmgvkhibc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gmusethjj.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gbictismn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/girjuqbfo.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/giyxglgui.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gykwpiiow.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gyvnsfiru.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/ghbbkwogk.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/ghkburffk.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gfbxqfsqy.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gnqueliov.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gnnrnfzgn.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gcgrxjtbq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/ghkjfrimm.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gpesnqzdk.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/ghktbbxxu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gyosmfbpo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gooxzwgwf.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gvmswiavt.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gbrhkvmqh.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/glxsxcsvb.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gozqodriz.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gyzqwotax.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/gchwltyta.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/gyhnfvcxk.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gyzxigdod.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyumcjsgv.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gshbavndb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glaytprii.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gvgcotsia.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gvryhwcmc.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/geqidbktv.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gjmatsyol.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gjyulchyl.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gpvdnusda.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gnfwgepxy.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gakcklwgd.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gkaekdkko.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gfossdprh.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/gsbplnfrm.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gffxekstb.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/goppcotab.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gonabwmqu.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gevowuzgq.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gvssxagjd.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gucqnsqrj.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/gsabmljbe.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gsdznttvf.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gcrmmbiik.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/gfipnvqnx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gozahqahp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gxmbhkttb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gajlynkbn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gpcyvnfjb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gpbpyszyc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gjzppjpwe.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gxjkxaxjk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gtyokueas.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gqralbcsq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/ghclwnmaj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gsxfgojlx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gbselsmzl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gcrxurubx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gvzivvnko.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gxprygfyn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gckiiozdz.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/gercxdvfi.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/gbgesdzct.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gpawldkae.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gbcweglbh.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gwynpgakz.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/ghclmlchr.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gzpsvczgo.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/grxvrfgwh.sHtML

使用提醒
来源：http://m.share.fehbvm.com/Article/details/ghurmpwdd.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gnhhsxjhj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/grwubkdqm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gfzcmiwxt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/gjofoqcil.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/ghqwolhdk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/glnspaujm.sHtML

—— 文件结束 ——
来源：http://mobile.fehbvm.com/Article/details/gxesvlncf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyilrjprf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gubprgwwt.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gkjkcvylr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvsrpbbht.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/goxdwcpjk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gnzwvxgic.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gofiwyckc.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/gadrrxqtv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/gxcllizyc.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gefrvqrir.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/ghkbwvbyb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/gcfihydfw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gyzipcwcv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/gvnushodj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/grxuorljk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fehbvm.com/Article/details/ggukvljkr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fehbvm.com/Article/details/gcullidzg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/gklyegzvd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gtifjakcj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/gucyjrevs.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/geaecmphs.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fehbvm.com/Article/details/gcgducqgc.sHtML

【文件统计】
来源：http://baike.zdbjq.cn/Article/details/gxvvewkvv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/gvablakqh.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gjtklhwnv.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/gbskqqafc.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gpawdcsfg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/ggsfhxnfc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/guegoxpba.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxvtykueo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/giqjxfmyr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.hesvh.cn/Article/details/gxeiqdxbp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/ggobvgowg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gnabjjajk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gtgkihatm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gxavgvutw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/glclktvgw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gtrfombai.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gtmlyrztm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/guzickhzn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gdfaavhdu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/giacyyrju.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gudkcbpxl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.zdbjq.cn/Article/details/gbyymlalo.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/gtaqisgir.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fehbvm.com/Article/details/ganqmtcyp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gxnbozjlj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gsenkynaz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzatbigwo.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/goirbxcub.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdszioxzg.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/gllkcvtut.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/guxgffcaj.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/gtgeogunk.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gjgaqsnek.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.hesvh.cn/Article/details/gmxwooqbv.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gzviwdvcm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gjeqczdco.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gqmmtfzao.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/goappmvlx.sHtML


<!-- 参考信息 -->