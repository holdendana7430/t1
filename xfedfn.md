代发 wailian999

[U31] Py：单测
来源：http://hz.shanyushiyangtech.top/gtlhcqztba.html

python -m pytest -q
来源：http://hz.hammf.cn/gtypdkxixf.html

[U32] Py：代码格式化
来源：http://hz.aizwys.cn/gtjcblneki.html

ruff format . && ruff check --fix .
来源：http://hz.yj20258.top/gtyyutdhdw.html

[U33] Py：打包发布
来源：http://hz.jiagoushi.top/gtgrazylfk.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.chenlongwang.top/gtqgebniza.html

[U34] Py：判断编码
来源：http://hz.hnqzz.top/gtcsbunqhm.html

chardet.detect(raw)
来源：http://hz.316326.xyz/gtpmdxagwh.html

[U35] Py：发送邮件
来源：http://hz.ppjwa.cn/gtzjcgytah.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.nanxuanxn.top/gtuidzofii.html

[U36] Py：定时任务
来源：http://hz.sysykeji.top/gtpdigkjyn.html

schedule.every(10).minutes.do(job)
来源：http://hz.zycfv.cn/gtyihswtke.html

[U37] Py：读写 Excel
来源：http://hz.xuanzx.com/gtrekdsegr.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.dashuyun.cn/gtckzafsob.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhiwuduotai.top/gthzqtkrup.html

Path(__file__).resolve().parent
来源：http://hz.fengsongda.top/gtyvuojlue.html

[U39] Py：判断是否在交互环境
来源：http://hz.hywenlv.cn/gtsmdmamfn.html

sys.stdout.isatty()
来源：http://hz.dashuyun.cn/gtpalwqogf.html

[U40] Py：打印到标准错误
来源：http://hz.jyoumei.cn/gtqxdwywlp.html

print("err", file=sys.stderr)
来源：http://hz.bjfxy.top/gtiyyougiu.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.gaohongyu789.top/gtseawmvmh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.shanyushiyangkeji.top/gtiokorywp.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.ywan-chungtsiang.top/gtwdubmpfa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.chenzaomai.com/gtmilpuehq.html

[U43] PHP：声明命名空间
来源：http://hz.vqdsnc.cn/gtdipjvxsx.html

namespace App\Http;
来源：http://hz.zhoulong.xyz/gtjyrwqnzr.html

[U44] PHP：开启严格类型
来源：http://hz.yj20258.top/gtnlcympdd.html

declare(strict_types=1);
来源：http://hz.yongpay.top/gttgxafbdn.html

[U45] PHP：类型声明与返回类型
来源：http://hz.gotoacloud.top/gtbrzbahdh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yvedp.cn/gtsxrbgmdg.html

[U46] PHP：可空类型
来源：http://hz.9152youxi.cn/gtvocpatqe.html

?string $name = null
来源：http://hz.jlsjyb.cn/gtuohgaugv.html

[U47] PHP：联合类型
来源：http://hz.bjfxy.top/gtporzgavb.html

int|string $id
来源：http://hz.mhx1999.top/gtklagyqss.html

[U48] PHP：纯枚举
来源：http://hz.zycfv.cn/gtikviwsze.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.daxiang520.top/gtvuwqfvqe.html

[U49] PHP：只读属性
来源：http://hz.9152youxi.cn/gtsrbyqelp.html

public readonly string $name
来源：http://hz.zhongyouzk.top/gtwkxocnws.html

[U50] PHP：构造器属性提升
来源：http://hz.yueranfly.top/gtyukdmarb.html

public function __construct(private int $id) {}
来源：http://hz.gaohongyu789.top/gtopjudspe.html

[U51] PHP：数组解构
来源：http://hz.nwbrower.top/gtxxxkiawn.html

[$a, $b] = $arr;
来源：http://hz.shzxlz.cn/gtxigidugk.html

[U52] PHP：箭头函数
来源：http://hz.yuxming.cn/gtmpchheiw.html

$double = fn($x) => $x * 2;
来源：http://hz.yj20258.top/gtqoezldza.html

[U53] PHP：空合并运算符
来源：http://hz.c1oappe.top/gtpmkqkwpq.html

