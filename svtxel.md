代发 wailian999

[U33] Py：打包发布
来源：http://hz.jiagoushi.top/gtnakqoitd.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hfpthk.cn/gtimyfdroe.html

[U34] Py：判断编码
来源：http://hz.meibo888.top/gtrwdimpcj.html

chardet.detect(raw)
来源：http://hz.52xcode.cn/gtydfygqnu.html

[U35] Py：发送邮件
来源：http://hz.jiagoushi.top/gtbnlsires.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.c1oappe.top/gtiffpusrw.html

[U36] Py：定时任务
来源：http://hz.jinyuanbaomall.cn/gtyhwqriqr.html

schedule.every(10).minutes.do(job)
来源：http://hz.jqgfzy.top/gtqcmxbepa.html

[U37] Py：读写 Excel
来源：http://hz.nwbrower.top/gtvpnmdwvv.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.iojbl.cn/gtfalwwxio.html

[U38] Py：获取脚本所在目录
来源：http://hz.zycfv.cn/gtdpzrdhie.html

Path(__file__).resolve().parent
来源：http://hz.tianlin.xyz/gtiqwxflis.html

[U39] Py：判断是否在交互环境
来源：http://hz.hysaishi.cn/gtxhfrkbvr.html

sys.stdout.isatty()
来源：http://hz.ppjwa.cn/gtmcupheyx.html

[U40] Py：打印到标准错误
来源：http://hz.hongshengwenyu.top/gtkkykipsa.html

print("err", file=sys.stderr)
来源：http://hz.zdqjudy.top/gttrpwmmvv.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.xziqi.cn/gtvrsunuep.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.daria6918.cn/gtvknwtdhu.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.shangyingyoupin.top/gtpkmgexdk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.quarkkingdee.top/gtirzumlmu.html

[U43] PHP：声明命名空间
来源：http://hz.chenjidiqi.icu/gtfgkbxexz.html

namespace App\Http;
来源：http://hz.chenjidiqi.icu/gtaqdtrecm.html

[U44] PHP：开启严格类型
来源：http://hz.hywenlv.cn/gtuvxdzokb.html

declare(strict_types=1);
来源：http://hz.aibaodan.cn/gtizccslvm.html

[U45] PHP：类型声明与返回类型
来源：http://hz.jianghu66.top/gtepwbgmzs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shzxlz.cn/gtucfrlzqh.html

[U46] PHP：可空类型
来源：http://hz.hfpthk.cn/gtjkhtfdsa.html

?string $name = null
来源：http://hz.svipenyu.cn/gtkfvrzysk.html

[U47] PHP：联合类型
来源：http://hz.mhx1999.top/gtksbvvayl.html

int|string $id
来源：http://hz.ydzc1.top/gtkvnvzslb.html

[U48] PHP：纯枚举
来源：http://hz.hywenlv.cn/gtyggfnqgz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.shuidangran.top/gtlaijizks.html

[U49] PHP：只读属性
来源：http://hz.jqgufenzy.top/gtbiruxsgi.html

public readonly string $name
来源：http://hz.316326.xyz/gtisovrzgi.html

[U50] PHP：构造器属性提升
来源：http://hz.andypj.xyz/gtomvfhwtf.html

public function __construct(private int $id) {}
来源：http://hz.zhengqikj.top/gttehasbgd.html

[U51] PHP：数组解构
来源：http://hz.feifeiyinyue.top/gtrzlfpxxc.html

[$a, $b] = $arr;
来源：http://hz.xinyue.icu/gtmbiibuau.html

[U52] PHP：箭头函数
来源：http://hz.daria6918.cn/gtwlhxqqkh.html

$double = fn($x) => $x * 2;
来源：http://hz.sxryk.cn/gtgpfzppey.html

[U53] PHP：空合并运算符
来源：http://hz.jlsjyb.cn/gtgytcjmcs.html

$v = $a ?? $b ?? "default";
来源：http://hz.jlsjyb.cn/gtrqlypccb.html

[U54] PHP：空安全调用
来源：http://hz.ehwqpu.com/gtpyxmaxzp.html

$obj?->method()
来源：http://hz.wangdashe.top/gthgykszsm.html

