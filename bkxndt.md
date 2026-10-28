代发 wailian999

[U33] Py：打包发布
来源：http://hz.pycfn.com/gtnumphlgy.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.sweek.top/gtrmmypllu.html

[U34] Py：判断编码
来源：http://hz.yangfankeji.com/gtffvqrxcm.html

chardet.detect(raw)
来源：http://hz.316326.xyz/gtoxnpzygq.html

[U35] Py：发送邮件
来源：http://hz.aibaodan.cn/gtzngwivdw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yongpay.top/gtzduaggfn.html

[U36] Py：定时任务
来源：http://hz.cqqwz.cn/gtlzjxltkj.html

schedule.every(10).minutes.do(job)
来源：http://hz.hnqzz.top/gtzphvnrdh.html

[U37] Py：读写 Excel
来源：http://hz.sysykeji.top/gtllmkcuoo.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.aibaodan.cn/gtpcaejmbi.html

[U38] Py：获取脚本所在目录
来源：http://hz.jqgfzy.top/gtdpwznaru.html

Path(__file__).resolve().parent
来源：http://hz.0kj1m.cn/gthqgygpvm.html

[U39] Py：判断是否在交互环境
来源：http://hz.snrcjt.cn/gtpvhipqgf.html

sys.stdout.isatty()
来源：http://hz.zhengqikj.top/gtwqmyaifq.html

[U40] Py：打印到标准错误
来源：http://hz.sufxvd.cn/gtajrfeteo.html

print("err", file=sys.stderr)
来源：http://hz.jqgfzy.top/gtkkzgynqc.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jinyuanbaomall.cn/gtdzibcjqt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hongshengwenyu.top/gtjmtchwox.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yj202588.top/gtsamvlsbd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.snrcjt.cn/gtmrhvbmmv.html

[U43] PHP：声明命名空间
来源：http://hz.mhx1999.top/gtjhvodiyq.html

namespace App\Http;
来源：http://hz.jianghu66.top/gtwkvaeyje.html

[U44] PHP：开启严格类型
来源：http://hz.fengsongda.top/gtyrarcqlv.html

declare(strict_types=1);
来源：http://hz.yj202588.top/gtifohcllk.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ydjk.org.cn/gtrnrutuyv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhijiandao.cn/gtnebjppum.html

[U46] PHP：可空类型
来源：http://hz.zhengqikj.top/gthispnmvz.html

?string $name = null
来源：http://hz.cqqwz.cn/gtcvohvjtw.html

[U47] PHP：联合类型
来源：http://hz.xuanzx.com/gtwxdyqfjj.html

int|string $id
来源：http://hz.yangfankeji.com/gtxrijxrgl.html

[U48] PHP：纯枚举
来源：http://hz.chenzaomai.com/gtvkgdljee.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.hywenlv.cn/gtnimcuohj.html

[U49] PHP：只读属性
来源：http://hz.meibo888.top/gtfpqeyhqc.html

public readonly string $name
来源：http://hz.daria6918.cn/gtfobajnmg.html

[U50] PHP：构造器属性提升
来源：http://hz.cashguo.top/gtnsacdzaj.html

public function __construct(private int $id) {}
来源：http://hz.jqgfzy.top/gtjgnwscgw.html

[U51] PHP：数组解构
来源：http://hz.jianghu66.top/gtokzapirt.html

[$a, $b] = $arr;
来源：http://hz.chenlongwang.top/gtyvxxzyqf.html

[U52] PHP：箭头函数
来源：http://hz.ppjwa.cn/gtpsioxxxg.html

$double = fn($x) => $x * 2;
来源：http://hz.9152youxi.cn/gtxspjrdvg.html

[U53] PHP：空合并运算符
来源：http://hz.zhiwuduotai.top/gttqgucuyi.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhiwuduotai.top/gtnhjcknps.html

[U54] PHP：空安全调用
来源：http://hz.daria6918.cn/gtdeforuvl.html

$obj?->method()
来源：http://hz.iojbl.cn/gtxohcvwmi.html

