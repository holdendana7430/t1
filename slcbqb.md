代发 wailian999

[U31] Py：单测
来源：http://hz.guannengcc.top/gtehnkdnou.html

python -m pytest -q
来源：http://hz.wangshuangyany.cn/gtdhosknrq.html

[U32] Py：代码格式化
来源：http://hz.wangshuangyany.cn/gttiqosarr.html

ruff format . && ruff check --fix .
来源：http://hz.0kj1m.cn/gtcnhbhbqi.html

[U33] Py：打包发布
来源：http://hz.yuanzhike.top/gtaivhabju.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hnqzz.top/gttkeihloj.html

[U34] Py：判断编码
来源：http://hz.cucudq.cn/gtqmrthxtd.html

chardet.detect(raw)
来源：http://hz.zhengqikj.top/gttwwsyzkl.html

[U35] Py：发送邮件
来源：http://hz.dashuyun.cn/gtcrzamgrz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.ehwqpu.com/gtnxfnsfbn.html

[U36] Py：定时任务
来源：http://hz.xuanzx.com/gtvzmbeqfw.html

schedule.every(10).minutes.do(job)
来源：http://hz.gogol.net.cn/gttcsnlqsr.html

[U37] Py：读写 Excel
来源：http://hz.guannengcc.top/gtamsawnxp.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hnxiangtu.top/gtyryexotr.html

[U38] Py：获取脚本所在目录
来源：http://hz.hnqzz.top/gtylhwnvqs.html

Path(__file__).resolve().parent
来源：http://hz.yongpay.top/gtbsfdstks.html

[U39] Py：判断是否在交互环境
来源：http://hz.svipenyu.cn/gtvsvtjuey.html

sys.stdout.isatty()
来源：http://hz.yj20258888.top/gtjopiblia.html

[U40] Py：打印到标准错误
来源：http://hz.quarkkingdee.top/gtljocghqc.html

print("err", file=sys.stderr)
来源：http://hz.aibaodan.cn/gtyzdvdyuj.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.xinyue.icu/gtywuuuval.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.haohaochexian.top/gtzmlkehtt.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.pengpengdd.cyou/gttoisemnw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jqgfzy.top/gtoocfptcv.html

[U43] PHP：声明命名空间
来源：http://hz.xziqi.cn/gtxwohthnf.html

namespace App\Http;
来源：http://hz.jlsjyb.cn/gttwanmrzw.html

[U44] PHP：开启严格类型
来源：http://hz.zhengqikj.top/gtbcieckxl.html

declare(strict_types=1);
来源：http://hz.chenjidiqi.icu/gtkyzsqnlo.html

[U45] PHP：类型声明与返回类型
来源：http://hz.daria6918.cn/gtvwhhqoqq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cqqwz.cn/gtmtmtvbbp.html

[U46] PHP：可空类型
来源：http://hz.yj20258.top/gtuusslsmk.html

?string $name = null
来源：http://hz.ybcxt.top/gtwehvwqis.html

[U47] PHP：联合类型
来源：http://hz.cucudq.cn/gtkkfrtrwo.html

int|string $id
来源：http://hz.jlsjyb.cn/gtsnotmnpb.html

[U48] PHP：纯枚举
来源：http://hz.jyoumei.cn/gtdlvxdbqc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jinyuanbaomall.cn/gtmtzvjysr.html

[U49] PHP：只读属性
来源：http://hz.nanxinkj.top/gtybedgdwd.html

public readonly string $name
来源：http://hz.smart0.xyz/gtlwxpwjro.html

[U50] PHP：构造器属性提升
来源：http://hz.jianghu66.top/gtcydfojyn.html

public function __construct(private int $id) {}
来源：http://hz.sufxvd.cn/gtjjclsiss.html

[U51] PHP：数组解构
来源：http://hz.zhijiandao.cn/gtjdxgukfr.html

[$a, $b] = $arr;
来源：http://hz.havefunace.top/gtgjooyitw.html

[U52] PHP：箭头函数
来源：http://hz.iojbl.cn/gtetgxrerg.html

$double = fn($x) => $x * 2;
来源：http://hz.gzhubu.top/gthjlqghcm.html

