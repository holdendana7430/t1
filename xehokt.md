代发 wailian999

[U29] Py：属性校验
来源：http://hz.shanyushiyangkeji.top/gtqqyfmxwh.html

@property 与 @x.setter 配合
来源：http://hz.hnqzz.top/gtyzrxxfso.html

[U30] Py：数据类
来源：http://hz.dianchejie.cn/gtkgcbhalp.html

@dataclass(slots=True)
来源：http://hz.daria6918.cn/gtftwxcrux.html

[U31] Py：单测
来源：http://hz.shuidangran.top/gtcyclxnur.html

python -m pytest -q
来源：http://hz.gzhubu.top/gthjnppzdo.html

[U32] Py：代码格式化
来源：http://hz.zhoulong.xyz/gtozuyxwge.html

ruff format . && ruff check --fix .
来源：http://hz.c1oappe.top/gtxwwxffem.html

[U33] Py：打包发布
来源：http://hz.zhoulong.xyz/gtnjvpvlkx.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.xingfuxueyuan.xyz/gtxagrntwj.html

[U34] Py：判断编码
来源：http://hz.gaohongyu789.top/gtniawytgr.html

chardet.detect(raw)
来源：http://hz.xuetiantiany.cn/gtrqyuaair.html

[U35] Py：发送邮件
来源：http://hz.pengpengdd.cyou/gtioudawus.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.mhx1999.top/gtiuqxfzwc.html

[U36] Py：定时任务
来源：http://hz.hfpthk.cn/gtjtwextus.html

schedule.every(10).minutes.do(job)
来源：http://hz.zycfv.cn/gtrgavkenp.html

[U37] Py：读写 Excel
来源：http://hz.shangyingyoupin.top/gtgunxzegq.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhixingplan.top/gtvklviimc.html

[U38] Py：获取脚本所在目录
来源：http://hz.ppjwa.cn/gtqbqyicgl.html

Path(__file__).resolve().parent
来源：http://hz.havefunace.top/gtaslfotmu.html

[U39] Py：判断是否在交互环境
来源：http://hz.bjfxy.top/gtufovgitd.html

sys.stdout.isatty()
来源：http://hz.ppjwa.cn/gtkszbcepk.html

[U40] Py：打印到标准错误
来源：http://hz.zhijiandao.cn/gtxggtnbvj.html

print("err", file=sys.stderr)
来源：http://hz.gaohongyu789.top/gtuftaaddp.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.cheryme.top/gtvxdjbtrx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.quarkkingdee.top/gtakyyubpi.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.gogol.net.cn/gthonokjpr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.pycfn.com/gtydfuoabn.html

[U43] PHP：声明命名空间
来源：http://hz.guannengcc.top/gttidudxtl.html

namespace App\Http;
来源：http://hz.ydzc1.top/gtkqbbfozu.html

[U44] PHP：开启严格类型
来源：http://hz.shanyushiyangtech.top/gtlxqbpcit.html

declare(strict_types=1);
来源：http://hz.daxiang520.top/gtevujreae.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yuanzhike.top/gtbhsyfwhg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinqigufen.top/gtohzulozg.html

[U46] PHP：可空类型
来源：http://hz.cqqwz.cn/gtrvuoavvk.html

?string $name = null
来源：http://hz.shangyingyoupin.top/gtcbvoxkij.html

[U47] PHP：联合类型
来源：http://hz.0kj1m.cn/gtjuhvropi.html

int|string $id
来源：http://hz.zhiwuduotai.top/gtujvusidi.html

[U48] PHP：纯枚举
来源：http://hz.zdqjudy.top/gtxmghtplt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.pycfn.com/gtsukpbrtv.html

[U49] PHP：只读属性
来源：http://hz.nanxuanxn.top/gtmrbwlbgj.html

public readonly string $name
来源：http://hz.bjfxy.top/gtpjrhhidf.html

[U50] PHP：构造器属性提升
来源：http://hz.daxiang520.top/gtqxzmivxm.html

public function __construct(private int $id) {}
来源：http://hz.xinyue.icu/gtngmytavw.html

[U51] PHP：数组解构
来源：http://hz.xziqi.cn/gtlwletjwo.html

