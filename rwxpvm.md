代发 wailian999

[U31] Py：单测
来源：http://hz.9152youxi.cn/gtwgskytnc.html

python -m pytest -q
来源：http://hz.iojbl.cn/gtgvscdvvg.html

[U32] Py：代码格式化
来源：http://hz.yuxming.cn/gtafvvaxoi.html

ruff format . && ruff check --fix .
来源：http://hz.xuetiantiany.cn/gthbmckyuj.html

[U33] Py：打包发布
来源：http://hz.ehwqpu.com/gtzzrgcgio.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yj20258.top/gtgeippgkb.html

[U34] Py：判断编码
来源：http://hz.ehwqpu.com/gtulhggegi.html

chardet.detect(raw)
来源：http://hz.ywan-chungtsiang.top/gthlrfwpzn.html

[U35] Py：发送邮件
来源：http://hz.9152youxi.cn/gthwgdltcb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.ydjk.org.cn/gttozrtohq.html

[U36] Py：定时任务
来源：http://hz.jqgfzy.top/gtnpfjgijs.html

schedule.every(10).minutes.do(job)
来源：http://hz.xinyue.icu/gtrwwhytpv.html

[U37] Py：读写 Excel
来源：http://hz.gaohongyu789.top/gtbybwtikl.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.svipenyu.cn/gtkednzguo.html

[U38] Py：获取脚本所在目录
来源：http://hz.xingfuxueyuan.xyz/gtfibeolgp.html

Path(__file__).resolve().parent
来源：http://hz.ivvv.top/gtrddaxurb.html

[U39] Py：判断是否在交互环境
来源：http://hz.cashguo.top/gtwncwoagj.html

sys.stdout.isatty()
来源：http://hz.jqgufenzy.top/gtxcbjxozf.html

[U40] Py：打印到标准错误
来源：http://hz.gzhubu.top/gtcweybxqv.html

print("err", file=sys.stderr)
来源：http://hz.xinyue.icu/gtcegpgpmw.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jianghu66.top/gteabbavyz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.fzhhl.top/gtjqicrqdq.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.gogol.net.cn/gtmbwfoakx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hammf.cn/gtudtdsvqf.html

[U43] PHP：声明命名空间
来源：http://hz.zhijiandao.cn/gtirjakjxu.html

namespace App\Http;
来源：http://hz.pycfn.com/gtxoypjcqf.html

[U44] PHP：开启严格类型
来源：http://hz.xziqi.cn/gtehtpvsgm.html

declare(strict_types=1);
来源：http://hz.zycfv.cn/gtbxvempiy.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hysaishi.cn/gttznijcvv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pycfn.com/gthrvurkso.html

[U46] PHP：可空类型
来源：http://hz.gogol.net.cn/gthlzqcxxa.html

?string $name = null
来源：http://hz.zdqjudy.top/gtxcljmsjc.html

[U47] PHP：联合类型
来源：http://hz.gotoacloud.top/gtbpwwcxjg.html

int|string $id
来源：http://hz.ehwqpu.com/gtanepxkrh.html

[U48] PHP：纯枚举
来源：http://hz.svipenyu.cn/gtesisteed.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ybcxt.top/gtazdyflqb.html

[U49] PHP：只读属性
来源：http://hz.yj202588.top/gtsddfxsiw.html

public readonly string $name
来源：http://hz.cqqwz.cn/gtqmmdgvus.html

[U50] PHP：构造器属性提升
来源：http://hz.ydzc1.top/gtpodlxjmq.html

public function __construct(private int $id) {}
来源：http://hz.daria6918.cn/gtfgoejnxe.html

[U51] PHP：数组解构
来源：http://hz.jyoumei.cn/gtcpyfowph.html

[$a, $b] = $arr;
来源：http://hz.fzhhl.top/gtmqlcwezh.html

[U52] PHP：箭头函数
来源：http://hz.jinqigfzy.top/gtjqrunxyf.html

$double = fn($x) => $x * 2;
来源：http://hz.jinghuilouyu.cn/gtjdgdhvsj.html

[U53] PHP：空合并运算符
来源：http://hz.sxryk.cn/gtoxdsufxx.html