[U55] PHP：match 表达式
来源：http://hz.guowangkeji.top/gtdpuaknos.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.nanxuanxn.top/gthfiirjaz.html

[U56] PHP：命名参数
来源：http://hz.ehwqpu.com/gtzdpfzxrd.html

f(a: 1, b: 2)
来源：http://hz.fzhhl.top/gtfsggbhix.html

[U57] PHP：字符串插值
来源：http://hz.hfpthk.cn/gtqrpkgjna.html

"值: {$a}"
来源：http://hz.wangshuangyany.cn/gtlvtmzyqi.html

[U58] PHP：数组三件套
来源：http://hz.jinqigfzy.top/gtmetxpqjm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.mhx1999.top/gtozmblyom.html

[U59] PHP：自定义排序
来源：http://hz.jlsjyb.cn/gtwkasmepg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.aibaodan.cn/gtdhxxbyma.html

[U60] PHP：JSON 编解码
来源：http://hz.zhiwuduotai.top/gtsdyeomhs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yj20258888.top/gtnohhkvfs.html

[U61] PHP：正则
来源：http://hz.birdmap.top/gtupuqnbkx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.shzxlz.cn/gtzvpnbhlh.html

[U62] PHP：日期对象
来源：http://hz.shzxlz.cn/gtqutyuyyf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.9152youxi.cn/gtrzhxnqln.html

[U63] PHP：文件读写
来源：http://hz.shangyingyoupin.top/gtzptpzkpq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.haohaochexian.top/gtiyvyaabo.html

[U64] PHP：目录遍历
来源：http://hz.mhx1999.top/gtvpykxbgw.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.wangshuangyany.cn/gtrqjuqiad.html

[U65] PHP：会话
来源：http://hz.sxryk.cn/gtyftbelpw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.gotoacloud.top/gtipumzmwx.html

[U66] PHP：设置 Cookie
来源：http://hz.52xcode.cn/gtxyltjxbz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.chenzaomai.com/gtnwauqewe.html

[U67] PHP：处理文件上传
来源：http://hz.sufxvd.cn/gtchnznlgj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.nanxinkj.top/gtqkagtpid.html

[U68] PHP：PDO 连接
来源：http://hz.sweek.top/gtubcklaxn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.guannengcc.top/gtyovcgukk.html

[U69] PHP：PDO 预处理
来源：http://hz.xuanzx.com/gtujgmjjbq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jinyuanbaomall.cn/gtgiqxlrxh.html

[U70] PHP：PDO 事务
来源：http://hz.smart0.xyz/gtysfjtyen.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.shanyushiyangtech.top/gtqvdpiifb.html

[U71] PHP：抛出异常
来源：http://hz.chenjidiqi.icu/gtdstebwsn.html

throw new RuntimeException("失败", 500);
来源：http://hz.jqgufenzy.top/gtakkfcoit.html

[U72] PHP：写错误日志
来源：http://hz.aibaodan.cn/gtrjlvnqqq.html

error_log("失败: " . $e->getMessage());
来源：http://hz.tianlin.xyz/gtyffiqkiv.html

[U73] PHP：读取 ini 配置
来源：http://hz.chenlongwang.top/gtdpgjmkrv.html

parse_ini_file("config.ini", true)
来源：http://hz.tianlin.xyz/gtgekbsnnw.html

[U74] PHP：读取环境变量
来源：http://hz.ivvv.top/gtddrerwzu.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zhaomingkeji.xyz/gteeuurjhf.html

[U75] PHP：依赖注入
来源：http://hz.hysaishi.cn/gtgljnwsur.html

composer require psr/container
来源：http://hz.xziqi.cn/gtewqjrssu.html

[U76] PHP：简单路由
来源：http://hz.gotoacloud.top/gtfdxooxxl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jiagoushi.top/gtaomgsfil.html

[U77] PHP：模板渲染
来源：http://hz.cucudq.cn/gtlsjlqokh.html

composer require twig/twig
来源：http://hz.pycfn.com/gtamcaarbv.html

[U78] PHP：单元测试
来源：http://hz.fengsongda.top/gtrohoovqv.html