[$a, $b] = $arr;
来源：http://hz.316326.xyz/gttdzptkzi.html

[U52] PHP：箭头函数
来源：http://hz.daxiang520.top/gtqliuqgcl.html

$double = fn($x) => $x * 2;
来源：http://hz.wangshuangyany.cn/gtomplywzw.html

[U53] PHP：空合并运算符
来源：http://hz.smart0.xyz/gtmforneji.html

$v = $a ?? $b ?? "default";
来源：http://hz.shanyushiyangkeji.top/gtoiihudqj.html

[U54] PHP：空安全调用
来源：http://hz.daxiang520.top/gtxavbwccf.html

$obj?->method()
来源：http://hz.tanke756.top/gtnxyzqrqk.html

[U55] PHP：match 表达式
来源：http://hz.guowangkeji.top/gtvarfsbdx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jqgfzy.top/gtbobohrqc.html

[U56] PHP：命名参数
来源：http://hz.52xcode.cn/gtwdjsiwnr.html

f(a: 1, b: 2)
来源：http://hz.chenjidiqi.icu/gtdamyafui.html

[U57] PHP：字符串插值
来源：http://hz.jlsjyb.cn/gtspgbupws.html

"值: {$a}"
来源：http://hz.ydzc1.top/gtfqgaefrb.html

[U58] PHP：数组三件套
来源：http://hz.hnxiangtu.top/gtocviagel.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yanxiufei.cn/gtfvomorop.html

[U59] PHP：自定义排序
来源：http://hz.jiagoushi.top/gtaafjraez.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shzxlz.cn/gtikczaiid.html

[U60] PHP：JSON 编解码
来源：http://hz.redwolf501.top/gtmpornosv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.hysaishi.cn/gtfkdfyeea.html

[U61] PHP：正则
来源：http://hz.zycfv.cn/gtvsrhzujs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.daxiang520.top/gtozicicow.html

[U62] PHP：日期对象
来源：http://hz.yj20258888.top/gttbomrqfg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.pycfn.com/gtrnopwdsh.html

[U63] PHP：文件读写
来源：http://hz.hysaishi.cn/gttrmtruca.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.hnqzz.top/gtvpqlyyrk.html

[U64] PHP：目录遍历
来源：http://hz.jinqigufen.top/gtczobdivb.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.quarkkingdee.top/gtisrgmiai.html

[U65] PHP：会话
来源：http://hz.jinyuanbaomall.cn/gtbhvlenrk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.xuetiantiany.cn/gttrejgluk.html

[U66] PHP：设置 Cookie
来源：http://hz.nwbrower.top/gtwmrhupvt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.hnqzz.top/gtlgqaunuq.html

[U67] PHP：处理文件上传
来源：http://hz.cdnleiting.top/gteshtqerv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.shangyingyoupin.top/gtpikhayzu.html

[U68] PHP：PDO 连接
来源：http://hz.gogol.net.cn/gtchvrnqwe.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.gotoacloud.top/gtdfrprzxw.html

[U69] PHP：PDO 预处理
来源：http://hz.c1oappe.top/gtrozomczr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.tianlin.xyz/gtgkxxmstp.html

[U70] PHP：PDO 事务
来源：http://hz.hysaishi.cn/gtektpcoho.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.ywan-chungtsiang.top/gtylqmonuu.html

[U71] PHP：抛出异常
来源：http://hz.gaohongyu789.top/gtkhcnixws.html

throw new RuntimeException("失败", 500);
来源：http://hz.dianchejie.cn/gtziljdqta.html

[U72] PHP：写错误日志
来源：http://hz.yuxming.cn/gtxufpnuts.html

error_log("失败: " . $e->getMessage());
来源：http://hz.iojbl.cn/gtqcusvpmp.html

[U73] PHP：读取 ini 配置
来源：http://hz.dianchejie.cn/gtfzibblbm.html

parse_ini_file("config.ini", true)
来源：http://hz.nanxuanxn.top/gtjpqmvnpu.html

[U74] PHP：读取环境变量
来源：http://hz.yonumen.top/gtvwfntcmp.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hfpthk.cn/gtrzotqeiq.html

