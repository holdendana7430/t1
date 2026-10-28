代发 wailian999

[U31] Py：单测
来源：http://hz.c1oappe.top/gtlcqwxcdj.html

python -m pytest -q
来源：http://hz.zhiwuduotai.top/gtssdrucqm.html

[U32] Py：代码格式化
来源：http://hz.ywan-chungtsiang.top/gtebigiggb.html

ruff format . && ruff check --fix .
来源：http://hz.fzhhl.top/gttdbqmybj.html

[U33] Py：打包发布
来源：http://hz.xinyue.icu/gtwnmgfcnb.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jianghu66.top/gttretdodg.html

[U34] Py：判断编码
来源：http://hz.pycfn.com/gtkcxzovwk.html

chardet.detect(raw)
来源：http://hz.jqgufenzy.top/gtezbohrde.html

[U35] Py：发送邮件
来源：http://hz.chenjidiqi.icu/gtvzwfldix.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.gotoacloud.top/gtuvmvhjhx.html

[U36] Py：定时任务
来源：http://hz.dashuyun.cn/gtrahxsaow.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhijiandao.cn/gtzswxguyj.html

[U37] Py：读写 Excel
来源：http://hz.havefunace.top/gtvdxerolb.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ybcxt.top/gtqflamwdf.html

[U38] Py：获取脚本所在目录
来源：http://hz.nanxinkj.top/gtjkwrgmum.html

Path(__file__).resolve().parent
来源：http://hz.nanxuanxn.top/gtihoippbn.html

[U39] Py：判断是否在交互环境
来源：http://hz.yueranfly.top/gtqcmihsqd.html

sys.stdout.isatty()
来源：http://hz.ydjk.org.cn/gtuyjubbuh.html

[U40] Py：打印到标准错误
来源：http://hz.gaohongyu789.top/gtyuxqkdsh.html

print("err", file=sys.stderr)
来源：http://hz.0kj1m.cn/gtkyvyqezl.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.svipenyu.cn/gtczhlgfvq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.xziqi.cn/gtcqrwagkv.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhijiandao.cn/gtxawopmoa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.9152youxi.cn/gtbkqdhmsw.html

[U43] PHP：声明命名空间
来源：http://hz.chenjidiqi.icu/gtglzuuagc.html

namespace App\Http;
来源：http://hz.0kj1m.cn/gttvghywbb.html

[U44] PHP：开启严格类型
来源：http://hz.sweek.top/gtgzvjswjg.html

declare(strict_types=1);
来源：http://hz.hfpthk.cn/gtrowxkuky.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yueranfly.top/gtqirfjjsv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gzhubu.top/gtzmwcyhms.html

[U46] PHP：可空类型
来源：http://hz.yuxming.cn/gtrhgzjsrb.html

?string $name = null
来源：http://hz.yonumen.top/gthhsoqmnd.html

[U47] PHP：联合类型
来源：http://hz.xziqi.cn/gtegnzbadm.html

int|string $id
来源：http://hz.zhixingplan.top/gtsilkdpej.html

[U48] PHP：纯枚举
来源：http://hz.dashuyun.cn/gtltulmsup.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yangfankeji.com/gtgvbdailz.html

[U49] PHP：只读属性
来源：http://hz.nanxuanxn.top/gthdekgcth.html

public readonly string $name
来源：http://hz.xinyue.icu/gtsfixvvge.html

[U50] PHP：构造器属性提升
来源：http://hz.dianchejie.cn/gtfnvhvdol.html

public function __construct(private int $id) {}
来源：http://hz.smart0.xyz/gtemgwmbpl.html

[U51] PHP：数组解构
来源：http://hz.hnqzz.top/gtegjauvyw.html

[$a, $b] = $arr;
来源：http://hz.tian-w.cn/gtrtasvvsa.html

[U52] PHP：箭头函数
来源：http://hz.yj20258.top/gtpeuidfwh.html

$double = fn($x) => $x * 2;
来源：http://hz.mhx1999.top/gtqfkchymm.html