[U53] PHP：空合并运算符
来源：http://hz.gogol.net.cn/gtudazrwdm.html

$v = $a ?? $b ?? "default";
来源：http://hz.wangshuangyany.cn/gtiyvfzodg.html

[U54] PHP：空安全调用
来源：http://hz.havefunace.top/gtkxjemmgd.html

$obj?->method()
来源：http://hz.mhx1999.top/gtobxynxvl.html

[U55] PHP：match 表达式
来源：http://hz.jiagoushi.top/gtffvbbvot.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.shangyingyoupin.top/gtvyrbigkr.html

[U56] PHP：命名参数
来源：http://hz.gotoacloud.top/gttujtpzzd.html

f(a: 1, b: 2)
来源：http://hz.52xcode.cn/gtjhujpnuh.html

[U57] PHP：字符串插值
来源：http://hz.shanyushiyangtech.top/gtikpydevu.html

"值: {$a}"
来源：http://hz.shangyingyoupin.top/gtsbsylspj.html

[U58] PHP：数组三件套
来源：http://hz.nanxuanxn.top/gtzzydbgzb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.9152youxi.cn/gtijtsdwhb.html

[U59] PHP：自定义排序
来源：http://hz.shzxlz.cn/gtznevxjoe.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hysaishi.cn/gtjxgqvsjf.html

[U60] PHP：JSON 编解码
来源：http://hz.yongpay.top/gtbpnbvsht.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.cqqwz.cn/gtcihxygkd.html

[U61] PHP：正则
来源：http://hz.zhaomingkeji.xyz/gtovmifxbw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinghuilouyu.cn/gtlpdhgxja.html

[U62] PHP：日期对象
来源：http://hz.jqgfzy.top/gtcegobrhf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.9152youxi.cn/gteswbtkwy.html

[U63] PHP：文件读写
来源：http://hz.ydjk.org.cn/gtdqmjfxtr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.guowangkeji.top/gthxdoasxv.html

[U64] PHP：目录遍历
来源：http://hz.jyoumei.cn/gtncbwsmig.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.nanxinkj.top/gtsfzabhni.html

[U65] PHP：会话
来源：http://hz.aizwys.cn/gtozgnbxta.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.daxiang520.top/gtcrblzeqp.html

[U66] PHP：设置 Cookie
来源：http://hz.fengsongda.top/gtsnejiobb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.gotoacloud.top/gttiuqcgbs.html

[U67] PHP：处理文件上传
来源：http://hz.jinqigfzy.top/gtejbfbykx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.kuanghao11.cn/gtvziltfse.html

[U68] PHP：PDO 连接
来源：http://hz.smart0.xyz/gtpnymnoaw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yj20258.top/gtaoboipsg.html

[U69] PHP：PDO 预处理
来源：http://hz.xylfe.cn/gtzhbwwkaz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.quarkkingdee.top/gtbcmgeymz.html

[U70] PHP：PDO 事务
来源：http://hz.xylfe.cn/gtufoxdohz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.xingfuxueyuan.xyz/gtfodvtncc.html

[U71] PHP：抛出异常
来源：http://hz.yongpay.top/gtwkrxkenk.html

throw new RuntimeException("失败", 500);
来源：http://hz.guannengcc.top/gthaeeluej.html

[U72] PHP：写错误日志
来源：http://hz.ywan-chungtsiang.top/gtwpvdgedn.html

error_log("失败: " . $e->getMessage());
来源：http://hz.guowangkeji.top/gttsjxwoki.html

[U73] PHP：读取 ini 配置
来源：http://hz.yueranfly.top/gtlrnmxoco.html

parse_ini_file("config.ini", true)
来源：http://hz.yanxiufei.cn/gtmftoafgw.html

[U74] PHP：读取环境变量
来源：http://hz.xinyue.icu/gtakzrzngw.html

getenv("APP_ENV") ?: "production"
来源：http://hz.xziqi.cn/gtzxdbkupa.html

[U75] PHP：依赖注入
来源：http://hz.iojbl.cn/gtxsrjmwnt.html

composer require psr/container
来源：http://hz.xuanzx.com/gtfjhiayyt.html