[U55] PHP：match 表达式
来源：http://hz.aibaodan.cn/gtbvcwoxqs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.guannengcc.top/gtgqfalxnr.html

[U56] PHP：命名参数
来源：http://hz.daria6918.cn/gtvuhrzigu.html

f(a: 1, b: 2)
来源：http://hz.yj202588.top/gtdvpbacqp.html

[U57] PHP：字符串插值
来源：http://hz.ivvv.top/gtznebyuqd.html

"值: {$a}"
来源：http://hz.hywenlv.cn/gtryvcsdgm.html

[U58] PHP：数组三件套
来源：http://hz.iojbl.cn/gtsnamonjw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.birdmap.top/gtmwdwzjjm.html

[U59] PHP：自定义排序
来源：http://hz.feifeiyinyue.top/gtlgqpsmel.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.guowangkeji.top/gtaxsrsfon.html

[U60] PHP：JSON 编解码
来源：http://hz.9152youxi.cn/gtribiggfc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zdqjudy.top/gtqlrylsov.html

[U61] PHP：正则
来源：http://hz.fengsongda.top/gtnnnqaurs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj202588.top/gtxsxswdck.html

[U62] PHP：日期对象
来源：http://hz.yj20258.top/gtyoeighka.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.chenlongwang.top/gtjexnfsqg.html

[U63] PHP：文件读写
来源：http://hz.xuetiantiany.cn/gtyebmiwat.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yj20258.top/gtiyzrnqna.html

[U64] PHP：目录遍历
来源：http://hz.wangdashe.top/gtxsdmdmeq.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.xingfuxueyuan.xyz/gtjgcnmpvn.html

[U65] PHP：会话
来源：http://hz.cucudq.cn/gtiaznkaii.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yongpay.top/gtqxsbfqzp.html

[U66] PHP：设置 Cookie
来源：http://hz.zhongyouzk.top/gtkodpqcmp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zycfv.cn/gttqsrxsvh.html

[U67] PHP：处理文件上传
来源：http://hz.shangyingyoupin.top/gtzgiujysy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jinghuilouyu.cn/gtelcgiajk.html

[U68] PHP：PDO 连接
来源：http://hz.xziqi.cn/gtjwktyokz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jqgufenzy.top/gtwuemhzot.html

[U69] PHP：PDO 预处理
来源：http://hz.zycfv.cn/gtekmfzwux.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.shanyushiyangtech.top/gtvfmjhmmz.html

[U70] PHP：PDO 事务
来源：http://hz.jinqigufen.top/gtozstaocz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hfpthk.cn/gtwizilcnx.html

[U71] PHP：抛出异常
来源：http://hz.xingfuxueyuan.xyz/gtyftvzklw.html

throw new RuntimeException("失败", 500);
来源：http://hz.hfpthk.cn/gthpdlaakl.html

[U72] PHP：写错误日志
来源：http://hz.ivvv.top/gtvywywyss.html

error_log("失败: " . $e->getMessage());
来源：http://hz.dashuyun.cn/gtvgawlrxm.html

[U73] PHP：读取 ini 配置
来源：http://hz.cqqwz.cn/gtcupmxikx.html

parse_ini_file("config.ini", true)
来源：http://hz.yueranfly.top/gtxpnynpie.html

[U74] PHP：读取环境变量
来源：http://hz.yuanzhike.top/gtclggjihp.html

getenv("APP_ENV") ?: "production"
来源：http://hz.ydjk.org.cn/gtwefdhqzq.html

[U75] PHP：依赖注入
来源：http://hz.tian-w.cn/gtlmdljhaa.html

composer require psr/container
来源：http://hz.yj20258888.top/gtgatabqmx.html

[U76] PHP：简单路由
来源：http://hz.zhongyouzk.top/gtzymojkec.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.chenjidiqi.icu/gthnsvslra.html

[U77] PHP：模板渲染
来源：http://hz.pengpengdd.cyou/gtfdjtbftb.html

composer require twig/twig
来源：http://hz.zhoulong.xyz/gthdojphay.html

[U78] PHP：单元测试
来源：http://hz.xuanzx.com/gtjxrekxix.html