[U53] PHP：空合并运算符
来源：http://hz.quarkkingdee.top/gtgmwjebci.html

$v = $a ?? $b ?? "default";
来源：http://hz.xinyue.icu/gtvbktwrbk.html

[U54] PHP：空安全调用
来源：http://hz.yj202588.top/gtemaieegh.html

$obj?->method()
来源：http://hz.cheryme.top/gtzefsdiji.html

[U55] PHP：match 表达式
来源：http://hz.zhijiandao.cn/gtvhuokytt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jyoumei.cn/gtkjbkyroi.html

[U56] PHP：命名参数
来源：http://hz.guowangkeji.top/gtgxkotluv.html

f(a: 1, b: 2)
来源：http://hz.fzhhl.top/gtxucfijrs.html

[U57] PHP：字符串插值
来源：http://hz.zhengqikj.top/gttqsftzsg.html

"值: {$a}"
来源：http://hz.gzhubu.top/gtgtyjukbf.html

[U58] PHP：数组三件套
来源：http://hz.zycfv.cn/gteunsdmpx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.wangdashe.top/gtznjttdct.html

[U59] PHP：自定义排序
来源：http://hz.cqqwz.cn/gtomaamayq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nwbrower.top/gtutdwqbyj.html

[U60] PHP：JSON 编解码
来源：http://hz.daria6918.cn/gtgslrbenl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhongyouzk.top/gtthflozjz.html

[U61] PHP：正则
来源：http://hz.316326.xyz/gtwdxpywkk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hfpthk.cn/gtofzgfxms.html

[U62] PHP：日期对象
来源：http://hz.tian-w.cn/gttvltjlpp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.cheryme.top/gtqfkqbcvo.html

[U63] PHP：文件读写
来源：http://hz.yuxming.cn/gtnrplwxxk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yvedp.cn/gtrzzcsvuq.html

[U64] PHP：目录遍历
来源：http://hz.chenlongwang.top/gtgelpqcru.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.iojbl.cn/gtugtxfsdq.html

[U65] PHP：会话
来源：http://hz.hnxiangtu.top/gtqkxedgto.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.svipenyu.cn/gtnfbqzmyx.html

[U66] PHP：设置 Cookie
来源：http://hz.ybcxt.top/gtzdtclhgw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.xuetiantiany.cn/gtlrevvrnn.html

[U67] PHP：处理文件上传
来源：http://hz.jyoumei.cn/gtusbyjbpp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.cqqwz.cn/gtezaqpjca.html

[U68] PHP：PDO 连接
来源：http://hz.jinyuanbaomall.cn/gtoututbut.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.gotoacloud.top/gtdksbbffh.html

[U69] PHP：PDO 预处理
来源：http://hz.aizwys.cn/gtkybvtbzy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hnxiangtu.top/gtdlhybacg.html

[U70] PHP：PDO 事务
来源：http://hz.gogol.net.cn/gtmkqwnooe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.chenlongwang.top/gtjhabsimv.html

[U71] PHP：抛出异常
来源：http://hz.jqgfzy.top/gteppilydq.html

throw new RuntimeException("失败", 500);
来源：http://hz.hnxiangtu.top/gtlzzhdcid.html

[U72] PHP：写错误日志
来源：http://hz.dianchejie.cn/gtknlibzwc.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhiwuduotai.top/gtfobscjib.html

[U73] PHP：读取 ini 配置
来源：http://hz.nanxinkj.top/gtrrdoruil.html

parse_ini_file("config.ini", true)
来源：http://hz.sysykeji.top/gtnxumlfev.html

[U74] PHP：读取环境变量
来源：http://hz.yj202588.top/gttiieuwkc.html

getenv("APP_ENV") ?: "production"
来源：http://hz.feifeiyinyue.top/gtkmngdigj.html

[U75] PHP：依赖注入
来源：http://hz.pycfn.com/gtrfkcdupg.html

composer require psr/container
来源：http://hz.jinqigfzy.top/gtdrbkendr.html

[U76] PHP：简单路由
来源：http://hz.shanyushiyangkeji.top/gtvmtnmojd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zycfv.cn/gthwwavrub.html

