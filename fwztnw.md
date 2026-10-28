代发 wailian999

[U31] Py：单测
来源：http://hz.daxiang520.top/gtszwtjyxh.html

python -m pytest -q
来源：http://hz.vqdsnc.cn/gtsvrfopub.html

[U32] Py：代码格式化
来源：http://hz.zhiwuduotai.top/gtlstvufpc.html

ruff format . && ruff check --fix .
来源：http://hz.iojbl.cn/gtoubbwvja.html

[U33] Py：打包发布
来源：http://hz.jinyuanbaomall.cn/gtrzujrbdr.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.sufxvd.cn/gtfoqnetqj.html

[U34] Py：判断编码
来源：http://hz.vqdsnc.cn/gteppwdxjr.html

chardet.detect(raw)
来源：http://hz.xuanzx.com/gtzjzxupad.html

[U35] Py：发送邮件
来源：http://hz.yangfankeji.com/gtybcevzup.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.guannengcc.top/gthcrgiqnf.html

[U36] Py：定时任务
来源：http://hz.iojbl.cn/gtpjnlbftk.html

schedule.every(10).minutes.do(job)
来源：http://hz.ppjwa.cn/gtobeybbgs.html

[U37] Py：读写 Excel
来源：http://hz.ydzc1.top/gtbozunjlh.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yuxming.cn/gtzzdhhvyn.html

[U38] Py：获取脚本所在目录
来源：http://hz.daxiang520.top/gtntlfvkcx.html

Path(__file__).resolve().parent
来源：http://hz.zhongyouzk.top/gtbhjpejgj.html

[U39] Py：判断是否在交互环境
来源：http://hz.sweek.top/gtqgeamsqv.html

sys.stdout.isatty()
来源：http://hz.wangdashe.top/gtkslhugub.html

[U40] Py：打印到标准错误
来源：http://hz.pengpengdd.cyou/gthofwszwg.html

print("err", file=sys.stderr)
来源：http://hz.ppjwa.cn/gtftqmmbvs.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jqgufenzy.top/gtyymmsncw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ydjk.org.cn/gtogaliyia.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.pengpengdd.cyou/gtfosculha.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.aizwys.cn/gtpdpeeecb.html

[U43] PHP：声明命名空间
来源：http://hz.xinyue.icu/gtpmfbwknu.html

namespace App\Http;
来源：http://hz.zycfv.cn/gtlpuwgafb.html

[U44] PHP：开启严格类型
来源：http://hz.zhongyouzk.top/gtejcdzcdw.html

declare(strict_types=1);
来源：http://hz.nwbrower.top/gtnhhoqilh.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shanyushiyangkeji.top/gthpaxvzef.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ydjk.org.cn/gtjihkxuko.html

[U46] PHP：可空类型
来源：http://hz.jianghu66.top/gtmjixeyub.html

?string $name = null
来源：http://hz.ppjwa.cn/gttrfsppcq.html

[U47] PHP：联合类型
来源：http://hz.jlsjyb.cn/gtgdbflsyy.html

int|string $id
来源：http://hz.316326.xyz/gtsqimqoju.html

[U48] PHP：纯枚举
来源：http://hz.shanyushiyangkeji.top/gthmycidqw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.cdnleiting.top/gtvqicfixf.html

[U49] PHP：只读属性
来源：http://hz.shanyushiyangtech.top/gtsruceiud.html

public readonly string $name
来源：http://hz.ppjwa.cn/gtomfngoks.html

[U50] PHP：构造器属性提升
来源：http://hz.tian-w.cn/gtyetgljjo.html

public function __construct(private int $id) {}
来源：http://hz.9152youxi.cn/gtfrbrjatl.html

[U51] PHP：数组解构
来源：http://hz.yj20258.top/gtlwiknhgl.html

[$a, $b] = $arr;
来源：http://hz.feifeiyinyue.top/gtelijawoa.html

[U52] PHP：箭头函数
来源：http://hz.chenzaomai.com/gtmvkqorbz.html

$double = fn($x) => $x * 2;
来源：http://hz.xuanzx.com/gtaozhphca.html