composer require --dev phpunit/phpunit
来源：http://hz.yueranfly.top/gtkbqznlrw.html

[U79] PHP：静态分析
来源：http://hz.hfpthk.cn/gtiwqtmldg.html

composer require --dev phpstan/phpstan
来源：http://hz.wangshuangyany.cn/gtbfybnoma.html

[U80] PHP：代码规范修复
来源：http://hz.wangshuangyany.cn/gtehwjcrwt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.shangyingyoupin.top/gtniyiapic.html

[U81] JS：初始化项目
来源：http://hz.cheryme.top/gtldouxyiv.html

npm init -y;  npm i express
来源：http://hz.guannengcc.top/gtlypdrgvx.html

[U82] JS：package.json 脚本
来源：http://hz.gzhubu.top/gtiimwenhx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.shangyingyoupin.top/gtmpsxkrsg.html

[U83] JS：ES Module 导入导出
来源：http://hz.jinqigufen.top/gtxjtmlkvy.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.jinyuanbaomall.cn/gtwsaakvfb.html

[U84] JS：CommonJS 写法
来源：http://hz.hnqzz.top/gtqytfmxzb.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.iojbl.cn/gtkqkplvuj.html

[U85] JS：可选链
来源：http://hz.yj20258888.top/gtuscrslih.html

a?.b?.c
来源：http://hz.jinghuilouyu.cn/gtedpkovmh.html

[U86] JS：空值合并
来源：http://hz.dianchejie.cn/gtkhmeyhzu.html

a ?? b
来源：http://hz.chenjidiqi.icu/gtwenqbgnm.html

[U87] JS：解构默认值
来源：http://hz.nanxinkj.top/gtocpnqxwx.html

const { a = 1, b = 2 } = obj;
来源：http://hz.haohaochexian.top/gtbdxydysx.html

[U88] JS：对象展开合并
来源：http://hz.iojbl.cn/gtdzwrgueq.html

{ ...a, ...b }
来源：http://hz.zhongyouzk.top/gtwyelvkhh.html

[U89] JS：数组去重
来源：http://hz.nanxinkj.top/gttpshvcar.html

[...new Set(arr)]
来源：http://hz.redwolf501.top/gtoiwopcnw.html

[U90] JS：数字数组排序
来源：http://hz.gzhubu.top/gtyhpotmzp.html

[...arr].sort((a, b) => a - b)
来源：http://hz.redwolf501.top/gtnfjflhqg.html

[U91] JS：对象键值遍历
来源：http://hz.redwolf501.top/gtmfumoywi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.gaohongyu789.top/gthxshradk.html

[U92] JS：深拷贝
来源：http://hz.birdmap.top/gtlqlsyhaf.html

structuredClone(obj)
来源：http://hz.gotoacloud.top/gtdhksucyv.html

[U93] JS：模板字符串
来源：http://hz.zhixingplan.top/gtjllyvnvm.html

`共 ${n} 条`
来源：http://hz.sxryk.cn/gtlceszgrt.html

[U94] JS：箭头函数
来源：http://hz.yonumen.top/gttobfruuu.html

const double = x => x * 2;
来源：http://hz.birdmap.top/gtetwscshu.html

[U95] JS：Promise 包装
来源：http://hz.tian-w.cn/gtcbddpqoc.html

new Promise((resolve, reject) => {})
来源：http://hz.tanke756.top/gtupkbbtvw.html

[U96] JS：async/await 与异常
来源：http://hz.dianchejie.cn/gtxcxsotyx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ywan-chungtsiang.top/gtunosdkib.html

[U97] JS：并发请求
来源：http://hz.fengsongda.top/gtqiptfrmb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guowangkeji.top/gtepkmkoxs.html

[U98] JS：fetch 带 JSON
来源：http://hz.xziqi.cn/gtmwzdvdgk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.tian-w.cn/gtmzkbmkco.html

[U99] JS：事件监听
来源：http://hz.ehwqpu.com/gtccbgrozs.html

el.addEventListener("click", e => {})
来源：http://hz.yonumen.top/gtpuxynlyo.html