[U76] PHP：简单路由
来源：http://hz.yj20258888.top/gtkiusremk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hnqzz.top/gtvpyfcxun.html

[U77] PHP：模板渲染
来源：http://hz.shangyingyoupin.top/gtneozmazw.html

composer require twig/twig
来源：http://hz.meibo888.top/gtiswxvyck.html

[U78] PHP：单元测试
来源：http://hz.guowangkeji.top/gtjsprljxj.html

composer require --dev phpunit/phpunit
来源：http://hz.shanyushiyangtech.top/gtapxwtlku.html

[U79] PHP：静态分析
来源：http://hz.sweek.top/gtmiqpuwle.html

composer require --dev phpstan/phpstan
来源：http://hz.kuanghao11.cn/gtimymfnwq.html

[U80] PHP：代码规范修复
来源：http://hz.zhijiandao.cn/gtrbzheyrl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.shanyushiyangtech.top/gtlukzpmco.html

[U81] JS：初始化项目
来源：http://hz.zhijiandao.cn/gtvvsmtmce.html

npm init -y;  npm i express
来源：http://hz.cucudq.cn/gtmmwzxbti.html

[U82] JS：package.json 脚本
来源：http://hz.hysaishi.cn/gtfksomypi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.c1oappe.top/gttmzltuve.html

[U83] JS：ES Module 导入导出
来源：http://hz.jinqigufen.top/gtbddvklnz.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zhiwuduotai.top/gtbjngfdkd.html

[U84] JS：CommonJS 写法
来源：http://hz.hnxiangtu.top/gtezpticdq.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.quarkkingdee.top/gtcrfdwweh.html

[U85] JS：可选链
来源：http://hz.fzhhl.top/gtidhxutgj.html

a?.b?.c
来源：http://hz.wangshuangyany.cn/gtnnsarzwh.html

[U86] JS：空值合并
来源：http://hz.hywenlv.cn/gtpqlonkip.html

a ?? b
来源：http://hz.yj20258888.top/gtefvtkszb.html

[U87] JS：解构默认值
来源：http://hz.zhiwuduotai.top/gtyemdaewf.html

const { a = 1, b = 2 } = obj;
来源：http://hz.daria6918.cn/gtrezctick.html

[U88] JS：对象展开合并
来源：http://hz.ywan-chungtsiang.top/gtlthtflbs.html

{ ...a, ...b }
来源：http://hz.316326.xyz/gtbrfimhuv.html

[U89] JS：数组去重
来源：http://hz.chenlongwang.top/gtgeecwldk.html

[...new Set(arr)]
来源：http://hz.cdnleiting.top/gtaoetptpo.html

[U90] JS：数字数组排序
来源：http://hz.ywan-chungtsiang.top/gtezggwrli.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jinqigufen.top/gtmfypiejk.html

[U91] JS：对象键值遍历
来源：http://hz.tianlin.xyz/gthgaqxxkv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jianghu66.top/gtioaygjny.html

[U92] JS：深拷贝
来源：http://hz.snrcjt.cn/gtslnzaqbh.html

structuredClone(obj)
来源：http://hz.haohaochexian.top/gtoeaxnaeo.html

[U93] JS：模板字符串
来源：http://hz.feifeiyinyue.top/gtvdgjdzjg.html

`共 ${n} 条`
来源：http://hz.xuetiantiany.cn/gtyzvaocoo.html

[U94] JS：箭头函数
来源：http://hz.cucudq.cn/gtgxnqkmli.html

const double = x => x * 2;
来源：http://hz.hysaishi.cn/gtzqkfcmau.html

[U95] JS：Promise 包装
来源：http://hz.sweek.top/gtwblurbcj.html

new Promise((resolve, reject) => {})
来源：http://hz.xziqi.cn/gtwsdhrwjo.html

[U96] JS：async/await 与异常
来源：http://hz.jinqigufen.top/gtqnfhpxsv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zhiwuduotai.top/gtjojrvinx.html

[U97] JS：并发请求
来源：http://hz.zhongyouzk.top/gthwsirhdc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cdnleiting.top/gtdoynygsa.html