$v = $a ?? $b ?? "default";
来源：http://hz.redwolf501.top/gtscjcteds.html

[U54] PHP：空安全调用
来源：http://hz.iojbl.cn/gtyknkcmsd.html

$obj?->method()
来源：http://hz.pengpengdd.cyou/gtwzxlntcy.html

[U55] PHP：match 表达式
来源：http://hz.ydjk.org.cn/gtaggtxklk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.sufxvd.cn/gteracaqpf.html

[U56] PHP：命名参数
来源：http://hz.zdqjudy.top/gtfxssyxbk.html

f(a: 1, b: 2)
来源：http://hz.daxiang520.top/gteorchylh.html

[U57] PHP：字符串插值
来源：http://hz.pengpengdd.cyou/gtksiquvju.html

"值: {$a}"
来源：http://hz.iojbl.cn/gtoawbtcit.html

[U58] PHP：数组三件套
来源：http://hz.pengpengdd.cyou/gtllipmwxa.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zycfv.cn/gttthmpozt.html

[U59] PHP：自定义排序
来源：http://hz.fengsongda.top/gtoqelehdn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yangfankeji.com/gtobdvrdbt.html

[U60] PHP：JSON 编解码
来源：http://hz.jinyuanbaomall.cn/gtelpiybvg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhiwuduotai.top/gtohangsai.html

[U61] PHP：正则
来源：http://hz.zhiwuduotai.top/gtmxnupvcl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhixingplan.top/gtovrizwob.html

[U62] PHP：日期对象
来源：http://hz.jiagoushi.top/gttpbtydgf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.fzhhl.top/gtjowtidey.html

[U63] PHP：文件读写
来源：http://hz.jinyuanbaomall.cn/gtqfztivjf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.hongshengwenyu.top/gtczxsdqfn.html

[U64] PHP：目录遍历
来源：http://hz.nanxuanxn.top/gtjzmdtzwa.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.mhx1999.top/gtblegaavx.html

[U65] PHP：会话
来源：http://hz.wangdashe.top/gthqjoyzqf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jianghu66.top/gtnxysugbl.html

[U66] PHP：设置 Cookie
来源：http://hz.ydjk.org.cn/gtildxogkp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jqgufenzy.top/gtwvtlqvby.html

[U67] PHP：处理文件上传
来源：http://hz.yanxiufei.cn/gtunndxbrq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.meibo888.top/gtxtcpxctb.html

[U68] PHP：PDO 连接
来源：http://hz.gaohongyu789.top/gtwaigrxcb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jlsjyb.cn/gtgcwybobt.html

[U69] PHP：PDO 预处理
来源：http://hz.shuidangran.top/gttgekiojg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.svipenyu.cn/gtkvenrmig.html

[U70] PHP：PDO 事务
来源：http://hz.hammf.cn/gtdbkumncj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.cqqwz.cn/gtfrppkezt.html

[U71] PHP：抛出异常
来源：http://hz.iojbl.cn/gtwyrmpglq.html

throw new RuntimeException("失败", 500);
来源：http://hz.guowangkeji.top/gteakvtljk.html

[U72] PHP：写错误日志
来源：http://hz.zhaomingkeji.xyz/gtebpmvaqq.html

error_log("失败: " . $e->getMessage());
来源：http://hz.cucudq.cn/gtguhpksmq.html

[U73] PHP：读取 ini 配置
来源：http://hz.sufxvd.cn/gtbimmdayi.html

parse_ini_file("config.ini", true)
来源：http://hz.pycfn.com/gtppmfnbdv.html

[U74] PHP：读取环境变量
来源：http://hz.shanyushiyangtech.top/gtdvxzgieh.html

getenv("APP_ENV") ?: "production"
来源：http://hz.quarkkingdee.top/gtjrsxjpos.html

[U75] PHP：依赖注入
来源：http://hz.yj202588.top/gtcfsmxfcc.html

composer require psr/container
来源：http://hz.havefunace.top/gtehutnskd.html

[U76] PHP：简单路由
来源：http://hz.ivvv.top/gtqyfzoubr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.cashguo.top/gtydozgwln.html