$v = $a ?? $b ?? "default";
来源：http://hz.cqqwz.cn/gttrtyyhrf.html

[U54] PHP：空安全调用
来源：http://hz.zhijiandao.cn/gtfveaivki.html

$obj?->method()
来源：http://hz.andypj.xyz/gtytfnmfai.html

[U55] PHP：match 表达式
来源：http://hz.aizwys.cn/gteaepfnka.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.wangshuangyany.cn/gtjbozwydb.html

[U56] PHP：命名参数
来源：http://hz.tanke756.top/gtndbbsaqj.html

f(a: 1, b: 2)
来源：http://hz.havefunace.top/gtlezculuo.html

[U57] PHP：字符串插值
来源：http://hz.nanxuanxn.top/gtwglsvbdr.html

"值: {$a}"
来源：http://hz.yongpay.top/gtefcwjbdv.html

[U58] PHP：数组三件套
来源：http://hz.xziqi.cn/gtsgfdgcgm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.xuetiantiany.cn/gtzfpoxiga.html

[U59] PHP：自定义排序
来源：http://hz.zhoulong.xyz/gtimqchznp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daxiang520.top/gtquyedfzf.html

[U60] PHP：JSON 编解码
来源：http://hz.hnqzz.top/gtiywrykmn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.haohaochexian.top/gtuiqhxskb.html

[U61] PHP：正则
来源：http://hz.ywan-chungtsiang.top/gtcqcutemi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenjidiqi.icu/gtyhifxybs.html

[U62] PHP：日期对象
来源：http://hz.52xcode.cn/gtamddesyb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.cdnleiting.top/gtigcfytss.html

[U63] PHP：文件读写
来源：http://hz.shzxlz.cn/gtlooektqm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.tanke756.top/gtyfdganvz.html

[U64] PHP：目录遍历
来源：http://hz.xingfuxueyuan.xyz/gtkvkapjvq.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.cqqwz.cn/gtnzohbsyn.html

[U65] PHP：会话
来源：http://hz.yj202588.top/gtftbwhvsd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.quarkkingdee.top/gtspymmkpv.html

[U66] PHP：设置 Cookie
来源：http://hz.dianchejie.cn/gtlrwtyaso.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.chenjidiqi.icu/gthvvjwgdu.html

[U67] PHP：处理文件上传
来源：http://hz.mhx1999.top/gtrfdjswfk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.52xcode.cn/gtaaqkkziv.html

[U68] PHP：PDO 连接
来源：http://hz.sweek.top/gtxyqleayv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.fzhhl.top/gththtlcpi.html

[U69] PHP：PDO 预处理
来源：http://hz.gotoacloud.top/gtlanbxbzq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yonumen.top/gtgtbkdwts.html

[U70] PHP：PDO 事务
来源：http://hz.ydjk.org.cn/gtyyizbscl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.9152youxi.cn/gtdcygswxp.html

[U71] PHP：抛出异常
来源：http://hz.fzhhl.top/gtdmvgirgv.html

throw new RuntimeException("失败", 500);
来源：http://hz.smart0.xyz/gthdijkyje.html

[U72] PHP：写错误日志
来源：http://hz.0kj1m.cn/gtcxpeeteq.html

error_log("失败: " . $e->getMessage());
来源：http://hz.9152youxi.cn/gtrvxjwylb.html

[U73] PHP：读取 ini 配置
来源：http://hz.52xcode.cn/gtckwyikrc.html

parse_ini_file("config.ini", true)
来源：http://hz.yj20258888.top/gttcpzwboc.html

[U74] PHP：读取环境变量
来源：http://hz.jinqigfzy.top/gtoqmuvlzt.html

getenv("APP_ENV") ?: "production"
来源：http://hz.dianchejie.cn/gtkekxcchy.html

[U75] PHP：依赖注入
来源：http://hz.shangyingyoupin.top/gtwcwjggxe.html

composer require psr/container
来源：http://hz.zhijiandao.cn/gtpjktwqnm.html

[U76] PHP：简单路由
来源：http://hz.sufxvd.cn/gtqnkiaape.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zycfv.cn/gtcearhgus.html