[U53] PHP：空合并运算符
来源：http://hz.nanxuanxn.top/gtocyehpcb.html

$v = $a ?? $b ?? "default";
来源：http://hz.cashguo.top/gtrkunrevs.html

[U54] PHP：空安全调用
来源：http://hz.xingfuxueyuan.xyz/gtveorgcsj.html

$obj?->method()
来源：http://hz.c1oappe.top/gtmtfwhaqt.html

[U55] PHP：match 表达式
来源：http://hz.hnxiangtu.top/gtspqklodj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhixingplan.top/gtwrrexkmf.html

[U56] PHP：命名参数
来源：http://hz.gogol.net.cn/gtsgzwlnxo.html

f(a: 1, b: 2)
来源：http://hz.wangdashe.top/gtvbnkgyii.html

[U57] PHP：字符串插值
来源：http://hz.tian-w.cn/gttsnvutda.html

"值: {$a}"
来源：http://hz.c1oappe.top/gthnsqrzbq.html

[U58] PHP：数组三件套
来源：http://hz.snrcjt.cn/gtkkgsjrep.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.quarkkingdee.top/gtbbncprkb.html

[U59] PHP：自定义排序
来源：http://hz.guowangkeji.top/gtbfdeqlpo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zdqjudy.top/gtgliyobqq.html

[U60] PHP：JSON 编解码
来源：http://hz.yj20258888.top/gtseahbnxd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.cheryme.top/gtkwlafnoi.html

[U61] PHP：正则
来源：http://hz.xinyue.icu/gtnqtkebyb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.dashuyun.cn/gtdufdnvtp.html

[U62] PHP：日期对象
来源：http://hz.jinqigfzy.top/gtdomimixr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.nanxuanxn.top/gtokfgdcrr.html

[U63] PHP：文件读写
来源：http://hz.jqgfzy.top/gttvchipgb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.ydjk.org.cn/gtuaiuvmcv.html

[U64] PHP：目录遍历
来源：http://hz.cucudq.cn/gtfuhuqxia.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.havefunace.top/gtmrqthubp.html

[U65] PHP：会话
来源：http://hz.smart0.xyz/gtwjemuhhm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hywenlv.cn/gtrskjanhh.html

[U66] PHP：设置 Cookie
来源：http://hz.cucudq.cn/gtsgkdmnrd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.gzhubu.top/gtwwfaraym.html

[U67] PHP：处理文件上传
来源：http://hz.ywan-chungtsiang.top/gtmlzpcrzh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.hysaishi.cn/gttvqzgcao.html

[U68] PHP：PDO 连接
来源：http://hz.yuanzhike.top/gtgekflklr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yongpay.top/gtejyyqsuw.html

[U69] PHP：PDO 预处理
来源：http://hz.hammf.cn/gtaupqjela.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.ydjk.org.cn/gtwxahzzqj.html

[U70] PHP：PDO 事务
来源：http://hz.ivvv.top/gtklgshubg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.gotoacloud.top/gthvmlkvzy.html

[U71] PHP：抛出异常
来源：http://hz.zycfv.cn/gttwkicpqi.html

throw new RuntimeException("失败", 500);
来源：http://hz.ehwqpu.com/gtpjadfreu.html

[U72] PHP：写错误日志
来源：http://hz.chenlongwang.top/gtqtrfjbni.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hywenlv.cn/gtxavnnoee.html

[U73] PHP：读取 ini 配置
来源：http://hz.jinqigufen.top/gtyouoflcj.html

parse_ini_file("config.ini", true)
来源：http://hz.zdqjudy.top/gteurlhejf.html

[U74] PHP：读取环境变量
来源：http://hz.gaohongyu789.top/gtzgyhxpyo.html

getenv("APP_ENV") ?: "production"
来源：http://hz.dianchejie.cn/gthewfodca.html

[U75] PHP：依赖注入
来源：http://hz.9152youxi.cn/gtnhuevkdj.html

composer require psr/container
来源：http://hz.daria6918.cn/gtjbukuyeg.html

[U76] PHP：简单路由
来源：http://hz.meibo888.top/gtkdppycyx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.aizwys.cn/gtwsogalpw.html