[U75] PHP：依赖注入
来源：http://hz.jinqigufen.top/gtamardsfe.html

composer require psr/container
来源：http://hz.yuxming.cn/gtltquyyeu.html

[U76] PHP：简单路由
来源：http://hz.jinghuilouyu.cn/gtrdlunthj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zhengqikj.top/gtgtczmlha.html

[U77] PHP：模板渲染
来源：http://hz.snrcjt.cn/gtlrjyfktq.html

composer require twig/twig
来源：http://hz.gotoacloud.top/gtaaphrbhb.html

[U78] PHP：单元测试
来源：http://hz.cdnleiting.top/gtsydbmybn.html

composer require --dev phpunit/phpunit
来源：http://hz.haohaochexian.top/gtigiijkkm.html

[U79] PHP：静态分析
来源：http://hz.mhx1999.top/gtlmfcffoq.html

composer require --dev phpstan/phpstan
来源：http://hz.nanxuanxn.top/gtkunmokys.html

[U80] PHP：代码规范修复
来源：http://hz.ydzc1.top/gtcyifagvu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yongpay.top/gtlirhlzif.html

[U81] JS：初始化项目
来源：http://hz.yj20258.top/gtqtwzkomf.html

npm init -y;  npm i express
来源：http://hz.gaohongyu789.top/gtdllllyka.html

[U82] JS：package.json 脚本
来源：http://hz.0kj1m.cn/gtgxovutmi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.nanxuanxn.top/gtvwwmdsyc.html

[U83] JS：ES Module 导入导出
来源：http://hz.yangfankeji.com/gtikjpwsvw.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.jiagoushi.top/gtahfrgwzy.html

[U84] JS：CommonJS 写法
来源：http://hz.sufxvd.cn/gtmkxyixza.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zhoulong.xyz/gtljbqmgyp.html

[U85] JS：可选链
来源：http://hz.jyoumei.cn/gteybqfkcz.html

a?.b?.c
来源：http://hz.hnqzz.top/gtmezfvtha.html

[U86] JS：空值合并
来源：http://hz.yonumen.top/gtjodvssaw.html

a ?? b
来源：http://hz.nanxinkj.top/gtbunvxllc.html

[U87] JS：解构默认值
来源：http://hz.yangfankeji.com/gtjfkscbah.html

const { a = 1, b = 2 } = obj;
来源：http://hz.9152youxi.cn/gtahdtmptq.html

[U88] JS：对象展开合并
来源：http://hz.gogol.net.cn/gttuwxyple.html

{ ...a, ...b }
来源：http://hz.0kj1m.cn/gtdjsaqway.html

[U89] JS：数组去重
来源：http://hz.jiagoushi.top/gtpbhmiwbq.html

[...new Set(arr)]
来源：http://hz.yangfankeji.com/gtfluucmav.html

[U90] JS：数字数组排序
来源：http://hz.snrcjt.cn/gtumnpkxcd.html

[...arr].sort((a, b) => a - b)
来源：http://hz.52xcode.cn/gtcxkacbzv.html

[U91] JS：对象键值遍历
来源：http://hz.ehwqpu.com/gtafbajihi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.sufxvd.cn/gtdwbziyjp.html

[U92] JS：深拷贝
来源：http://hz.cqqwz.cn/gtokqtkfic.html

structuredClone(obj)
来源：http://hz.vqdsnc.cn/gtfhcktkro.html

[U93] JS：模板字符串
来源：http://hz.tianlin.xyz/gtuheamnkf.html

`共 ${n} 条`
来源：http://hz.kuanghao11.cn/gtdtqapmqy.html

[U94] JS：箭头函数
来源：http://hz.guannengcc.top/gthjheogfd.html

const double = x => x * 2;
来源：http://hz.chenjidiqi.icu/gtawbilxuu.html

[U95] JS：Promise 包装
来源：http://hz.hnqzz.top/gttczkflsb.html

new Promise((resolve, reject) => {})
来源：http://hz.jinghuilouyu.cn/gtwzpktees.html

[U96] JS：async/await 与异常
来源：http://hz.quarkkingdee.top/gteuyohlbn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.pycfn.com/gthprngwvu.html