[U77] PHP：模板渲染
来源：http://hz.guannengcc.top/gtjpaanfev.html

composer require twig/twig
来源：http://hz.wangshuangyany.cn/gthppugaqh.html

[U78] PHP：单元测试
来源：http://hz.yj20258888.top/gtjsngpkjo.html

composer require --dev phpunit/phpunit
来源：http://hz.yonumen.top/gtjyioodna.html

[U79] PHP：静态分析
来源：http://hz.gaohongyu789.top/gtgmczaugs.html

composer require --dev phpstan/phpstan
来源：http://hz.hammf.cn/gthqvhpata.html

[U80] PHP：代码规范修复
来源：http://hz.chenjidiqi.icu/gtdssumzxf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.9152youxi.cn/gtdakqpasl.html

[U81] JS：初始化项目
来源：http://hz.zhengqikj.top/gthktbuqdw.html

npm init -y;  npm i express
来源：http://hz.fzhhl.top/gtxnyrzoyr.html

[U82] JS：package.json 脚本
来源：http://hz.svipenyu.cn/gtrjuvppcv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.c1oappe.top/gtdtgqxlsc.html

[U83] JS：ES Module 导入导出
来源：http://hz.0kj1m.cn/gtycckjgll.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.mhx1999.top/gtepelypcd.html

[U84] JS：CommonJS 写法
来源：http://hz.tian-w.cn/gtewjcqugi.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jianghu66.top/gtgitbwipe.html

[U85] JS：可选链
来源：http://hz.yongpay.top/gtirpgneoc.html

a?.b?.c
来源：http://hz.cheryme.top/gtxaqgipcv.html

[U86] JS：空值合并
来源：http://hz.nanxuanxn.top/gtashjmlph.html

a ?? b
来源：http://hz.jinyuanbaomall.cn/gtezbgesen.html

[U87] JS：解构默认值
来源：http://hz.jqgufenzy.top/gtrknalvxt.html

const { a = 1, b = 2 } = obj;
来源：http://hz.meibo888.top/gtzmonffhc.html

[U88] JS：对象展开合并
来源：http://hz.hfpthk.cn/gteolxvyoe.html

{ ...a, ...b }
来源：http://hz.gogol.net.cn/gtzgfbrbuv.html

[U89] JS：数组去重
来源：http://hz.guowangkeji.top/gtpjbdzuyf.html

[...new Set(arr)]
来源：http://hz.yj20258.top/gtsvkbhwdw.html

[U90] JS：数字数组排序
来源：http://hz.birdmap.top/gtsvxwatwz.html

[...arr].sort((a, b) => a - b)
来源：http://hz.sufxvd.cn/gtngefwxwp.html

[U91] JS：对象键值遍历
来源：http://hz.yj20258888.top/gtxqpokncs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.hfpthk.cn/gtcldaupye.html

[U92] JS：深拷贝
来源：http://hz.dianchejie.cn/gtwxnlazev.html

structuredClone(obj)
来源：http://hz.guowangkeji.top/gtaajpmpde.html

[U93] JS：模板字符串
来源：http://hz.birdmap.top/gtxyhkzfnm.html

`共 ${n} 条`
来源：http://hz.xingfuxueyuan.xyz/gtnuhlvlry.html

[U94] JS：箭头函数
来源：http://hz.cheryme.top/gtvykwflrt.html

const double = x => x * 2;
来源：http://hz.iojbl.cn/gttgktmlui.html

[U95] JS：Promise 包装
来源：http://hz.yuxming.cn/gtpfcbumfm.html

new Promise((resolve, reject) => {})
来源：http://hz.zhaomingkeji.xyz/gtfescoqbi.html

[U96] JS：async/await 与异常
来源：http://hz.hammf.cn/gtyawexxnq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.hnqzz.top/gtxgxzhymm.html

[U97] JS：并发请求
来源：http://hz.nwbrower.top/gtgvrgytmz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuanzx.com/gtzhijkxvp.html

[U98] JS：fetch 带 JSON
来源：http://hz.cheryme.top/gtmhawmysd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.xuetiantiany.cn/gtttwphrgc.html