[U77] PHP：模板渲染
来源：http://hz.hywenlv.cn/gtfzksypzy.html

composer require twig/twig
来源：http://hz.jyoumei.cn/gtqsrsskms.html

[U78] PHP：单元测试
来源：http://hz.yuanzhike.top/gtsogkqohq.html

composer require --dev phpunit/phpunit
来源：http://hz.gaohongyu789.top/gttokkbqbz.html

[U79] PHP：静态分析
来源：http://hz.shzxlz.cn/gtkjbierbx.html

composer require --dev phpstan/phpstan
来源：http://hz.daxiang520.top/gtjsdfffaq.html

[U80] PHP：代码规范修复
来源：http://hz.gotoacloud.top/gtnjddtnab.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.chenlongwang.top/gtykguysou.html

[U81] JS：初始化项目
来源：http://hz.yangfankeji.com/gtdksqmwai.html

npm init -y;  npm i express
来源：http://hz.hfpthk.cn/gtzgntcyrf.html

[U82] JS：package.json 脚本
来源：http://hz.nanxuanxn.top/gtdqzfkjmj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.gaohongyu789.top/gtvqzdgwbs.html

[U83] JS：ES Module 导入导出
来源：http://hz.jqgufenzy.top/gtydgvlizg.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.jinqigufen.top/gttcnceoca.html

[U84] JS：CommonJS 写法
来源：http://hz.tanke756.top/gtkiqrqabh.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jqgfzy.top/gtogwtltad.html

[U85] JS：可选链
来源：http://hz.sufxvd.cn/gtvfimyaxc.html

a?.b?.c
来源：http://hz.zdqjudy.top/gtgqezhsze.html

[U86] JS：空值合并
来源：http://hz.jinghuilouyu.cn/gtnxekeikh.html

a ?? b
来源：http://hz.zhaomingkeji.xyz/gtitmtesqw.html

[U87] JS：解构默认值
来源：http://hz.9152youxi.cn/gtbyidkcde.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jinyuanbaomall.cn/gtscfkkaju.html

[U88] JS：对象展开合并
来源：http://hz.dianchejie.cn/gtnlegkiwa.html

{ ...a, ...b }
来源：http://hz.zhiwuduotai.top/gtyucsdbcj.html

[U89] JS：数组去重
来源：http://hz.iojbl.cn/gtnybfrtfm.html

[...new Set(arr)]
来源：http://hz.tian-w.cn/gtacaqvuet.html

[U90] JS：数字数组排序
来源：http://hz.yj20258888.top/gtegbcinwb.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yj20258888.top/gtdlnoerzz.html

[U91] JS：对象键值遍历
来源：http://hz.xuetiantiany.cn/gtekduxgyn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jinqigfzy.top/gtkvrllfpl.html

[U92] JS：深拷贝
来源：http://hz.jqgufenzy.top/gtjznndkxt.html

structuredClone(obj)
来源：http://hz.cucudq.cn/gtutbfqipg.html

[U93] JS：模板字符串
来源：http://hz.cqqwz.cn/gtsrhckzuy.html

`共 ${n} 条`
来源：http://hz.wangshuangyany.cn/gtvkixoozj.html

[U94] JS：箭头函数
来源：http://hz.yueranfly.top/gtwthtbyft.html

const double = x => x * 2;
来源：http://hz.dashuyun.cn/gtuiijlzwu.html

[U95] JS：Promise 包装
来源：http://hz.cdnleiting.top/gtsfcspwen.html

new Promise((resolve, reject) => {})
来源：http://hz.0kj1m.cn/gthzhzdetq.html

[U96] JS：async/await 与异常
来源：http://hz.fzhhl.top/gtcoypkgii.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.tanke756.top/gtegcjclyn.html

[U97] JS：并发请求
来源：http://hz.chenzaomai.com/gtoacoiavx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.52xcode.cn/gtnqwfgelm.html

[U98] JS：fetch 带 JSON
来源：http://hz.yanxiufei.cn/gteydbdibo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.cqqwz.cn/gtcirjdcqb.html

[U99] JS：事件监听
来源：http://hz.pycfn.com/gtmeqhipmx.html