[U77] PHP：模板渲染
来源：http://hz.nanxinkj.top/gtykpnkepr.html

composer require twig/twig
来源：http://hz.sxryk.cn/gtegrdxeij.html

[U78] PHP：单元测试
来源：http://hz.andypj.xyz/gtornsuyqh.html

composer require --dev phpunit/phpunit
来源：http://hz.xziqi.cn/gtntnjkfef.html

[U79] PHP：静态分析
来源：http://hz.xziqi.cn/gtelhkgnkz.html

composer require --dev phpstan/phpstan
来源：http://hz.zhengqikj.top/gtqkbukeay.html

[U80] PHP：代码规范修复
来源：http://hz.cucudq.cn/gtutnzljaq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hammf.cn/gtgteicwgd.html

[U81] JS：初始化项目
来源：http://hz.ybcxt.top/gtocloudvm.html

npm init -y;  npm i express
来源：http://hz.zycfv.cn/gtakxxbejc.html

[U82] JS：package.json 脚本
来源：http://hz.ehwqpu.com/gtkongfeij.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.pengpengdd.cyou/gtbiynumtk.html

[U83] JS：ES Module 导入导出
来源：http://hz.ywan-chungtsiang.top/gtzcgdmmrj.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.hongshengwenyu.top/gtxiqemshb.html

[U84] JS：CommonJS 写法
来源：http://hz.jianghu66.top/gtqequrcvi.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.xingfuxueyuan.xyz/gtkhmveply.html

[U85] JS：可选链
来源：http://hz.xingfuxueyuan.xyz/gtvaetkdtt.html

a?.b?.c
来源：http://hz.jiagoushi.top/gthmziketa.html

[U86] JS：空值合并
来源：http://hz.gogol.net.cn/gtzkcoxhpa.html

a ?? b
来源：http://hz.kuanghao11.cn/gtxbiwxmss.html

[U87] JS：解构默认值
来源：http://hz.daria6918.cn/gtzxkxqofk.html

const { a = 1, b = 2 } = obj;
来源：http://hz.fengsongda.top/gtovudyinu.html

[U88] JS：对象展开合并
来源：http://hz.yj20258.top/gtdkiihjpg.html

{ ...a, ...b }
来源：http://hz.zycfv.cn/gtnbapcjxp.html

[U89] JS：数组去重
来源：http://hz.zycfv.cn/gttcunwrhb.html

[...new Set(arr)]
来源：http://hz.zhengqikj.top/gtnriolrzi.html

[U90] JS：数字数组排序
来源：http://hz.gotoacloud.top/gtkvtagfzw.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hfpthk.cn/gtfguffoto.html

[U91] JS：对象键值遍历
来源：http://hz.316326.xyz/gtphtjrnrq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yj20258.top/gtzsjbadkg.html

[U92] JS：深拷贝
来源：http://hz.jyoumei.cn/gtuhksrmbm.html

structuredClone(obj)
来源：http://hz.daria6918.cn/gtezguhkrz.html

[U93] JS：模板字符串
来源：http://hz.ivvv.top/gtjyivzbsw.html

`共 ${n} 条`
来源：http://hz.jinghuilouyu.cn/gtuecfzodl.html

[U94] JS：箭头函数
来源：http://hz.sysykeji.top/gtgbdvwcpt.html

const double = x => x * 2;
来源：http://hz.zdqjudy.top/gtmikvqlet.html

[U95] JS：Promise 包装
来源：http://hz.c1oappe.top/gtalvumpoj.html

new Promise((resolve, reject) => {})
来源：http://hz.tian-w.cn/gtpqcigffi.html

[U96] JS：async/await 与异常
来源：http://hz.yj20258.top/gtkdvfabxo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.316326.xyz/gtmhtwyyca.html

[U97] JS：并发请求
来源：http://hz.meibo888.top/gtmziqztii.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtiqvahdxe.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhijiandao.cn/gtabwiyipb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhixingplan.top/gtqibtqgte.html

[U99] JS：事件监听
来源：http://hz.yj20258888.top/gtmtwzsmvy.html