[U97] JS：并发请求
来源：http://hz.pycfn.com/gtgekqpser.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtlorsdiok.html

[U98] JS：fetch 带 JSON
来源：http://hz.wangdashe.top/gtuyrzhdsn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.guannengcc.top/gtjkdyljty.html

[U99] JS：事件监听
来源：http://hz.yj20258888.top/gtnkcnjcmc.html

el.addEventListener("click", e => {})
来源：http://hz.yueranfly.top/gtflwipklm.html

[U100] JS：DOM 查询
来源：http://hz.chenzaomai.com/gtbcbkzcfo.html

document.querySelector(".item")
来源：http://hz.yongpay.top/gtenytopry.html

[U101] JS：classList 操作
来源：http://hz.hnxiangtu.top/gtseshsoes.html

el.classList.toggle("active")
来源：http://hz.zhengqikj.top/gtbwrarcmc.html

[U102] JS：本地存储
来源：http://hz.yuanzhike.top/gtsqnyhrjr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.sxryk.cn/gtzcbwweqx.html

[U103] JS：定时器
来源：http://hz.ydjk.org.cn/gtbqfxirwn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.shzxlz.cn/gtpzhcklxp.html

[U104] JS：防抖
来源：http://hz.hnxiangtu.top/gtoudndaci.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guowangkeji.top/gtezuiuqxp.html

[U105] JS：节流
来源：http://hz.yvedp.cn/gtxqybklqz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.vqdsnc.cn/gtdxcrjksw.html

[U106] JS：日期格式化
来源：http://hz.ydjk.org.cn/gtjrhffzgw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.hnqzz.top/gtqbunmhso.html

[U107] JS：数字千分位
来源：http://hz.316326.xyz/gtllxnsnqp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yuxming.cn/gtbdmqwxog.html

[U108] JS：随机整数
来源：http://hz.hysaishi.cn/gtsqpnkabu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jqgufenzy.top/gtqvupynxd.html

[U109] JS：数组分组
来源：http://hz.jiagoushi.top/gtgiuvvfuc.html

Object.groupBy(arr, x => x.type)
来源：http://hz.tianlin.xyz/gttuwuawqh.html

[U110] JS：数组分块
来源：http://hz.chenjidiqi.icu/gtfgaqdkmo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.52xcode.cn/gtefkjpuol.html

[U111] JS：对象转 Map
来源：http://hz.zdqjudy.top/gtwsicugcv.html

new Map(Object.entries(obj))
来源：http://hz.jiagoushi.top/gtaptfphqx.html

[U112] JS：字符串补位
来源：http://hz.dashuyun.cn/gtslaciduz.html

"7".padStart(3, "0")
来源：http://hz.hammf.cn/gtqtzdlqzn.html

[U113] JS：正则替换全部
来源：http://hz.redwolf501.top/gtatnjwysc.html

s.replaceAll("a", "b")
来源：http://hz.ehwqpu.com/gtdvovtslu.html

[U114] JS：JSON 深比较
来源：http://hz.jiagoushi.top/gtdjdsdvoe.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sysykeji.top/gtmgjdobhw.html

[U115] JS：生成 UUID
来源：http://hz.guannengcc.top/gtetunytkf.html

crypto.randomUUID()
来源：http://hz.xylfe.cn/gtcorhsehi.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jlsjyb.cn/gtyfrybtsr.html

/** @param {string} name */ function f(name) {}
来源：http://hz.hongshengwenyu.top/gtutilggnu.html

[U117] JS：单元测试
来源：http://hz.redwolf501.top/gtlnzuinhg.html

npm i -D vitest;  npx vitest
来源：http://hz.jqgfzy.top/gtxubtrymu.html

[U118] JS：开发服务器
来源：http://hz.zhijiandao.cn/gtqnxxoctr.html

npm i -D vite;  npx vite
来源：http://hz.jinqigufen.top/gtunitaayw.html

[U119] JS：生产构建
来源：http://hz.yueranfly.top/gtrqgqgxjm.html

npx vite build
来源：http://hz.yuxming.cn/gtlzixnnok.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.sweek.top/gtdrlswtko.html