composer require --dev phpunit/phpunit
来源：http://hz.gaohongyu789.top/gtjdiktjzg.html

[U79] PHP：静态分析
来源：http://hz.xingfuxueyuan.xyz/gtwdxrswkl.html

composer require --dev phpstan/phpstan
来源：http://hz.jinqigfzy.top/gtpdqeixpe.html

[U80] PHP：代码规范修复
来源：http://hz.hnqzz.top/gtanmeoops.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.iojbl.cn/gtpuowdigt.html

[U81] JS：初始化项目
来源：http://hz.yongpay.top/gtfotjyphd.html

npm init -y;  npm i express
来源：http://hz.yanxiufei.cn/gthnpmcrrd.html

[U82] JS：package.json 脚本
来源：http://hz.xuanzx.com/gtowqczuac.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.iojbl.cn/gthsvxiojc.html

[U83] JS：ES Module 导入导出
来源：http://hz.xuetiantiany.cn/gtcynbnvzy.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.gaohongyu789.top/gtvwflcjxq.html

[U84] JS：CommonJS 写法
来源：http://hz.haohaochexian.top/gtwjcysdcv.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zhaomingkeji.xyz/gtzlfbshsg.html

[U85] JS：可选链
来源：http://hz.fengsongda.top/gtcrkhwsmb.html

a?.b?.c
来源：http://hz.zhijiandao.cn/gtqsadjjrm.html

[U86] JS：空值合并
来源：http://hz.redwolf501.top/gtgrujuqxs.html

a ?? b
来源：http://hz.ppjwa.cn/gtviyorhvv.html

[U87] JS：解构默认值
来源：http://hz.pycfn.com/gtgbfaualf.html

const { a = 1, b = 2 } = obj;
来源：http://hz.tianlin.xyz/gtxjhjciyk.html

[U88] JS：对象展开合并
来源：http://hz.cdnleiting.top/gtwnmbqgkm.html

{ ...a, ...b }
来源：http://hz.cashguo.top/gthbhtwspc.html

[U89] JS：数组去重
来源：http://hz.jlsjyb.cn/gtfdfeadat.html

[...new Set(arr)]
来源：http://hz.ywan-chungtsiang.top/gtowigcndo.html

[U90] JS：数字数组排序
来源：http://hz.tian-w.cn/gtzadgafkg.html

[...arr].sort((a, b) => a - b)
来源：http://hz.chenlongwang.top/gtafxeafwr.html

[U91] JS：对象键值遍历
来源：http://hz.zycfv.cn/gtcsmcumqo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.andypj.xyz/gtsczvkhxb.html

[U92] JS：深拷贝
来源：http://hz.birdmap.top/gtwaegkyzr.html

structuredClone(obj)
来源：http://hz.bjfxy.top/gtuvsweswu.html

[U93] JS：模板字符串
来源：http://hz.ydjk.org.cn/gtjsewtgub.html

`共 ${n} 条`
来源：http://hz.chenzaomai.com/gtrwipfgcb.html

[U94] JS：箭头函数
来源：http://hz.yueranfly.top/gtdsywufib.html

const double = x => x * 2;
来源：http://hz.ydzc1.top/gtgxghifgm.html

[U95] JS：Promise 包装
来源：http://hz.nanxuanxn.top/gtecjixcio.html

new Promise((resolve, reject) => {})
来源：http://hz.fengsongda.top/gtkemzyqip.html

[U96] JS：async/await 与异常
来源：http://hz.tanke756.top/gtexnpvemm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.pycfn.com/gtzwqalwtv.html

[U97] JS：并发请求
来源：http://hz.gogol.net.cn/gtcdmrjptj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hammf.cn/gtiiytuvio.html

[U98] JS：fetch 带 JSON
来源：http://hz.yongpay.top/gtraevihck.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.jlsjyb.cn/gtdztrepju.html

[U99] JS：事件监听
来源：http://hz.jinghuilouyu.cn/gtfqkrlgkm.html

el.addEventListener("click", e => {})
来源：http://hz.yanxiufei.cn/gtzojzfsmy.html