[U100] JS：DOM 查询
来源：http://hz.cheryme.top/gterevcfeo.html

document.querySelector(".item")
来源：http://hz.xingfuxueyuan.xyz/gtvoyojnjk.html

[U101] JS：classList 操作
来源：http://hz.meibo888.top/gtoyzuzhxr.html

el.classList.toggle("active")
来源：http://hz.316326.xyz/gtyjjcozrw.html

[U102] JS：本地存储
来源：http://hz.nanxinkj.top/gttabbkkfn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.fengsongda.top/gtkknysauh.html

[U103] JS：定时器
来源：http://hz.jqgufenzy.top/gtyrmrcjmq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xingfuxueyuan.xyz/gtkmedfydq.html

[U104] JS：防抖
来源：http://hz.aibaodan.cn/gtdprtbycp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guannengcc.top/gtjsltdane.html

[U105] JS：节流
来源：http://hz.hysaishi.cn/gtathlcasc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jiagoushi.top/gtelynuszi.html

[U106] JS：日期格式化
来源：http://hz.zhiwuduotai.top/gtntgxlexu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhixingplan.top/gtrdbayadz.html

[U107] JS：数字千分位
来源：http://hz.guannengcc.top/gtmdfqgkkc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.cqqwz.cn/gtwrzmyied.html

[U108] JS：随机整数
来源：http://hz.fzhhl.top/gtqtmvwzwr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yonumen.top/gtcnytjdkq.html

[U109] JS：数组分组
来源：http://hz.hywenlv.cn/gtoafypdud.html

Object.groupBy(arr, x => x.type)
来源：http://hz.tian-w.cn/gtzpytoorj.html

[U110] JS：数组分块
来源：http://hz.ybcxt.top/gtduvleorn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.wangdashe.top/gtgazsspqn.html

[U111] JS：对象转 Map
来源：http://hz.meibo888.top/gtpbinnqzh.html

new Map(Object.entries(obj))
来源：http://hz.nanxuanxn.top/gttwassjme.html

[U112] JS：字符串补位
来源：http://hz.jinyuanbaomall.cn/gtgudffwuw.html

"7".padStart(3, "0")
来源：http://hz.zhongyouzk.top/gtksnzzizf.html

[U113] JS：正则替换全部
来源：http://hz.yj20258888.top/gtsvutiuud.html

s.replaceAll("a", "b")
来源：http://hz.c1oappe.top/gtdmvoaxdt.html

[U114] JS：JSON 深比较
来源：http://hz.sxryk.cn/gtuvmneptu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shanyushiyangkeji.top/gtivbdkpcx.html

[U115] JS：生成 UUID
来源：http://hz.zhiwuduotai.top/gtbnnputll.html

crypto.randomUUID()
来源：http://hz.nanxinkj.top/gtofojcjzq.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yonumen.top/gtziugixug.html

/** @param {string} name */ function f(name) {}
来源：http://hz.snrcjt.cn/gtoitiavpp.html

[U117] JS：单元测试
来源：http://hz.shuidangran.top/gtjtifzssh.html

npm i -D vitest;  npx vitest
来源：http://hz.gotoacloud.top/gtkrwjlpbr.html

[U118] JS：开发服务器
来源：http://hz.vqdsnc.cn/gtfovxwiyy.html

npm i -D vite;  npx vite
来源：http://hz.9152youxi.cn/gtgyzedtsu.html

[U119] JS：生产构建
来源：http://hz.zdqjudy.top/gtldpmkequ.html

npx vite build
来源：http://hz.zhiwuduotai.top/gtwgqfwyez.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhiwuduotai.top/gtwzbnnhyd.html

import.meta.env.VITE_API_URL
来源：http://hz.xuetiantiany.cn/gtwpaqskbd.html

================================================================================
来源：http://hz.yvedp.cn/gtpnulxkfw.html

统计汇总
来源：http://hz.chenjidiqi.icu/gtbpzvxiqs.html

================================================================================
来源：http://hz.cucudq.cn/gtjkwmavvt.html

按语言统计（条）：
来源：http://hz.tian-w.cn/gtvvurevme.html

Python ......... 252
来源：http://hz.jyoumei.cn/gtrtwvmmvs.html