el.addEventListener("click", e => {})
来源：http://hz.cdnleiting.top/gtjwbxthsi.html

[U100] JS：DOM 查询
来源：http://hz.pengpengdd.cyou/gtzpojrsru.html

document.querySelector(".item")
来源：http://hz.52xcode.cn/gtmwfoqvow.html

[U101] JS：classList 操作
来源：http://hz.ppjwa.cn/gtwicdflpi.html

el.classList.toggle("active")
来源：http://hz.hammf.cn/gtbzawtjvj.html

[U102] JS：本地存储
来源：http://hz.bjfxy.top/gtevqqdapk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zycfv.cn/gtchfdvnrb.html

[U103] JS：定时器
来源：http://hz.jyoumei.cn/gtxptcxjrb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.svipenyu.cn/gtzvkyfphk.html

[U104] JS：防抖
来源：http://hz.tanke756.top/gtvfaclezj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xingfuxueyuan.xyz/gtcclnknov.html

[U105] JS：节流
来源：http://hz.xinyue.icu/gtedxjtfgp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yangfankeji.com/gtvyvqarhv.html

[U106] JS：日期格式化
来源：http://hz.svipenyu.cn/gtcbvzruxe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.birdmap.top/gtgmvrpwbh.html

[U107] JS：数字千分位
来源：http://hz.xuetiantiany.cn/gtdewcnban.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.gaohongyu789.top/gtcrwjktmq.html

[U108] JS：随机整数
来源：http://hz.dianchejie.cn/gtedzdjeen.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.guannengcc.top/gtumjmkxjr.html

[U109] JS：数组分组
来源：http://hz.andypj.xyz/gtzfhthbak.html

Object.groupBy(arr, x => x.type)
来源：http://hz.zhoulong.xyz/gtdjwdywcm.html

[U110] JS：数组分块
来源：http://hz.tianlin.xyz/gtrunpxmit.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.dianchejie.cn/gtlfaghvnx.html

[U111] JS：对象转 Map
来源：http://hz.sweek.top/gtfxontvui.html

new Map(Object.entries(obj))
来源：http://hz.hongshengwenyu.top/gtamvcnpcs.html

[U112] JS：字符串补位
来源：http://hz.jiagoushi.top/gtwtofuwpf.html

"7".padStart(3, "0")
来源：http://hz.zdqjudy.top/gtglwjihod.html

[U113] JS：正则替换全部
来源：http://hz.yangfankeji.com/gtxnsgueig.html

s.replaceAll("a", "b")
来源：http://hz.ydzc1.top/gtefsapiuf.html

[U114] JS：JSON 深比较
来源：http://hz.hfpthk.cn/gtubyyhsgd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.quarkkingdee.top/gtbwkogqsr.html

[U115] JS：生成 UUID
来源：http://hz.yanxiufei.cn/gttakbewcy.html

crypto.randomUUID()
来源：http://hz.gzhubu.top/gtdgbfwohq.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.cucudq.cn/gtvlcpovxp.html

/** @param {string} name */ function f(name) {}
来源：http://hz.kuanghao11.cn/gtbqvfdmpj.html

[U117] JS：单元测试
来源：http://hz.chenjidiqi.icu/gtrfmgvagy.html

npm i -D vitest;  npx vitest
来源：http://hz.zhengqikj.top/gtrmiegspc.html

[U118] JS：开发服务器
来源：http://hz.shanyushiyangkeji.top/gttlfzfnes.html

npm i -D vite;  npx vite
来源：http://hz.316326.xyz/gtfeyggwaa.html

[U119] JS：生产构建
来源：http://hz.shanyushiyangkeji.top/gtruxiujfk.html

npx vite build
来源：http://hz.zhijiandao.cn/gtcjseexap.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jinyuanbaomall.cn/gtpgbtyyku.html

import.meta.env.VITE_API_URL
来源：http://hz.shanyushiyangtech.top/gtdcxcqber.html

================================================================================
来源：http://hz.ppjwa.cn/gtolimdbyb.html

统计汇总
来源：http://hz.daria6918.cn/gthwqgzrgz.html