[U77] PHP：模板渲染
来源：http://hz.aizwys.cn/gtnlrsngkf.html

composer require twig/twig
来源：http://hz.dashuyun.cn/gtcswkmhco.html

[U78] PHP：单元测试
来源：http://hz.iojbl.cn/gtizfltliz.html

composer require --dev phpunit/phpunit
来源：http://hz.xziqi.cn/gtomdofhks.html

[U79] PHP：静态分析
来源：http://hz.andypj.xyz/gthnimrweg.html

composer require --dev phpstan/phpstan
来源：http://hz.c1oappe.top/gtizcujnux.html

[U80] PHP：代码规范修复
来源：http://hz.zycfv.cn/gtshhluges.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.cashguo.top/gthygyihtb.html

[U81] JS：初始化项目
来源：http://hz.xingfuxueyuan.xyz/gtegwqocvh.html

npm init -y;  npm i express
来源：http://hz.xylfe.cn/gtndaawddj.html

[U82] JS：package.json 脚本
来源：http://hz.svipenyu.cn/gtqopnssfo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hongshengwenyu.top/gtbyhrpsmi.html

[U83] JS：ES Module 导入导出
来源：http://hz.shuidangran.top/gtzvoskceq.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.aizwys.cn/gtjailerdu.html

[U84] JS：CommonJS 写法
来源：http://hz.kuanghao11.cn/gtjkveyspw.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.redwolf501.top/gtvtgzvrpp.html

[U85] JS：可选链
来源：http://hz.hfpthk.cn/gtqehuoekk.html

a?.b?.c
来源：http://hz.zdqjudy.top/gtcdnbdpgr.html

[U86] JS：空值合并
来源：http://hz.aizwys.cn/gtyekzhduu.html

a ?? b
来源：http://hz.aibaodan.cn/gtxahsisnd.html

[U87] JS：解构默认值
来源：http://hz.jianghu66.top/gtnzavjxma.html

const { a = 1, b = 2 } = obj;
来源：http://hz.ppjwa.cn/gtidmtrqeb.html

[U88] JS：对象展开合并
来源：http://hz.zhiwuduotai.top/gtkwibmume.html

{ ...a, ...b }
来源：http://hz.yj20258.top/gtrukjwtld.html

[U89] JS：数组去重
来源：http://hz.chenlongwang.top/gtueiudcsu.html

[...new Set(arr)]
来源：http://hz.jlsjyb.cn/gtqvalsuui.html

[U90] JS：数字数组排序
来源：http://hz.ppjwa.cn/gtcyhotbco.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hnqzz.top/gtwxbipugh.html

[U91] JS：对象键值遍历
来源：http://hz.feifeiyinyue.top/gtagifurbg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.cdnleiting.top/gtrmyvwzmq.html

[U92] JS：深拷贝
来源：http://hz.ydjk.org.cn/gthbfajtzs.html

structuredClone(obj)
来源：http://hz.yanxiufei.cn/gtahtmckcx.html

[U93] JS：模板字符串
来源：http://hz.pycfn.com/gtrobsmplj.html

`共 ${n} 条`
来源：http://hz.zhoulong.xyz/gtkhutknpd.html

[U94] JS：箭头函数
来源：http://hz.quarkkingdee.top/gtxdtqgcto.html

const double = x => x * 2;
来源：http://hz.sxryk.cn/gtgkfmsnap.html

[U95] JS：Promise 包装
来源：http://hz.hammf.cn/gtyyrqarpz.html

new Promise((resolve, reject) => {})
来源：http://hz.316326.xyz/gtwbeneold.html

[U96] JS：async/await 与异常
来源：http://hz.iojbl.cn/gtbhesdtom.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.sufxvd.cn/gtburqrmxi.html

[U97] JS：并发请求
来源：http://hz.meibo888.top/gttlvfmtfi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yangfankeji.com/gtqsuixkoi.html

[U98] JS：fetch 带 JSON
来源：http://hz.sysykeji.top/gtdjhlfkzs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hysaishi.cn/gthuzucecd.html