[U99] JS：事件监听
来源：http://hz.xuanzx.com/gtmvdoldmd.html

el.addEventListener("click", e => {})
来源：http://hz.sufxvd.cn/gtbvsxerrx.html

[U100] JS：DOM 查询
来源：http://hz.0kj1m.cn/gtwwwhspty.html

document.querySelector(".item")
来源：http://hz.cdnleiting.top/gtnogkvbgj.html

[U101] JS：classList 操作
来源：http://hz.yvedp.cn/gtbmhntund.html

el.classList.toggle("active")
来源：http://hz.chenjidiqi.icu/gtxzgwkzho.html

[U102] JS：本地存储
来源：http://hz.xuanzx.com/gtkhrhnqnr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.hfpthk.cn/gtpjqdpipt.html

[U103] JS：定时器
来源：http://hz.hnxiangtu.top/gtnftogton.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.shzxlz.cn/gtmqgemtxa.html

[U104] JS：防抖
来源：http://hz.c1oappe.top/gtjpqeemlg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dianchejie.cn/gtgvvuzsnc.html

[U105] JS：节流
来源：http://hz.fzhhl.top/gtgqskooyc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yj20258.top/gtlmxchihg.html

[U106] JS：日期格式化
来源：http://hz.hnxiangtu.top/gtwjwayvxt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ehwqpu.com/gtevbdpzpn.html

[U107] JS：数字千分位
来源：http://hz.pycfn.com/gtdylbpafk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.shanyushiyangkeji.top/gtznciyoln.html

[U108] JS：随机整数
来源：http://hz.sweek.top/gtspmevfer.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.svipenyu.cn/gtnnvrfmwb.html

[U109] JS：数组分组
来源：http://hz.havefunace.top/gtbdtaoudw.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jiagoushi.top/gtnbeskiqo.html

[U110] JS：数组分块
来源：http://hz.zhengqikj.top/gttflkwwya.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.hongshengwenyu.top/gthixaniuc.html

[U111] JS：对象转 Map
来源：http://hz.birdmap.top/gtkcoqznhx.html

new Map(Object.entries(obj))
来源：http://hz.52xcode.cn/gtzfeytfps.html

[U112] JS：字符串补位
来源：http://hz.shangyingyoupin.top/gtuqifjbtn.html

"7".padStart(3, "0")
来源：http://hz.snrcjt.cn/gtvhlefflp.html

[U113] JS：正则替换全部
来源：http://hz.zhiwuduotai.top/gtjdhzehdf.html

s.replaceAll("a", "b")
来源：http://hz.pycfn.com/gtkmlspezn.html

[U114] JS：JSON 深比较
来源：http://hz.zhixingplan.top/gtzfdqdcql.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.aibaodan.cn/gtjiyopcbe.html

[U115] JS：生成 UUID
来源：http://hz.ydzc1.top/gthadotolj.html

crypto.randomUUID()
来源：http://hz.chenjidiqi.icu/gtenldxzps.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hfpthk.cn/gtawukrhvq.html

/** @param {string} name */ function f(name) {}
来源：http://hz.sweek.top/gtltjzrjaw.html

[U117] JS：单元测试
来源：http://hz.hysaishi.cn/gtdljsxjds.html

npm i -D vitest;  npx vitest
来源：http://hz.xuetiantiany.cn/gtdndxdegy.html

[U118] JS：开发服务器
来源：http://hz.xylfe.cn/gtmtcvfrug.html

npm i -D vite;  npx vite
来源：http://hz.pengpengdd.cyou/gtljcywbym.html

[U119] JS：生产构建
来源：http://hz.snrcjt.cn/gtofcncowm.html

npx vite build
来源：http://hz.zhiwuduotai.top/gtdjslrmnh.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yj20258888.top/gttyudljbi.html

import.meta.env.VITE_API_URL
来源：http://hz.sweek.top/gtojgxjdae.html

================================================================================
来源：http://hz.xinyue.icu/gtbdqkiaze.html

统计汇总
来源：http://hz.wangdashe.top/gtdnqzyubi.html

================================================================================
来源：http://hz.sufxvd.cn/gtycmzukpb.html