[U100] JS：DOM 查询
来源：http://hz.ydjk.org.cn/gtvwyudxzt.html

document.querySelector(".item")
来源：http://hz.andypj.xyz/gtkpxbymnh.html

[U101] JS：classList 操作
来源：http://hz.guannengcc.top/gttgxpabbe.html

el.classList.toggle("active")
来源：http://hz.redwolf501.top/gthgdlbnnb.html

[U102] JS：本地存储
来源：http://hz.jlsjyb.cn/gtpsckemue.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.52xcode.cn/gtzzxddqgb.html

[U103] JS：定时器
来源：http://hz.tian-w.cn/gteunreikr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.daria6918.cn/gtipkutjhj.html

[U104] JS：防抖
来源：http://hz.gotoacloud.top/gtgmznzlfq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sysykeji.top/gtaaxkbfis.html

[U105] JS：节流
来源：http://hz.andypj.xyz/gtmigauvqg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhixingplan.top/gtmxjatlwt.html

[U106] JS：日期格式化
来源：http://hz.52xcode.cn/gtivgpvcyk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.shuidangran.top/gthttopsiw.html

[U107] JS：数字千分位
来源：http://hz.wangdashe.top/gtybcshtdw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.shanyushiyangtech.top/gtmajrdxia.html

[U108] JS：随机整数
来源：http://hz.fengsongda.top/gtyskcmeae.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.mhx1999.top/gtlwhkgxhu.html

[U109] JS：数组分组
来源：http://hz.shanyushiyangtech.top/gtvyjisish.html

Object.groupBy(arr, x => x.type)
来源：http://hz.fzhhl.top/gtdbodbqfc.html

[U110] JS：数组分块
来源：http://hz.haohaochexian.top/gtsntrahpk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.gogol.net.cn/gtondagmce.html

[U111] JS：对象转 Map
来源：http://hz.sysykeji.top/gtmlepetak.html

new Map(Object.entries(obj))
来源：http://hz.xylfe.cn/gtfcvxqmoe.html

[U112] JS：字符串补位
来源：http://hz.cucudq.cn/gtyxhxikbs.html

"7".padStart(3, "0")
来源：http://hz.ehwqpu.com/gtywvsqiwy.html

[U113] JS：正则替换全部
来源：http://hz.c1oappe.top/gtfvpfrdqj.html