import.meta.env.VITE_API_URL
来源：http://hz.fzhhl.top/gtywrhqnuc.html

================================================================================
来源：http://hz.tianlin.xyz/gtqbckekln.html

统计汇总
来源：http://hz.hnxiangtu.top/gtayddflqn.html

================================================================================
来源：http://hz.hammf.cn/gttfivlsyr.html

按语言统计（条）：
来源：http://hz.sxryk.cn/gtuodznpko.html

Python ......... 252
来源：http://hz.sysykeji.top/gtnxhdgdtr.html

PHP ............ 252
来源：http://hz.52xcode.cn/gtljtkhxzg.html

JavaScript ..... 252
来源：http://hz.kuanghao11.cn/gtlmiecxif.html

TypeScript ..... 212
来源：http://hz.shangyingyoupin.top/gtcgpctjmr.html

Java ........... 212
来源：http://hz.gzhubu.top/gtfpzqzrqm.html

Go ............. 212
来源：http://hz.jinghuilouyu.cn/gtxvkatsyb.html

Ruby ........... 212
来源：http://hz.pycfn.com/gtgsthwvdm.html

C# ............. 212
来源：http://hz.yanxiufei.cn/gtztbzkwhh.html

C .............. 30
来源：http://hz.nanxuanxn.top/gtamvvzkgg.html

C++ ............ 30
来源：http://hz.yongpay.top/gtjcytsjae.html

SQL ............ 90
来源：http://hz.jqgufenzy.top/gtfenqexun.html

Bash ........... 80
来源：http://hz.52xcode.cn/gtaligemkk.html

Kotlin ......... 15
来源：http://hz.nwbrower.top/gtlcpmzyku.html

Swift .......... 15
来源：http://hz.cdnleiting.top/gtzjrieipb.html

Lua ............ 10
来源：http://hz.dianchejie.cn/gtqcjwjprt.html

Perl ........... 10
来源：http://hz.nanxinkj.top/gtdcgtukps.html

Scala .......... 10
来源：http://hz.c1oappe.top/gtdcwcfbns.html

------------------------------------
来源：http://hz.svipenyu.cn/gtsaoptwaf.html

合计 ........... 2106 条
来源：http://hz.snrcjt.cn/gtofkkowrl.html

按章节统计：
来源：http://hz.sweek.top/gtjxsmadrl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jyoumei.cn/gtvdsjnyri.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hnxiangtu.top/gtwqsmateo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jinqigfzy.top/gtqrexckrm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.bjfxy.top/gtgchxyzhm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.wangshuangyany.cn/gtjpewapcm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jinqigfzy.top/gtpjlfassq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.birdmap.top/gttwyvbhib.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yvedp.cn/gtcsptsech.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.9152youxi.cn/gtekwawcub.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.xziqi.cn/gtlejzjtqp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jyoumei.cn/gtoqdmnkte.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yanxiufei.cn/gtdoipmtfp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.cucudq.cn/gtptkphaxp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.sufxvd.cn/gtqeqqfswj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.0kj1m.cn/gtwmxsungw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.cheryme.top/gtdqwghozq.html

Q SQL 专题                              90
来源：http://hz.316326.xyz/gtarwhwcnd.html

R Bash 专题                             80
来源：http://hz.guowangkeji.top/gteeksiive.html

S C / C++ 专题                          60
来源：http://hz.ehwqpu.com/gtcbfajttb.html

T 其他语言补充                          60
来源：http://hz.tian-w.cn/gtqucgrzal.html

U 高频实用片段                         120
来源：http://hz.ydzc1.top/gtborekmtq.html

------------------------------------
来源：http://hz.cdnleiting.top/gtbaujxivv.html

合计                                  2106 条
来源：http://hz.cashguo.top/gtlysnjaqx.html

--------------------------------------------------------------------------------
来源：http://hz.andypj.xyz/gtwhqzdbgv.html

使用提醒
来源：http://hz.yanxiufei.cn/gtrzatqfhi.html

--------------------------------------------------------------------------------
来源：http://hz.zhijiandao.cn/gtygzjvawj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jinghuilouyu.cn/gtfhgcgpxv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yongpay.top/gtcgcjzemk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.jianghu66.top/gttryoesdl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yangfankeji.com/gtdymocviw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.ydzc1.top/gtypggooxn.html