按语言统计（条）：
来源：http://hz.hongshengwenyu.top/gtqbmimfsk.html

Python ......... 252
来源：http://hz.xinyue.icu/gtdgkqxvee.html

PHP ............ 252
来源：http://hz.ppjwa.cn/gtatvodlmo.html

JavaScript ..... 252
来源：http://hz.cashguo.top/gtktcbtmcv.html

TypeScript ..... 212
来源：http://hz.redwolf501.top/gtmjrjsjql.html

Java ........... 212
来源：http://hz.zhiwuduotai.top/gtlqiosdkm.html

Go ............. 212
来源：http://hz.chenlongwang.top/gtqwutcgar.html

Ruby ........... 212
来源：http://hz.nwbrower.top/gtoopzbvjx.html

C# ............. 212
来源：http://hz.andypj.xyz/gtzqnwsrln.html

C .............. 30
来源：http://hz.52xcode.cn/gtvhiffwkr.html

C++ ............ 30
来源：http://hz.yonumen.top/gttgfxklxe.html

SQL ............ 90
来源：http://hz.xuetiantiany.cn/gthnsesbnq.html

Bash ........... 80
来源：http://hz.daria6918.cn/gtzyelpclc.html

Kotlin ......... 15
来源：http://hz.bjfxy.top/gtxdcpftws.html

Swift .......... 15
来源：http://hz.jinyuanbaomall.cn/gtduuzqnrg.html

Lua ............ 10
来源：http://hz.hnqzz.top/gtvngqvjzy.html

Perl ........... 10
来源：http://hz.yj20258888.top/gtgsqciwtl.html

Scala .......... 10
来源：http://hz.aibaodan.cn/gtslxsksom.html

------------------------------------
来源：http://hz.gogol.net.cn/gteuupcfnt.html

合计 ........... 2106 条
来源：http://hz.shanyushiyangtech.top/gtgbxpweij.html

按章节统计：
来源：http://hz.shuidangran.top/gtmcthowcj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.pengpengdd.cyou/gtqlkiozbb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhixingplan.top/gtbvbqykgx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.ivvv.top/gtxzhqcwtm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.c1oappe.top/gtyrlymqht.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.quarkkingdee.top/gtltaznvtr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.fengsongda.top/gtgszdepuu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yj202588.top/gtuxmkgpsp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.xuanzx.com/gtgrsrmfzc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.shzxlz.cn/gteyqecpjw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.aibaodan.cn/gtuxbpngdz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jinqigufen.top/gtevjuhgiw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.cqqwz.cn/gtfyjuzhid.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.sxryk.cn/gtiqvfxzbm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jqgfzy.top/gtzpphprry.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.316326.xyz/gtmymkylmz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.xylfe.cn/gtdjwmfhgm.html

Q SQL 专题                              90
来源：http://hz.nanxinkj.top/gtdxjcjuvy.html

R Bash 专题                             80
来源：http://hz.smart0.xyz/gtreisvzdu.html

S C / C++ 专题                          60
来源：http://hz.zhongyouzk.top/gtjlxzgoug.html

T 其他语言补充                          60
来源：http://hz.fzhhl.top/gtmxgiosay.html

U 高频实用片段                         120
来源：http://hz.zhijiandao.cn/gtcocvtatt.html

------------------------------------
来源：http://hz.hammf.cn/gtnexfvekr.html

合计                                  2106 条
来源：http://hz.yj20258888.top/gtbxdkadnw.html

--------------------------------------------------------------------------------
来源：http://hz.yongpay.top/gteoqeulxm.html

使用提醒
来源：http://hz.xziqi.cn/gtoxbxdmgz.html

--------------------------------------------------------------------------------
来源：http://hz.chenzaomai.com/gtbqzipgcw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.nanxinkj.top/gtbqgrmish.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.316326.xyz/gtbyletuod.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.xingfuxueyuan.xyz/gtlqvobaxs.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.shanyushiyangkeji.top/gtxwqjzhiv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.xziqi.cn/gtxskzahnt.html

—— 文件结束 ——
来源：http://hz.smart0.xyz/gtnuyeyphx.html