el.addEventListener("click", e => {})
来源：http://hz.sysykeji.top/gtrjudmglb.html

[U100] JS：DOM 查询
来源：http://hz.fengsongda.top/gthywwfdis.html

document.querySelector(".item")
来源：http://hz.havefunace.top/gtpxoldvqq.html

[U101] JS：classList 操作
来源：http://hz.ppjwa.cn/gteiaxkwqd.html

el.classList.toggle("active")
来源：http://hz.jinghuilouyu.cn/gteziqiblm.html

[U102] JS：本地存储
来源：http://hz.tianlin.xyz/gtdtvjqqcn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.iojbl.cn/gtoentnsas.html

[U103] JS：定时器
来源：http://hz.ppjwa.cn/gtkpscpfjq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.nwbrower.top/gtcmivlmbx.html

[U104] JS：防抖
来源：http://hz.ppjwa.cn/gtvxkoivpu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangshuangyany.cn/gtijslwjwc.html

[U105] JS：节流
来源：http://hz.jinqigfzy.top/gtjrusaebs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yvedp.cn/gtlowbufhj.html

[U106] JS：日期格式化
来源：http://hz.gogol.net.cn/gtpywrhzyb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.hammf.cn/gtjqkdudoh.html

[U107] JS：数字千分位
来源：http://hz.yueranfly.top/gtnkkpbscb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhijiandao.cn/gtekmtybjz.html

[U108] JS：随机整数
来源：http://hz.fengsongda.top/gtpqqnjizi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hongshengwenyu.top/gtuporcprj.html

[U109] JS：数组分组
来源：http://hz.zhengqikj.top/gtecbtohei.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yj20258.top/gtzddymnga.html

[U110] JS：数组分块
来源：http://hz.fzhhl.top/gtfsidfwmk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.shuidangran.top/gtembhmgtw.html

[U111] JS：对象转 Map
来源：http://hz.chenlongwang.top/gtiqkeoigj.html

new Map(Object.entries(obj))
来源：http://hz.yuanzhike.top/gtxswstpcd.html

[U112] JS：字符串补位
来源：http://hz.birdmap.top/gtbtaaazwe.html

"7".padStart(3, "0")
来源：http://hz.jinghuilouyu.cn/gtfzqljawt.html

[U113] JS：正则替换全部
来源：http://hz.shanyushiyangtech.top/gtomydpisq.html

s.replaceAll("a", "b")
来源：http://hz.zdqjudy.top/gtnzyqmiad.html

[U114] JS：JSON 深比较
来源：http://hz.guowangkeji.top/gtqogaajjq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhongyouzk.top/gtfipnvnli.html

[U115] JS：生成 UUID
来源：http://hz.nanxinkj.top/gtbjnocrrx.html

crypto.randomUUID()
来源：http://hz.yj20258.top/gtegtvcsbd.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.tanke756.top/gtyircdjue.html

/** @param {string} name */ function f(name) {}
来源：http://hz.tianlin.xyz/gtwihznvqo.html

[U117] JS：单元测试
来源：http://hz.tian-w.cn/gtssmmnwej.html

npm i -D vitest;  npx vitest
来源：http://hz.hongshengwenyu.top/gtqqvgshmx.html

[U118] JS：开发服务器
来源：http://hz.jinqigfzy.top/gtyvajfuky.html

npm i -D vite;  npx vite
来源：http://hz.9152youxi.cn/gtbjbixymc.html

[U119] JS：生产构建
来源：http://hz.xinyue.icu/gtisyvsdgx.html

npx vite build
来源：http://hz.vqdsnc.cn/gtylrmxwfa.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.gaohongyu789.top/gtftfskhdv.html

import.meta.env.VITE_API_URL
来源：http://hz.mhx1999.top/gtzrtleidx.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtbcjmynwu.html

统计汇总
来源：http://hz.zhixingplan.top/gtmgrwgxft.html

================================================================================
来源：http://hz.pycfn.com/gtsvarkpfk.html