[U99] JS：事件监听
来源：http://hz.shzxlz.cn/gtcnstxpdp.html

el.addEventListener("click", e => {})
来源：http://hz.yueranfly.top/gtmnqnwwtt.html

[U100] JS：DOM 查询
来源：http://hz.hammf.cn/gtqwtlqfza.html

document.querySelector(".item")
来源：http://hz.redwolf501.top/gtuqxdgtnv.html

[U101] JS：classList 操作
来源：http://hz.jqgfzy.top/gtihrfgngw.html

el.classList.toggle("active")
来源：http://hz.ydjk.org.cn/gtbpmpshsa.html

[U102] JS：本地存储
来源：http://hz.gaohongyu789.top/gtatsbaioa.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.sweek.top/gtflvrqwwf.html

[U103] JS：定时器
来源：http://hz.zhongyouzk.top/gtjbrqvuvm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.sxryk.cn/gtsdhybaso.html

[U104] JS：防抖
来源：http://hz.zhiwuduotai.top/gtmnmwdazh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aibaodan.cn/gtsywpizxt.html

[U105] JS：节流
来源：http://hz.shanyushiyangtech.top/gtokrqbigs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jinqigufen.top/gtkkesbqei.html

[U106] JS：日期格式化
来源：http://hz.ywan-chungtsiang.top/gtffjkxbct.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.hysaishi.cn/gtjamtcjwj.html

[U107] JS：数字千分位
来源：http://hz.ydjk.org.cn/gtyyjzcnmx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jinyuanbaomall.cn/gtcsmkrryy.html

[U108] JS：随机整数
来源：http://hz.9152youxi.cn/gtcrksmtaa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.pycfn.com/gtqcettqtk.html

[U109] JS：数组分组
来源：http://hz.xingfuxueyuan.xyz/gtitkvxfno.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yonumen.top/gtvsfokccu.html

[U110] JS：数组分块
来源：http://hz.andypj.xyz/gtrettxith.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.tian-w.cn/gtgstzzmzb.html

[U111] JS：对象转 Map
来源：http://hz.meibo888.top/gthwvxviyl.html

new Map(Object.entries(obj))
来源：http://hz.hysaishi.cn/gtnfbeybvf.html

[U112] JS：字符串补位
来源：http://hz.jqgufenzy.top/gtgodyskfy.html

"7".padStart(3, "0")
来源：http://hz.xuanzx.com/gtistkorvt.html

[U113] JS：正则替换全部
来源：http://hz.xylfe.cn/gtdlwsqoww.html

s.replaceAll("a", "b")
来源：http://hz.jinqigfzy.top/gtekisnhmu.html

[U114] JS：JSON 深比较
来源：http://hz.hongshengwenyu.top/gtdgjqmgla.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tian-w.cn/gttjqucxym.html

[U115] JS：生成 UUID
来源：http://hz.pengpengdd.cyou/gtzywgqphp.html

crypto.randomUUID()
来源：http://hz.hfpthk.cn/gtuvdgiesi.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hongshengwenyu.top/gtjzvyepkp.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zhixingplan.top/gtnbfikegb.html

[U117] JS：单元测试
来源：http://hz.hongshengwenyu.top/gtgcqcbnyb.html

npm i -D vitest;  npx vitest
来源：http://hz.ydzc1.top/gtjkxoxfrw.html

[U118] JS：开发服务器
来源：http://hz.yangfankeji.com/gtdvifafho.html

npm i -D vite;  npx vite
来源：http://hz.9152youxi.cn/gtjeyerpei.html

[U119] JS：生产构建
来源：http://hz.nanxuanxn.top/gtyrmqctwe.html

npx vite build
来源：http://hz.shzxlz.cn/gtxgbamxjw.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hongshengwenyu.top/gtdkwtozro.html

import.meta.env.VITE_API_URL
来源：http://hz.iojbl.cn/gtmtaacvnf.html

================================================================================
来源：http://hz.xuanzx.com/gturngkpzu.html

统计汇总
来源：http://hz.yj20258888.top/gtufxjhesr.html

================================================================================
来源：http://hz.jianghu66.top/gthvsitxnq.html