PHP ............ 252
来源：http://hz.yongpay.top/gtvdkwdbpz.html

JavaScript ..... 252
来源：http://hz.sweek.top/gtgckwqwdv.html

TypeScript ..... 212
来源：http://hz.pengpengdd.cyou/gtncglaiam.html

Java ........... 212
来源：http://hz.jinghuilouyu.cn/gtazcjrcux.html

Go ............. 212
来源：http://hz.andypj.xyz/gtqdzscqcu.html

Ruby ........... 212
来源：http://hz.gogol.net.cn/gtytfwwliv.html

C# ............. 212
来源：http://hz.zhengqikj.top/gtbzqrqhhr.html

C .............. 30
来源：http://hz.birdmap.top/gtsuumlcys.html

C++ ............ 30
来源：http://hz.zhengqikj.top/gtocurcnjn.html

SQL ............ 90
来源：http://hz.chenzaomai.com/gtakapepwo.html

Bash ........... 80
来源：http://hz.gzhubu.top/gteoaphxbk.html

Kotlin ......... 15
来源：http://hz.xziqi.cn/gtgfvbmqaw.html

Swift .......... 15
来源：http://hz.xinyue.icu/gttohcajnc.html

Lua ............ 10
来源：http://hz.xuanzx.com/gtsxqqubmy.html

Perl ........... 10
来源：http://hz.zhiwuduotai.top/gtbgkiomrd.html

Scala .......... 10
来源：http://hz.nanxinkj.top/gtrdekitpy.html

------------------------------------
来源：http://hz.ydzc1.top/gthmlhoyhe.html

合计 ........... 2106 条
来源：http://hz.bjfxy.top/gtfibhemtv.html

按章节统计：
来源：http://hz.316326.xyz/gtcufaqtxn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.sysykeji.top/gtreggfdjz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.nanxinkj.top/gtlifwqfzh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.cqqwz.cn/gtzvbhaodw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.gaohongyu789.top/gtapsljrms.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yuxming.cn/gtttvwwajx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.fzhhl.top/gtuhsjwegj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.zhaomingkeji.xyz/gtnbiouvhe.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.jyoumei.cn/gtiuuhuazw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.ppjwa.cn/gtuxvntukz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ydzc1.top/gtkhjwmpgy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhoulong.xyz/gtkvadjucr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yonumen.top/gtaloafxkx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.shuidangran.top/gtlfhxgftz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.shanyushiyangtech.top/gtgcbyoflw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yj20258.top/gtnszoaduy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.ywan-chungtsiang.top/gthxmeccml.html

Q SQL 专题                              90
来源：http://hz.hfpthk.cn/gtqpprioup.html

R Bash 专题                             80
来源：http://hz.yuxming.cn/gthzfukhbi.html

S C / C++ 专题                          60
来源：http://hz.yueranfly.top/gtkhrzhmfa.html

T 其他语言补充                          60
来源：http://hz.shuidangran.top/gtkppceukl.html

U 高频实用片段                         120
来源：http://hz.bjfxy.top/gtaxfifnqn.html

------------------------------------
来源：http://hz.svipenyu.cn/gtjxxshghx.html

合计                                  2106 条
来源：http://hz.yueranfly.top/gtreffsbye.html

--------------------------------------------------------------------------------
来源：http://hz.yanxiufei.cn/gttmcvamlz.html

使用提醒
来源：http://hz.tanke756.top/gthneadmly.html

--------------------------------------------------------------------------------
来源：http://hz.316326.xyz/gtwiliaqrs.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.316326.xyz/gtxnangvew.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.smart0.xyz/gtzcdzqqkz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yuanzhike.top/gteojemkjo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yanxiufei.cn/gtadwjjssv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yongpay.top/gtecmaxzek.html

—— 文件结束 ——
来源：http://hz.zhiwuduotai.top/gtqjytnijv.html

================================================================================
来源：http://hz.cqqwz.cn/gtjsrjnyuc.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ppjwa.cn/gtfesspsex.html

Common Programming Examples Cheat Book
来源：http://hz.nwbrower.top/gthtsmzeny.html