按语言统计（条）：
来源：http://hz.pycfn.com/gtxxujjcav.html

Python ......... 252
来源：http://hz.ydjk.org.cn/gtgtiejant.html

PHP ............ 252
来源：http://hz.bjfxy.top/gtschveqsj.html

JavaScript ..... 252
来源：http://hz.yvedp.cn/gtybjwapmk.html

TypeScript ..... 212
来源：http://hz.cqqwz.cn/gtvmssujdi.html

Java ........... 212
来源：http://hz.aizwys.cn/gtyvwihndj.html

Go ............. 212
来源：http://hz.xuanzx.com/gthrkhabwh.html

Ruby ........... 212
来源：http://hz.yj20258.top/gttcmfgpcf.html

C# ............. 212
来源：http://hz.daxiang520.top/gtaiwvwibe.html

C .............. 30
来源：http://hz.iojbl.cn/gtwvmklsqa.html

C++ ............ 30
来源：http://hz.zhixingplan.top/gtbsognsec.html

SQL ............ 90
来源：http://hz.cheryme.top/gthjulozqp.html

Bash ........... 80
来源：http://hz.jqgufenzy.top/gtitkqcvzq.html

Kotlin ......... 15
来源：http://hz.c1oappe.top/gtmxoiiqph.html

Swift .......... 15
来源：http://hz.jinyuanbaomall.cn/gtpmecvhpq.html

Lua ............ 10
来源：http://hz.yuxming.cn/gtnjqfbidv.html

Perl ........... 10
来源：http://hz.iojbl.cn/gtckewykla.html

Scala .......... 10
来源：http://hz.meibo888.top/gtwlcwxnpe.html

------------------------------------
来源：http://hz.havefunace.top/gttmxwwkvl.html

合计 ........... 2106 条
来源：http://hz.snrcjt.cn/gtiuwlyata.html

按章节统计：
来源：http://hz.ehwqpu.com/gtrydsbizl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hywenlv.cn/gtiokkiofu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.xingfuxueyuan.xyz/gtxuydttvm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.shanyushiyangtech.top/gtrwhqtyvh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jlsjyb.cn/gtcbruhlpm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.cucudq.cn/gteapyegow.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.dashuyun.cn/gtyaphneyw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yuxming.cn/gtkznlcfxw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.jinqigfzy.top/gtgcydbpzh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.mhx1999.top/gtutnntadl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.chenzaomai.com/gtyhcmvvcp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.gzhubu.top/gtlnvysaud.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.chenjidiqi.icu/gtglgcnyeq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.shuidangran.top/gtdowzgpid.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.guowangkeji.top/gtxawjehxd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.xuetiantiany.cn/gtrwsnlqbj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.fengsongda.top/gtskdxhknr.html

Q SQL 专题                              90
来源：http://hz.cdnleiting.top/gtpwxaacyo.html

R Bash 专题                             80
来源：http://hz.pycfn.com/gtswtpruno.html

S C / C++ 专题                          60
来源：http://hz.cucudq.cn/gtpexzouok.html

T 其他语言补充                          60
来源：http://hz.hammf.cn/gtsrwttmkj.html

U 高频实用片段                         120
来源：http://hz.ydzc1.top/gtbqpungvg.html

------------------------------------
来源：http://hz.zhengqikj.top/gtocdeqxic.html

合计                                  2106 条
来源：http://hz.tian-w.cn/gtvqaarpwy.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigfzy.top/gtvpjetnem.html

使用提醒
来源：http://hz.gotoacloud.top/gtzfdrpgax.html

--------------------------------------------------------------------------------
来源：http://hz.jiagoushi.top/gtsaafdssw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zhaomingkeji.xyz/gtcdlqxrpe.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.daria6918.cn/gttdbzjcmu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zhoulong.xyz/gtbenlzpgr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yj202588.top/gtsihghfuj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.xziqi.cn/gtfktdrsix.html

—— 文件结束 ——
来源：http://hz.zdqjudy.top/gtpuntvkzf.html

================================================================================
来源：http://hz.chenzaomai.com/gtxlmegwtc.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.xingfuxueyuan.xyz/gtlnxkkoep.html