================================================================================
来源：http://hz.mhx1999.top/gtsnfnvufq.html

按语言统计（条）：
来源：http://hz.wangshuangyany.cn/gtmtcmujjt.html

Python ......... 252
来源：http://hz.chenzaomai.com/gtsrbhllvk.html

PHP ............ 252
来源：http://hz.chenzaomai.com/gtojaqidwf.html

JavaScript ..... 252
来源：http://hz.pycfn.com/gtekortruj.html

TypeScript ..... 212
来源：http://hz.yj20258888.top/gtpyxbrryn.html

Java ........... 212
来源：http://hz.jianghu66.top/gtqrzbtnbh.html

Go ............. 212
来源：http://hz.pycfn.com/gtmlfjyzmh.html

Ruby ........... 212
来源：http://hz.zhiwuduotai.top/gtkhmuyvps.html

C# ............. 212
来源：http://hz.vqdsnc.cn/gtywwbnljq.html

C .............. 30
来源：http://hz.nanxinkj.top/gtblqrdbiz.html

C++ ............ 30
来源：http://hz.gaohongyu789.top/gtgilctyur.html

SQL ............ 90
来源：http://hz.316326.xyz/gtbargqfbj.html

Bash ........... 80
来源：http://hz.zhixingplan.top/gtypuforvs.html

Kotlin ......... 15
来源：http://hz.gotoacloud.top/gtzuoqcbuk.html

Swift .......... 15
来源：http://hz.mhx1999.top/gtumvfumow.html

Lua ............ 10
来源：http://hz.xuetiantiany.cn/gthzdgdvnb.html

Perl ........... 10
来源：http://hz.dianchejie.cn/gtafefszdl.html

Scala .......... 10
来源：http://hz.tian-w.cn/gtmbhiwveg.html

------------------------------------
来源：http://hz.hysaishi.cn/gthybihawr.html

合计 ........... 2106 条
来源：http://hz.haohaochexian.top/gtbbevidqs.html

按章节统计：
来源：http://hz.sweek.top/gtmdwfrnqi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.tianlin.xyz/gtfaiczqju.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.xziqi.cn/gtctkfnjlz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.shzxlz.cn/gtkfpeaate.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jinqigufen.top/gtyftlatgh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.nwbrower.top/gtlragqjrv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yvedp.cn/gthmdkyxlq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.zhongyouzk.top/gtoyxlgsxk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.svipenyu.cn/gtpdhezgry.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yj202588.top/gtzlewjfpu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jqgfzy.top/gtqrczkzdl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yuxming.cn/gttwbctiio.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.smart0.xyz/gtywpwdyac.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jinyuanbaomall.cn/gtyyabidgz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yuanzhike.top/gtiudgmxaw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhaomingkeji.xyz/gtmhnqetqr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.shangyingyoupin.top/gtlfcppplb.html

Q SQL 专题                              90
来源：http://hz.gotoacloud.top/gtbtgrlrgt.html

R Bash 专题                             80
来源：http://hz.yongpay.top/gtkhzgxooz.html

S C / C++ 专题                          60
来源：http://hz.yj20258888.top/gtshrplxek.html

T 其他语言补充                          60
来源：http://hz.sxryk.cn/gtglwbyons.html

U 高频实用片段                         120
来源：http://hz.yanxiufei.cn/gtolzyhxyt.html

------------------------------------
来源：http://hz.zhaomingkeji.xyz/gtolfpjqss.html

合计                                  2106 条
来源：http://hz.chenlongwang.top/gteakeuwti.html

--------------------------------------------------------------------------------
来源：http://hz.sufxvd.cn/gthdykrbcz.html

使用提醒
来源：http://hz.sysykeji.top/gtirntjpjy.html

--------------------------------------------------------------------------------
来源：http://hz.ppjwa.cn/gtigmxadpj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.sxryk.cn/gtzozrpaaq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.xylfe.cn/gtyqybfxmq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yongpay.top/gtswmucfry.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.smart0.xyz/gtveumlidb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.mhx1999.top/gtezicwvky.html

—— 文件结束 ——
来源：http://hz.shzxlz.cn/gtezixomhw.html