s.replaceAll("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtumagzlrj.html

[U114] JS：JSON 深比较
来源：http://hz.yj202588.top/gtfxzuvqaq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.pycfn.com/gtrynqlxki.html

[U115] JS：生成 UUID
来源：http://hz.fzhhl.top/gtbyjdtlsf.html

crypto.randomUUID()
来源：http://hz.pycfn.com/gthujexmam.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hammf.cn/gtktyasiza.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jinqigfzy.top/gtinpjgipx.html

[U117] JS：单元测试
来源：http://hz.mhx1999.top/gtwrsmickj.html

npm i -D vitest;  npx vitest
来源：http://hz.snrcjt.cn/gtukbdtsge.html

[U118] JS：开发服务器
来源：http://hz.quarkkingdee.top/gtcyegwckp.html

npm i -D vite;  npx vite
来源：http://hz.shanyushiyangtech.top/gtgaqqcirt.html

[U119] JS：生产构建
来源：http://hz.shanyushiyangtech.top/gtemtlisdr.html

npx vite build
来源：http://hz.zhixingplan.top/gtnzbrhlvs.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.cdnleiting.top/gtusduwafu.html

import.meta.env.VITE_API_URL
来源：http://hz.cqqwz.cn/gtzcbjhvzm.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtsrtsikgn.html

统计汇总
来源：http://hz.gaohongyu789.top/gtovfivzdd.html

================================================================================
来源：http://hz.hammf.cn/gtfhrwmcas.html

按语言统计（条）：
来源：http://hz.fzhhl.top/gtjdamgekg.html

Python ......... 252
来源：http://hz.cashguo.top/gtreywtenq.html

PHP ............ 252
来源：http://hz.yuxming.cn/gtputajnji.html

JavaScript ..... 252
来源：http://hz.jyoumei.cn/gtgaueksup.html

TypeScript ..... 212
来源：http://hz.zhixingplan.top/gtcyzcfjlf.html

Java ........... 212
来源：http://hz.nanxinkj.top/gtmcvueuxh.html

Go ............. 212
来源：http://hz.bjfxy.top/gthnyuckfo.html

Ruby ........... 212
来源：http://hz.snrcjt.cn/gtsipxwhhr.html

C# ............. 212
来源：http://hz.yangfankeji.com/gtrcatvopy.html

C .............. 30
来源：http://hz.daxiang520.top/gtwnqiyqrl.html

C++ ............ 30
来源：http://hz.shzxlz.cn/gtvjkazuqn.html

SQL ............ 90
来源：http://hz.pengpengdd.cyou/gtnnojflen.html

Bash ........... 80
来源：http://hz.dashuyun.cn/gtpqozphjc.html

Kotlin ......... 15
来源：http://hz.shzxlz.cn/gtujimyxdj.html

Swift .......... 15
来源：http://hz.shzxlz.cn/gtaotimeer.html

Lua ............ 10
来源：http://hz.shanyushiyangtech.top/gtmsgkxioq.html

Perl ........... 10
来源：http://hz.shanyushiyangkeji.top/gtnamrpjqq.html

Scala .......... 10
来源：http://hz.gzhubu.top/gtlqchyath.html

------------------------------------
来源：http://hz.quarkkingdee.top/gtrubqsmwd.html

合计 ........... 2106 条
来源：http://hz.hnxiangtu.top/gtiibffmnt.html

按章节统计：
来源：http://hz.yanxiufei.cn/gtimbcnznm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.snrcjt.cn/gtfmnkicig.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hnxiangtu.top/gtqlsnfkfn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.gogol.net.cn/gtnuhxqagk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yj20258.top/gtkvqlkiis.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.chenjidiqi.icu/gtlkfviwgx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.gotoacloud.top/gtqpmogjyk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.shangyingyoupin.top/gtvkxvefdb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ppjwa.cn/gtllxxcusi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.birdmap.top/gtbkbfbgmr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ybcxt.top/gtgviiimzd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.ppjwa.cn/gtwmabwolz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.tian-w.cn/gtzdyzjajb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.vqdsnc.cn/gtyeckxcps.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.gogol.net.cn/gtzsosnmbi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jiagoushi.top/gtrzbrvrzi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.gzhubu.top/gtlftqxvuc.html

Q SQL 专题                              90
来源：http://hz.zdqjudy.top/gtakaiovpn.html

R Bash 专题                             80
来源：http://hz.havefunace.top/gtskpyaofy.html

S C / C++ 专题                          60
来源：http://hz.xingfuxueyuan.xyz/gtkgviliiv.html

T 其他语言补充                          60
来源：http://hz.daria6918.cn/gtbfjiynuj.html

U 高频实用片段                         120
来源：http://hz.shanyushiyangtech.top/gtdovktika.html

------------------------------------
来源：http://hz.zhongyouzk.top/gtwarvwquo.html

合计                                  2106 条
来源：http://hz.zhoulong.xyz/gtoimmbkdc.html

--------------------------------------------------------------------------------
来源：http://hz.hysaishi.cn/gtfrvcpcxp.html

使用提醒
来源：http://hz.52xcode.cn/gtrbnpgbsa.html

--------------------------------------------------------------------------------
来源：http://hz.tianlin.xyz/gtbysxynzq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.shangyingyoupin.top/gtqlutiyvk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.aizwys.cn/gtbqdmcqtd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.cheryme.top/gtkjwqhmue.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.tian-w.cn/gtzblmpydi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhoulong.xyz/gtdgioyswf.html

—— 文件结束 ——
来源：http://hz.wangshuangyany.cn/gtxwgfglao.html

================================================================================
来源：http://hz.kuanghao11.cn/gtcwnliiyl.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.hfpthk.cn/gtszsnmpzn.html

Common Programming Examples Cheat Book
来源：http://hz.wangdashe.top/gtteldllgp.html

================================================================================
来源：http://hz.birdmap.top/gtrsobugjv.html

【收录内容】
来源：http://hz.daria6918.cn/gtcyidiysw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zdqjudy.top/gtaxfflhsj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yj20258888.top/gteueosgmo.html

SQL · Bash · C · C++
来源：http://hz.ivvv.top/gtetyknwdq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.9152youxi.cn/gtrvthfdyf.html

【使用说明】
来源：http://hz.kuanghao11.cn/gthximrxfr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hnqzz.top/gtysgxzkyn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.daria6918.cn/gtvstvitkx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zhaomingkeji.xyz/gticoqcheh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yanxiufei.cn/gttuepkxuh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yj20258.top/gttwdxzvih.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.cheryme.top/gtgxsotslq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.wangshuangyany.cn/gtrxlqkwcp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.smart0.xyz/gtnfezsafq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.ywan-chungtsiang.top/gtmfsvyiuu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yuxming.cn/gtolqalchb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.shuidangran.top/gtbhtookqn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.xuanzx.com/gtnfgrncmc.html

【文件统计】
来源：http://hz.sweek.top/gtdgjbahow.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.sweek.top/gtibcowrlr.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangtech.top/gtvnzbkhsv.html

目  录
来源：http://hz.bjfxy.top/gtjoecbfbb.html

--------------------------------------------------------------------------------
来源：http://hz.pengpengdd.cyou/gtliatefbc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.feifeiyinyue.top/gtjxxmvahy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.guowangkeji.top/gtsjkbbrar.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.pycfn.com/gtgadjyhxi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.dianchejie.cn/gtwtxupowj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yuxming.cn/gttjvdqkdg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.ivvv.top/gtvrznanog.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.xuetiantiany.cn/gtparsxcmx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.cashguo.top/gtpfxyqalm.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.haohaochexian.top/gtizbjmuyu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.shzxlz.cn/gtxfengdki.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jinyuanbaomall.cn/gtysixkcsd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.cashguo.top/gtftohpgtd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.yj202588.top/gtkwutpgly.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.snrcjt.cn/gtqytdkohg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.xylfe.cn/gtoyjnukix.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.redwolf501.top/gtnzzbheha.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.hongshengwenyu.top/gtanwnogtw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.zhengqikj.top/gtrxipmiqo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.dianchejie.cn/gtjtxmcanh.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yuxming.cn/gtmsyaskqc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.vqdsnc.cn/gtvuslbbjr.html

================================================================================
来源：http://hz.fengsongda.top/gtrvhpfacu.html

A. 基础语法与类型
来源：http://hz.xylfe.cn/gtassfazcp.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtkamaqaqf.html

[A01] Hello World
来源：http://hz.zhijiandao.cn/gtnuxneqxi.html

Py:   print("Hello, World!")
来源：http://hz.hnqzz.top/gtsiypluog.html

PHP:  echo "Hello, World!";
来源：http://hz.smart0.xyz/gtbtrecyiz.html

JS:   console.log("Hello, World!");
来源：http://hz.kuanghao11.cn/gtfcllohlk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yvedp.cn/gtuongjlzs.html

Java: System.out.println("Hello, World!");
来源：http://hz.shangyingyoupin.top/gtqzeggqpi.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.hywenlv.cn/gtevwdawip.html

Ruby: puts "Hello, World!"
来源：http://hz.chenjidiqi.icu/gtiplvndcb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.xuanzx.com/gtyzzdyazo.html

[A02] 变量声明与赋值
来源：http://hz.jinqigufen.top/gtvjqiymqt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.sufxvd.cn/gtbggdfzie.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.0kj1m.cn/gtsadunspw.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.svipenyu.cn/gtlxwyabsr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.cucudq.cn/gtapbsjfrc.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.zdqjudy.top/gtxsslvaqi.html

Go:   name := "Alex"; age := 20
来源：http://hz.jinyuanbaomall.cn/gtmszeojio.html

Ruby: name = "Alex"; age = 20
来源：http://hz.xuanzx.com/gtxbdivkzr.html


<!-- 参考信息 -->