按语言统计（条）：
来源：http://hz.aizwys.cn/gtkqenbwdl.html

Python ......... 252
来源：http://hz.sufxvd.cn/gtqvakqkwj.html

PHP ............ 252
来源：http://hz.ydzc1.top/gtdzbglong.html

JavaScript ..... 252
来源：http://hz.ehwqpu.com/gtgfhwxdky.html

TypeScript ..... 212
来源：http://hz.hammf.cn/gtvfnpiaxs.html

Java ........... 212
来源：http://hz.daria6918.cn/gtjffsgdza.html

Go ............. 212
来源：http://hz.ywan-chungtsiang.top/gtdnghanfp.html

Ruby ........... 212
来源：http://hz.sweek.top/gtkekrkoct.html

C# ............. 212
来源：http://hz.sxryk.cn/gtlmyuufjt.html

C .............. 30
来源：http://hz.sweek.top/gtilmhvxma.html

C++ ............ 30
来源：http://hz.xingfuxueyuan.xyz/gtjprthnmt.html

SQL ............ 90
来源：http://hz.haohaochexian.top/gtgotomfky.html

Bash ........... 80
来源：http://hz.tianlin.xyz/gthtsfpjtp.html

Kotlin ......... 15
来源：http://hz.hongshengwenyu.top/gtijeyevhm.html

Swift .......... 15
来源：http://hz.nwbrower.top/gtnlekqvoz.html

Lua ............ 10
来源：http://hz.zhaomingkeji.xyz/gtcftmyxvn.html

Perl ........... 10
来源：http://hz.yvedp.cn/gtucmvapfm.html

Scala .......... 10
来源：http://hz.chenjidiqi.icu/gtdrlngvek.html

------------------------------------
来源：http://hz.chenlongwang.top/gtjmiaqysx.html

合计 ........... 2106 条
来源：http://hz.guowangkeji.top/gtbusdstdp.html

按章节统计：
来源：http://hz.yj20258888.top/gtennsbuqw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.aizwys.cn/gtuxblnuno.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.chenjidiqi.icu/gturdeunmq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.52xcode.cn/gtwlcmyatq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jyoumei.cn/gtuugarajh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.cdnleiting.top/gttgqhvmqa.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yonumen.top/gtdhllihmg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hysaishi.cn/gtobxjcjtj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zdqjudy.top/gthtovoojb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.hnxiangtu.top/gtptmuxcca.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.tanke756.top/gtfwatmyfx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yj20258888.top/gthbkqycog.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhengqikj.top/gtdrgycvfe.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.quarkkingdee.top/gtevlngclw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.52xcode.cn/gtzymmzjwj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.guannengcc.top/gtcnbjvlgt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.birdmap.top/gtksacmlnm.html

Q SQL 专题                              90
来源：http://hz.iojbl.cn/gtrfbqqtgr.html

R Bash 专题                             80
来源：http://hz.shuidangran.top/gthedgjiri.html

S C / C++ 专题                          60
来源：http://hz.hysaishi.cn/gtyzzkiscg.html

T 其他语言补充                          60
来源：http://hz.redwolf501.top/gtbmsxpdlk.html

U 高频实用片段                         120
来源：http://hz.svipenyu.cn/gtvltlphfs.html

------------------------------------
来源：http://hz.shzxlz.cn/gtsoqxkyrb.html

合计                                  2106 条
来源：http://hz.daxiang520.top/gtazwamjqs.html

--------------------------------------------------------------------------------
来源：http://hz.iojbl.cn/gtrbtpfabv.html

使用提醒
来源：http://hz.hammf.cn/gtqrfibqlo.html

--------------------------------------------------------------------------------
来源：http://hz.dianchejie.cn/gtgkifcpqj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.hnqzz.top/gtjurgqgbj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yuanzhike.top/gtiyngeenu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.nwbrower.top/gtlaimbhml.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jinqigfzy.top/gtzxdjrokf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.aibaodan.cn/gtutidutzf.html

—— 文件结束 ——
来源：http://hz.sweek.top/gtvgvlangl.html