—— 文件结束 ——
来源：http://hz.daxiang520.top/gtwwkhgdjv.html

================================================================================
来源：http://hz.yanxiufei.cn/gtahqjmajh.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yj20258888.top/gtgqhimcqy.html

Common Programming Examples Cheat Book
来源：http://hz.dianchejie.cn/gtgnwbmjar.html

================================================================================
来源：http://hz.kuanghao11.cn/gtqfakhtsk.html

【收录内容】
来源：http://hz.hnqzz.top/gtprxpsfkb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.cqqwz.cn/gtnmqujpod.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.0kj1m.cn/gtcwdtcqii.html

SQL · Bash · C · C++
来源：http://hz.cdnleiting.top/gtxlbgsbao.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.hysaishi.cn/gtjiwvphdy.html

【使用说明】
来源：http://hz.xuanzx.com/gtxntpkqjv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.redwolf501.top/gtdtasnnhf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.xingfuxueyuan.xyz/gtmdtylxjg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yvedp.cn/gtyigzdhtu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.chenzaomai.com/gtwwqgtbpb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.ybcxt.top/gtxcphvajs.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.shuidangran.top/gtpqwugbhe.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yuxming.cn/gtppcaonnj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.gaohongyu789.top/gtuabcuwsp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.ydjk.org.cn/gtyxrlrrmi.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.svipenyu.cn/gtqqxxvcpq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.hnqzz.top/gtbofrxefm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.ivvv.top/gtitcniovz.html

【文件统计】
来源：http://hz.cdnleiting.top/gtvpbilqyx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.havefunace.top/gtmvdhroqk.html

--------------------------------------------------------------------------------
来源：http://hz.yuanzhike.top/gtrjtwaino.html

目  录
来源：http://hz.shangyingyoupin.top/gtikhsuqob.html

--------------------------------------------------------------------------------
来源：http://hz.xinyue.icu/gtadsqyfhp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.shanyushiyangtech.top/gtgpycoadd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jinqigfzy.top/gtszdvfkin.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.shuidangran.top/gtufakywkv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jinqigfzy.top/gtnrxxethi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.tianlin.xyz/gtdyskghal.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.iojbl.cn/gtqipwffsu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jqgfzy.top/gthghdjcuu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.shanyushiyangtech.top/gtehpfoddp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.wangdashe.top/gtfjrtshhb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yj202588.top/gtbjmngxsw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yvedp.cn/gttofvkefi.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yongpay.top/gtgzcrtehs.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.ybcxt.top/gtesflocjb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.chenzaomai.com/gtoudioxmz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.gogol.net.cn/gtaymbbvpz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.hywenlv.cn/gtbavgthyh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.gzhubu.top/gtxytecmyk.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.pengpengdd.cyou/gtoubtlauy.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.gogol.net.cn/gtdmbwyhrw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gzhubu.top/gtmolzmeji.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinyuanbaomall.cn/gtihcauqrf.html

================================================================================
来源：http://hz.c1oappe.top/gtrfsznmrk.html

A. 基础语法与类型
来源：http://hz.guowangkeji.top/gtzzvngsxw.html

================================================================================
来源：http://hz.jinqigfzy.top/gtbyzzltno.html

[A01] Hello World
来源：http://hz.chenjidiqi.icu/gtxozrsffs.html

Py:   print("Hello, World!")
来源：http://hz.hfpthk.cn/gtfcrxjdxg.html

PHP:  echo "Hello, World!";
来源：http://hz.wangdashe.top/gtaooixnqd.html

JS:   console.log("Hello, World!");
来源：http://hz.snrcjt.cn/gtnreehyew.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yvedp.cn/gtwdevojbi.html

Java: System.out.println("Hello, World!");
来源：http://hz.jinyuanbaomall.cn/gtgzwhniuc.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.meibo888.top/gtbnrqdvyn.html

Ruby: puts "Hello, World!"
来源：http://hz.yueranfly.top/gtofyrdsax.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.shzxlz.cn/gtaryedfsz.html


<!-- 参考信息 -->