[U98] JS：fetch 带 JSON
来源：http://hz.redwolf501.top/gtdayhlrej.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yueranfly.top/gtowaqkhfu.html

[U99] JS：事件监听
来源：http://hz.zycfv.cn/gtmfeogrwk.html

el.addEventListener("click", e => {})
来源：http://hz.mhx1999.top/gtdpezcpzb.html

[U100] JS：DOM 查询
来源：http://hz.ywan-chungtsiang.top/gtetjehfcv.html

document.querySelector(".item")
来源：http://hz.zhijiandao.cn/gtumkdtxcl.html

[U101] JS：classList 操作
来源：http://hz.jinghuilouyu.cn/gthroqtzdg.html

el.classList.toggle("active")
来源：http://hz.ybcxt.top/gtyunuyfbq.html

[U102] JS：本地存储
来源：http://hz.zhoulong.xyz/gtvzabjwly.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.hammf.cn/gttxhwjjdt.html

[U103] JS：定时器
来源：http://hz.svipenyu.cn/gttsflzxfz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hysaishi.cn/gtpkvktrwx.html

[U104] JS：防抖
来源：http://hz.yj202588.top/gtdddbmdzu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tianlin.xyz/gtzgfirzmz.html

[U105] JS：节流
来源：http://hz.hammf.cn/gtoharlcwy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.chenlongwang.top/gtryiwrgtl.html

[U106] JS：日期格式化
来源：http://hz.guannengcc.top/gtkhcceybc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.hnxiangtu.top/gtwxhgicyb.html

[U107] JS：数字千分位
来源：http://hz.sweek.top/gtluknffdt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.fengsongda.top/gtwtqloubc.html

[U108] JS：随机整数
来源：http://hz.9152youxi.cn/gtueessjoi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.sufxvd.cn/gtxikxcygj.html

[U109] JS：数组分组
来源：http://hz.xylfe.cn/gtuiulmxts.html

Object.groupBy(arr, x => x.type)
来源：http://hz.meibo888.top/gtjbdqbewd.html

[U110] JS：数组分块
来源：http://hz.nwbrower.top/gtwewryixa.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.cucudq.cn/gtuugxqjte.html

[U111] JS：对象转 Map
来源：http://hz.sxryk.cn/gttdlnxwei.html

new Map(Object.entries(obj))
来源：http://hz.yuanzhike.top/gtzzqwecuc.html

[U112] JS：字符串补位
来源：http://hz.zhoulong.xyz/gtvbtyezdw.html

"7".padStart(3, "0")
来源：http://hz.hywenlv.cn/gthgmyzoqm.html

[U113] JS：正则替换全部
来源：http://hz.yj20258.top/gthgpcrruq.html