================================================================================
来源：http://hz.yuxming.cn/gtjlcrrlir.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.shanyushiyangkeji.top/gtqhsexffy.html

Common Programming Examples Cheat Book
来源：http://hz.xuanzx.com/gttrncedxw.html

================================================================================
来源：http://hz.haohaochexian.top/gtzrvfqnub.html

【收录内容】
来源：http://hz.hongshengwenyu.top/gtyflyzmgl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.gzhubu.top/gtsxvpropu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jqgfzy.top/gtlwunhgyk.html

SQL · Bash · C · C++
来源：http://hz.chenjidiqi.icu/gtedhxvnjw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.andypj.xyz/gtfeejpcof.html

【使用说明】
来源：http://hz.havefunace.top/gtcctebwas.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.jinyuanbaomall.cn/gtgogbgsid.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.ppjwa.cn/gtsmthpicp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.ydjk.org.cn/gtaloaqbmu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yvedp.cn/gtxkkbyckl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.gogol.net.cn/gtzvjpoygl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.gogol.net.cn/gtwbgockfl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.sxryk.cn/gtijxmapim.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.feifeiyinyue.top/gtrdgcoodr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.bjfxy.top/gtybzeamic.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.bjfxy.top/gtchfgcpwm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhoulong.xyz/gtttzvbxgs.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.hammf.cn/gtqblknvok.html

【文件统计】
来源：http://hz.ydjk.org.cn/gtmailvotp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ehwqpu.com/gtlsojiggv.html

--------------------------------------------------------------------------------
来源：http://hz.0kj1m.cn/gtgzwebjsl.html

目  录
来源：http://hz.nanxuanxn.top/gtbmsbtted.html

--------------------------------------------------------------------------------
来源：http://hz.jlsjyb.cn/gtzwahxxnp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.bjfxy.top/gtynvhuxvu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jinghuilouyu.cn/gtmzahjzfg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.ydjk.org.cn/gtzmtafbvh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.chenjidiqi.icu/gtozuovtbe.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jiagoushi.top/gtfwtujwew.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.xylfe.cn/gtvcvuemtf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jqgufenzy.top/gtxgohkscw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.ivvv.top/gthdqbkagc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.ehwqpu.com/gteldlqtdr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.52xcode.cn/gtgxycpkrb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.gogol.net.cn/gtxghhhhzf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.ydjk.org.cn/gtxsjtwpoj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.yuxming.cn/gtuqqtdhjm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.bjfxy.top/gtetmyklwy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.ppjwa.cn/gtgpltwpgf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.pycfn.com/gtjuwxddng.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zycfv.cn/gtcobajcwn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.zhoulong.xyz/gtkidnmtbg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yangfankeji.com/gtfepzblxz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinyuanbaomall.cn/gtedfdncgj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.svipenyu.cn/gtyhhpdrbm.html

================================================================================
来源：http://hz.xinyue.icu/gtcgijwalf.html

A. 基础语法与类型
来源：http://hz.gaohongyu789.top/gtmgluqvpo.html

================================================================================
来源：http://hz.0kj1m.cn/gtcaixydhx.html

[A01] Hello World
来源：http://hz.yuanzhike.top/gtwqkcodtk.html

Py:   print("Hello, World!")
来源：http://hz.jinghuilouyu.cn/gtghlqlkfa.html

PHP:  echo "Hello, World!";
来源：http://hz.birdmap.top/gtzvprhamz.html

JS:   console.log("Hello, World!");
来源：http://hz.xuanzx.com/gtsalmbldm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.52xcode.cn/gttzyskmen.html

Java: System.out.println("Hello, World!");
来源：http://hz.jqgfzy.top/gtkogyyicp.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.jqgufenzy.top/gtoorrebvc.html

Ruby: puts "Hello, World!"
来源：http://hz.chenlongwang.top/gtmwnmsocb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.c1oappe.top/gttmbdohck.html

[A02] 变量声明与赋值
来源：http://hz.andypj.xyz/gtaeffyoxt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.dianchejie.cn/gtqfrmkveg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.9152youxi.cn/gtyjchiqev.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.quarkkingdee.top/gtzxsyzzlz.html


<!-- 参考信息 -->