================================================================================
来源：http://hz.snrcjt.cn/gtygrsfvqf.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jyoumei.cn/gtjavuwiwn.html

Common Programming Examples Cheat Book
来源：http://hz.shzxlz.cn/gtfiwjpsmb.html

================================================================================
来源：http://hz.fengsongda.top/gtryzvsake.html

【收录内容】
来源：http://hz.shanyushiyangtech.top/gtvkqmrjew.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.haohaochexian.top/gtwrxqhihw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.cashguo.top/gtelnllbji.html

SQL · Bash · C · C++
来源：http://hz.quarkkingdee.top/gtcrpnzwtb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.0kj1m.cn/gtymwpqvqn.html

【使用说明】
来源：http://hz.chenjidiqi.icu/gtcfrwmdlr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.tanke756.top/gtszpnvqke.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.bjfxy.top/gtsdyckplk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yuanzhike.top/gtcbvbnbzi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.gzhubu.top/gtpasmocvu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jinqigfzy.top/gtozlyhlmh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.xingfuxueyuan.xyz/gtqyakebdg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.wangshuangyany.cn/gtvmkbpdhl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yonumen.top/gtgerlkmyc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.zhongyouzk.top/gtfccztrke.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xuetiantiany.cn/gtclnvkfiv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.ydzc1.top/gtjpbogcgm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.hnxiangtu.top/gtsfeybhcf.html

【文件统计】
来源：http://hz.sweek.top/gtgkvichpr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.havefunace.top/gtmsegvwdc.html

--------------------------------------------------------------------------------
来源：http://hz.0kj1m.cn/gtjwpckxbg.html

目  录
来源：http://hz.tian-w.cn/gtmvtjbtmw.html

--------------------------------------------------------------------------------
来源：http://hz.yonumen.top/gtcmmxybzv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.xinyue.icu/gtofktnqwu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.nanxinkj.top/gtbwrwsuta.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.zhijiandao.cn/gtukzvycpv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.sxryk.cn/gtnpllivzl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.zhijiandao.cn/gthhqhhwmd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yvedp.cn/gtakkrqpzl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.c1oappe.top/gtqjzcvitn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yj20258.top/gtjnativjs.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.zhongyouzk.top/gtwmmjobyl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yj20258888.top/gtqwdezdyl.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.ehwqpu.com/gtiyumnujc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.zhiwuduotai.top/gtyifscffp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.yuxming.cn/gtdygmujvs.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.gaohongyu789.top/gtljboigml.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.52xcode.cn/gtvnqvdpkb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.mhx1999.top/gtnytfowcp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.shangyingyoupin.top/gtwpugcqiz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.quarkkingdee.top/gtlqbvyifn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yongpay.top/gtsvomtmnb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhengqikj.top/gtreckdbna.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.nwbrower.top/gtlokcqich.html

================================================================================
来源：http://hz.ybcxt.top/gtefdsywsl.html

A. 基础语法与类型
来源：http://hz.gogol.net.cn/gttpffnyzq.html

================================================================================
来源：http://hz.aibaodan.cn/gtriizejwr.html

[A01] Hello World
来源：http://hz.cqqwz.cn/gtyagmkcsr.html

Py:   print("Hello, World!")
来源：http://hz.nanxuanxn.top/gtzrbackhc.html

PHP:  echo "Hello, World!";
来源：http://hz.yj20258888.top/gtprcfaigg.html

JS:   console.log("Hello, World!");
来源：http://hz.shangyingyoupin.top/gtriwzgxjv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.aizwys.cn/gtljprqquk.html

Java: System.out.println("Hello, World!");
来源：http://hz.tianlin.xyz/gtmdnydche.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.xziqi.cn/gtwkqwzirt.html

Ruby: puts "Hello, World!"
来源：http://hz.hammf.cn/gtkvqxiqse.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.tian-w.cn/gtooovsaoc.html

[A02] 变量声明与赋值
来源：http://hz.tanke756.top/gtpghnpeyd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.nanxuanxn.top/gtuifttluj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.zycfv.cn/gtpxszkhct.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.sufxvd.cn/gtpwvrwaar.html


<!-- 参考信息 -->