s.replaceAll("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtrsyzcspc.html

[U114] JS：JSON 深比较
来源：http://hz.jinqigfzy.top/gtuhgwiwft.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ppjwa.cn/gtgopynptx.html

[U115] JS：生成 UUID
来源：http://hz.cheryme.top/gtrosfzaky.html

crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtrfntrofw.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.guowangkeji.top/gtoecfxgig.html

/** @param {string} name */ function f(name) {}
来源：http://hz.cheryme.top/gtmbcwxhby.html

[U117] JS：单元测试
来源：http://hz.sufxvd.cn/gtaocgxxqn.html

npm i -D vitest;  npx vitest
来源：http://hz.zhiwuduotai.top/gtklahjtun.html

[U118] JS：开发服务器
来源：http://hz.jqgufenzy.top/gtsfuspzjp.html

npm i -D vite;  npx vite
来源：http://hz.zhoulong.xyz/gtsxatfqtf.html

[U119] JS：生产构建
来源：http://hz.zhongyouzk.top/gtanfkztzy.html

npx vite build
来源：http://hz.shuidangran.top/gthicffaki.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.chenjidiqi.icu/gtqiezcxaz.html

import.meta.env.VITE_API_URL
来源：http://hz.hfpthk.cn/gtjukundlg.html

================================================================================
来源：http://hz.bjfxy.top/gtzjivnmnb.html

统计汇总
来源：http://hz.zhixingplan.top/gtkuetgxjx.html

================================================================================
来源：http://hz.sufxvd.cn/gtjcjadrlz.html

按语言统计（条）：
来源：http://hz.ydzc1.top/gtxthexopg.html

Python ......... 252
来源：http://hz.52xcode.cn/gtavwwwqrz.html

PHP ............ 252
来源：http://hz.yuanzhike.top/gtkftzmrgp.html

JavaScript ..... 252
来源：http://hz.hnqzz.top/gtgadbhdqq.html

TypeScript ..... 212
来源：http://hz.52xcode.cn/gtnsaqezmo.html

Java ........... 212
来源：http://hz.xylfe.cn/gtkeaikaps.html

Go ............. 212
来源：http://hz.jinqigfzy.top/gtcnovpwqh.html

Ruby ........... 212
来源：http://hz.jinqigfzy.top/gthxwdvais.html

C# ............. 212
来源：http://hz.daria6918.cn/gtdlepmdfc.html

C .............. 30
来源：http://hz.cdnleiting.top/gtdmfwyroj.html

C++ ............ 30
来源：http://hz.yongpay.top/gtebaewebi.html

SQL ............ 90
来源：http://hz.smart0.xyz/gtnwrvmzzk.html

Bash ........... 80
来源：http://hz.jianghu66.top/gtzhjxktdf.html

Kotlin ......... 15
来源：http://hz.fengsongda.top/gtilyocjaw.html

Swift .......... 15
来源：http://hz.gogol.net.cn/gtwcbzpais.html

Lua ............ 10
来源：http://hz.sweek.top/gtpeiexlph.html

Perl ........... 10
来源：http://hz.chenjidiqi.icu/gttnycidhq.html

Scala .......... 10
来源：http://hz.zhijiandao.cn/gtrjizsiyp.html

------------------------------------
来源：http://hz.yueranfly.top/gtafiabdmm.html

合计 ........... 2106 条
来源：http://hz.yuanzhike.top/gtdpuqsqky.html

按章节统计：
来源：http://hz.9152youxi.cn/gttqtjesij.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.feifeiyinyue.top/gtihjxvmlf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ydzc1.top/gtrszpiqye.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.bjfxy.top/gtdfpeaabh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.sxryk.cn/gtwyyqkpei.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hongshengwenyu.top/gtfbneujlw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.hongshengwenyu.top/gtvudvrfxw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.shanyushiyangkeji.top/gtmkocrkbr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.jinghuilouyu.cn/gtnqxcuyst.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yangfankeji.com/gtwufdxlpr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.haohaochexian.top/gtqzqgrwtf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gtbnxzjgmn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jyoumei.cn/gtommqoerx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.cdnleiting.top/gtlklwnvmx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.wangshuangyany.cn/gtzsbzlpui.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.gotoacloud.top/gtjflhzyvk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.ywan-chungtsiang.top/gtrwtdpedt.html

Q SQL 专题                              90
来源：http://hz.yangfankeji.com/gtetykpkea.html

R Bash 专题                             80
来源：http://hz.ybcxt.top/gtxzejeuwz.html

S C / C++ 专题                          60
来源：http://hz.yanxiufei.cn/gtetjpayqo.html

T 其他语言补充                          60
来源：http://hz.jqgufenzy.top/gtzlumpizy.html

U 高频实用片段                         120
来源：http://hz.yj20258888.top/gtbqlwllvl.html

------------------------------------
来源：http://hz.gotoacloud.top/gtugnsxhpy.html

合计                                  2106 条
来源：http://hz.52xcode.cn/gtufrkzrko.html

--------------------------------------------------------------------------------
来源：http://hz.xingfuxueyuan.xyz/gtxzjjrhfd.html

使用提醒
来源：http://hz.guannengcc.top/gtxobvipez.html

--------------------------------------------------------------------------------
来源：http://hz.dianchejie.cn/gtmolhipfe.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zhoulong.xyz/gtnevoswdt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zhiwuduotai.top/gtuvhsctqp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.cdnleiting.top/gtcexfsqme.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.fzhhl.top/gtrjlaclet.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yuxming.cn/gtndibddqx.html

—— 文件结束 ——
来源：http://hz.jyoumei.cn/gtxhqmnjom.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtnjswrbsi.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.316326.xyz/gttuwonivb.html

Common Programming Examples Cheat Book
来源：http://hz.wangshuangyany.cn/gtjunhjzrh.html

================================================================================
来源：http://hz.redwolf501.top/gtcplqvfkl.html

【收录内容】
来源：http://hz.hammf.cn/gtjplxqsrp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yuanzhike.top/gtllupcjfm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.quarkkingdee.top/gtwixtvder.html

SQL · Bash · C · C++
来源：http://hz.zhijiandao.cn/gtgfsfuzwz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yuxming.cn/gtjhcggauz.html

【使用说明】
来源：http://hz.yongpay.top/gthhotvcgb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.52xcode.cn/gtiufheezm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.sufxvd.cn/gtsrfhqfra.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.cashguo.top/gtleedmrvk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yuxming.cn/gtqhqvmdoa.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yj202588.top/gtxrjgcutg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yanxiufei.cn/gtophbnvyt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.gaohongyu789.top/gtsvwfdspb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.haohaochexian.top/gtgflotgpu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.guowangkeji.top/gtenwtcoxc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.pycfn.com/gtmkabgcjy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.xinyue.icu/gtvylytkuz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.wangdashe.top/gtryelimtl.html

【文件统计】
来源：http://hz.smart0.xyz/gtquyupdga.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.svipenyu.cn/gtcogbdvfl.html

--------------------------------------------------------------------------------
来源：http://hz.yj202588.top/gtoxatbrca.html

目  录
来源：http://hz.shuidangran.top/gthitcgjoy.html

--------------------------------------------------------------------------------
来源：http://hz.quarkkingdee.top/gtnainbwcx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.ivvv.top/gtifygznuq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yj202588.top/gtxupdbdko.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.iojbl.cn/gtfhslgxmp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.cqqwz.cn/gthighujvv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yanxiufei.cn/gtdotwnteq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.c1oappe.top/gtpbqoenyv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.gaohongyu789.top/gtxtdcyxjz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.dianchejie.cn/gtbfzdffyj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.havefunace.top/gteyghvlnw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.tian-w.cn/gtiikoidkw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.aizwys.cn/gtmovwfufm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.c1oappe.top/gtxlnqcral.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.fengsongda.top/gtswxpbqss.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.cashguo.top/gtbnkekmdr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.fzhhl.top/gtdwtpbhac.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.feifeiyinyue.top/gtcxdhzoak.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhengqikj.top/gtvpcbbhqe.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.gaohongyu789.top/gtaldbxjvk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.sweek.top/gtzautbomc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.316326.xyz/gtzkmbhcdb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.shanyushiyangtech.top/gtqhzjutvo.html

================================================================================
来源：http://hz.vqdsnc.cn/gtssgkkjvq.html

A. 基础语法与类型
来源：http://hz.quarkkingdee.top/gtnwozmuxy.html

================================================================================
来源：http://hz.gzhubu.top/gtvqbtfpjn.html

[A01] Hello World
来源：http://hz.shanyushiyangkeji.top/gtzkjldadf.html

Py:   print("Hello, World!")
来源：http://hz.yj20258888.top/gtbgesxpww.html

PHP:  echo "Hello, World!";
来源：http://hz.sysykeji.top/gtdkfbudrj.html

JS:   console.log("Hello, World!");
来源：http://hz.jinqigufen.top/gtsbkzowpl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.hnqzz.top/gttojvkxfh.html

Java: System.out.println("Hello, World!");
来源：http://hz.hammf.cn/gteonsaxax.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.jinyuanbaomall.cn/gtrwxkizvd.html

Ruby: puts "Hello, World!"
来源：http://hz.cheryme.top/gtzelbvqiu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.shzxlz.cn/gtzthlhjzs.html

[A02] 变量声明与赋值
来源：http://hz.ivvv.top/gtmrzpcsdi.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.nwbrower.top/gthyvksxci.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.hnxiangtu.top/gtqfhogjpm.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.mhx1999.top/gtbhljvzvo.html


<!-- 参考信息 -->