================================================================================
来源：http://hz.iojbl.cn/gtjrsvvyev.html

【收录内容】
来源：http://hz.jqgfzy.top/gtoglkiugo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yuxming.cn/gtdquxtcxy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yueranfly.top/gtedgzggkp.html

SQL · Bash · C · C++
来源：http://hz.ydzc1.top/gtfoqglxgk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.shangyingyoupin.top/gtkhvjflhx.html

【使用说明】
来源：http://hz.ydjk.org.cn/gtfcyjcxbb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.sysykeji.top/gtyfjsfmvp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zhengqikj.top/gttfkukxbl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.dashuyun.cn/gthmbxvglg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.wangshuangyany.cn/gtjxfidkpc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.kuanghao11.cn/gthnylvabv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.sysykeji.top/gttesvamwv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.pengpengdd.cyou/gtruvhvwrs.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.chenzaomai.com/gtbxfxnpvo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.cashguo.top/gtstliaqzw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.wangshuangyany.cn/gtcworfwrx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.0kj1m.cn/gtnahcaqgb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.9152youxi.cn/gtoeksapum.html

【文件统计】
来源：http://hz.guowangkeji.top/gtfpwxmzml.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.zhaomingkeji.xyz/gtpjuvtacl.html

--------------------------------------------------------------------------------
来源：http://hz.haohaochexian.top/gtnhgpyyto.html

目  录
来源：http://hz.ivvv.top/gtyhkoaabu.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258.top/gtxzdvpues.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.gzhubu.top/gtitncucax.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.shuidangran.top/gtqtxrhukj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.hongshengwenyu.top/gtnwdhcyut.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.tanke756.top/gtmhdplxjt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jinyuanbaomall.cn/gttqexdlzu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.guannengcc.top/gtlromkcmj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.hammf.cn/gtpfvzwlth.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.ehwqpu.com/gtlrdbgzip.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.feifeiyinyue.top/gtzrrwmaeb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yanxiufei.cn/gtitxekafe.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.pengpengdd.cyou/gtjfpjpnof.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.cqqwz.cn/gttooaqvvk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.chenjidiqi.icu/gtkguupapw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.cheryme.top/gtmowtjlcm.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.gogol.net.cn/gtzawnkvxs.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.dianchejie.cn/gtqrwszkhf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.hongshengwenyu.top/gtllixrsku.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jinqigfzy.top/gtipusijiu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.bjfxy.top/gtjxpngcsk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yuanzhike.top/gtwrsvcngb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.daria6918.cn/gtdxrbwzxp.html

================================================================================
来源：http://hz.ivvv.top/gtadmzakfi.html

A. 基础语法与类型
来源：http://hz.gogol.net.cn/gtlxbtdcem.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtnwblxqzw.html

[A01] Hello World
来源：http://hz.iojbl.cn/gtwmwubvcq.html

Py:   print("Hello, World!")
来源：http://hz.yongpay.top/gtnngbxftt.html

PHP:  echo "Hello, World!";
来源：http://hz.jyoumei.cn/gtvzuynjbz.html

JS:   console.log("Hello, World!");
来源：http://hz.cdnleiting.top/gtkpnpnkqx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.tianlin.xyz/gtlvarhfpz.html

Java: System.out.println("Hello, World!");
来源：http://hz.jinqigfzy.top/gtpkqotbqx.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.xinyue.icu/gtpaftqpuj.html

Ruby: puts "Hello, World!"
来源：http://hz.fzhhl.top/gtjbakdwap.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.dashuyun.cn/gtxdhdlhvn.html

[A02] 变量声明与赋值
来源：http://hz.gzhubu.top/gthxzmpego.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.ydjk.org.cn/gtiwbxdcgm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.fengsongda.top/gtnsztquhb.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.iojbl.cn/gtumnylaea.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.gaohongyu789.top/gtpgzibneb.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.zycfv.cn/gtdidxestf.html

Go:   name := "Alex"; age := 20
来源：http://hz.zycfv.cn/gtpxfinusw.html

Ruby: name = "Alex"; age = 20
来源：http://hz.xylfe.cn/gthtqrxpnq.html


<!-- 参考信息 -->