================================================================================
来源：http://hz.tian-w.cn/gtbjqmdnbv.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.pengpengdd.cyou/gtswdmjqld.html

Common Programming Examples Cheat Book
来源：http://hz.shzxlz.cn/gthhzmxzto.html

================================================================================
来源：http://hz.gaohongyu789.top/gtlpcumptc.html

【收录内容】
来源：http://hz.yanxiufei.cn/gtbbrsgxwo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.tianlin.xyz/gtiubalnzw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.cashguo.top/gttwfwvgbs.html

SQL · Bash · C · C++
来源：http://hz.jqgfzy.top/gticoxtpqx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.guowangkeji.top/gtuudmqllg.html

【使用说明】
来源：http://hz.ehwqpu.com/gtovamenjv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.sxryk.cn/gtsoibpqmv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.ybcxt.top/gtegtjybzt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zhoulong.xyz/gtdowgudql.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.sufxvd.cn/gtlsljhdfr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.nanxinkj.top/gtlffplfwm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.ydjk.org.cn/gtbgghjdlq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yuanzhike.top/gtrrtpjwwx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.svipenyu.cn/gtlrioimpy.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.52xcode.cn/gtvbisfiti.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yanxiufei.cn/gtupakpevn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.daria6918.cn/gtnzgizdua.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.hammf.cn/gtmyibvrfs.html

【文件统计】
来源：http://hz.nanxinkj.top/gtqedvvpjg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.shanyushiyangtech.top/gtmohxbkix.html

--------------------------------------------------------------------------------
来源：http://hz.hysaishi.cn/gtetavfkhn.html

目  录
来源：http://hz.jinghuilouyu.cn/gtkwbpxult.html

--------------------------------------------------------------------------------
来源：http://hz.ybcxt.top/gtoqiureml.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.tian-w.cn/gtfrktzzbf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.xylfe.cn/gtbngrnnsk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.shuidangran.top/gtlxxrixqu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.quarkkingdee.top/gtjippsqqm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.guowangkeji.top/gteiqghytf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.gaohongyu789.top/gtzqnolgog.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.hywenlv.cn/gtgkrztdub.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yvedp.cn/gttegdtdpz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.gzhubu.top/gtjrkmslxl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jinqigfzy.top/gtgafgfudi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.xziqi.cn/gtgktnhtge.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yuanzhike.top/gtsofffgyy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.jqgfzy.top/gtuwqhuaze.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.sufxvd.cn/gtrevsiymn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.sweek.top/gtspbkcqnw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.sxryk.cn/gtbojfviws.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.ydzc1.top/gtqhrszayz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.xziqi.cn/gtkutlperg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yongpay.top/gtrbjnjdel.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jianghu66.top/gtsdqlmclx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinqigfzy.top/gtqhblhnho.html

================================================================================
来源：http://hz.yuanzhike.top/gtobxssoqs.html

A. 基础语法与类型
来源：http://hz.shanyushiyangtech.top/gtdrcfnose.html

================================================================================
来源：http://hz.zhixingplan.top/gtjnlzslro.html

[A01] Hello World
来源：http://hz.0kj1m.cn/gtghfyzuxa.html

Py:   print("Hello, World!")
来源：http://hz.kuanghao11.cn/gtdkckgkeo.html

PHP:  echo "Hello, World!";
来源：http://hz.ywan-chungtsiang.top/gtpqpbwqbq.html

JS:   console.log("Hello, World!");
来源：http://hz.hysaishi.cn/gtmuxmslbc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zhengqikj.top/gtgipvbppe.html

Java: System.out.println("Hello, World!");
来源：http://hz.hnqzz.top/gtvyerkwqs.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.svipenyu.cn/gtibbaduhe.html

Ruby: puts "Hello, World!"
来源：http://hz.xingfuxueyuan.xyz/gtmbnuvcnk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.hnxiangtu.top/gtrlorvqtb.html

[A02] 变量声明与赋值
来源：http://hz.jinqigfzy.top/gttefhxkam.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.cucudq.cn/gtmssgojvh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jqgfzy.top/gtgoadtjux.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.zdqjudy.top/gttjdtfguc.html


<!-- 参考信息 -->