Common Programming Examples Cheat Book
来源：http://hz.xylfe.cn/gttasfbnks.html

================================================================================
来源：http://hz.gaohongyu789.top/gtrvsrhrsr.html

【收录内容】
来源：http://hz.9152youxi.cn/gtwkejmlcm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.havefunace.top/gtcxjwtbwk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.iojbl.cn/gtjdhipczs.html

SQL · Bash · C · C++
来源：http://hz.yuanzhike.top/gtietkgekh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.hnqzz.top/gtenkktshu.html

【使用说明】
来源：http://hz.ybcxt.top/gtzpagxfth.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yj20258.top/gtojxsijbp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jyoumei.cn/gtdzvpbcam.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.sweek.top/gtmhnyodcx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.pengpengdd.cyou/gtorgtsiui.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.dashuyun.cn/gtrunygswq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.gaohongyu789.top/gtswicztqg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.ywan-chungtsiang.top/gtihrpzmdc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zhoulong.xyz/gtgbzsjbvo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jyoumei.cn/gtxamzfvuw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.cashguo.top/gtiykjusvk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.xuanzx.com/gtjdrhucio.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.hongshengwenyu.top/gtwkeqtolc.html

【文件统计】
来源：http://hz.0kj1m.cn/gtovwjqfte.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.hammf.cn/gtkjnovkln.html

--------------------------------------------------------------------------------
来源：http://hz.gogol.net.cn/gtupmabciy.html

目  录
来源：http://hz.kuanghao11.cn/gtcjvfmhoq.html

--------------------------------------------------------------------------------
来源：http://hz.316326.xyz/gtfzhgvhxl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.aibaodan.cn/gtycpxislr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.haohaochexian.top/gtsemvsdox.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.gogol.net.cn/gtxzfzcara.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.shangyingyoupin.top/gtifbgdglk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.smart0.xyz/gtmwgjvibl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.cashguo.top/gtnkipqixo.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.cheryme.top/gtynydidid.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.daria6918.cn/gtuqgizsgj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.xylfe.cn/gtseazaiep.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.havefunace.top/gtfrdgttmy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jinqigfzy.top/gtomjrgtjx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.mhx1999.top/gtiqjcltjk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.0kj1m.cn/gtlsxyxmms.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yuanzhike.top/gtchqjsdal.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.aibaodan.cn/gtubmhlnzz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.redwolf501.top/gtwikxlkmz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zycfv.cn/gtcqkxsuar.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.yj20258888.top/gtamrmqqbh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hammf.cn/gtfchwjqvl.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.iojbl.cn/gtibdnfjye.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.nanxuanxn.top/gtzjdkfxoe.html

================================================================================
来源：http://hz.aizwys.cn/gtszklobug.html

A. 基础语法与类型
来源：http://hz.c1oappe.top/gtifyfaczq.html

================================================================================
来源：http://hz.ppjwa.cn/gtgyijkzje.html

[A01] Hello World
来源：http://hz.redwolf501.top/gtpozcnksw.html

Py:   print("Hello, World!")
来源：http://hz.hfpthk.cn/gteirwkpcx.html

PHP:  echo "Hello, World!";
来源：http://hz.yuxming.cn/gteuuskzmn.html

JS:   console.log("Hello, World!");
来源：http://hz.zhoulong.xyz/gtvdmmqnub.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.hywenlv.cn/gthiszssin.html

Java: System.out.println("Hello, World!");
来源：http://hz.ywan-chungtsiang.top/gtvqvkxjiq.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.cdnleiting.top/gtgoongckd.html

Ruby: puts "Hello, World!"
来源：http://hz.hongshengwenyu.top/gtpjetprrn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.hnxiangtu.top/gtlqibljbm.html

[A02] 变量声明与赋值
来源：http://hz.shanyushiyangtech.top/gtjbnlfxjj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.sufxvd.cn/gthikhihea.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.fengsongda.top/gtewifyihb.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.shuidangran.top/gtpvrbzujl.html


<!-- 参考信息 -->