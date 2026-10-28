代发 wailian999

[U33] Py：打包发布
来源：http://hz.jinqigufen.top/gtlygoioop.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jyoumei.cn/gtpvrqkjma.html

[U34] Py：判断编码
来源：http://hz.jqgufenzy.top/gthxmwkdvv.html

chardet.detect(raw)
来源：http://hz.dianchejie.cn/gtidsvhwng.html

[U35] Py：发送邮件
来源：http://hz.gogol.net.cn/gtvegiovdh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.shzxlz.cn/gtatuitgxq.html

[U36] Py：定时任务
来源：http://hz.hywenlv.cn/gtmdbhqrhu.html

schedule.every(10).minutes.do(job)
来源：http://hz.daria6918.cn/gtowxhelkf.html

[U37] Py：读写 Excel
来源：http://hz.wangshuangyany.cn/gtwjqtitor.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.sxryk.cn/gtqnscheoz.html

[U38] Py：获取脚本所在目录
来源：http://hz.52xcode.cn/gtcmdrqdco.html

Path(__file__).resolve().parent
来源：http://hz.havefunace.top/gtcbdsjedd.html

[U39] Py：判断是否在交互环境
来源：http://hz.xuanzx.com/gttyygqbwf.html

sys.stdout.isatty()
来源：http://hz.hongshengwenyu.top/gtabbgrhfz.html

[U40] Py：打印到标准错误
来源：http://hz.sxryk.cn/gthiarirjn.html

print("err", file=sys.stderr)
来源：http://hz.xuanzx.com/gtvtbdsclb.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.svipenyu.cn/gttkmgcuba.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jyoumei.cn/gtejhmufid.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zycfv.cn/gtiswfcird.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.316326.xyz/gtxijzvosa.html

[U43] PHP：声明命名空间
来源：http://hz.iojbl.cn/gtkomzapco.html

namespace App\Http;
来源：http://hz.feifeiyinyue.top/gtahwnnhwo.html

[U44] PHP：开启严格类型
来源：http://hz.zhongyouzk.top/gtzwxieqme.html

declare(strict_types=1);
来源：http://hz.hnqzz.top/gtgcjrjfnu.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ybcxt.top/gttgpoturc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxuanxn.top/gttvmbtyns.html

[U46] PHP：可空类型
来源：http://hz.mhx1999.top/gtxvbxhgyl.html

?string $name = null
来源：http://hz.ywan-chungtsiang.top/gtmucwzvaq.html

[U47] PHP：联合类型
来源：http://hz.zhongyouzk.top/gtpdggshcf.html

int|string $id
来源：http://hz.tianlin.xyz/gtdsnqixpt.html

[U48] PHP：纯枚举
来源：http://hz.yj20258.top/gtjetqgjug.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.daxiang520.top/gtedgtehhh.html

[U49] PHP：只读属性
来源：http://hz.yvedp.cn/gtipeyvbof.html

public readonly string $name
来源：http://hz.jinqigufen.top/gtaborjqmt.html

[U50] PHP：构造器属性提升
来源：http://hz.cheryme.top/gtfaprsnve.html

public function __construct(private int $id) {}
来源：http://hz.tanke756.top/gtieuqmocv.html

[U51] PHP：数组解构
来源：http://hz.shanyushiyangtech.top/gtlzjbjehk.html

[$a, $b] = $arr;
来源：http://hz.yanxiufei.cn/gtmiwadbcb.html

[U52] PHP：箭头函数
来源：http://hz.yueranfly.top/gtagdidbzw.html

$double = fn($x) => $x * 2;
来源：http://hz.quarkkingdee.top/gtgrpmkjzj.html

[U53] PHP：空合并运算符
来源：http://hz.guannengcc.top/gtjetrawmt.html

$v = $a ?? $b ?? "default";
来源：http://hz.dianchejie.cn/gtvgzjndfv.html

[U54] PHP：空安全调用
来源：http://hz.gzhubu.top/gtusajtisc.html

$obj?->method()
来源：http://hz.xziqi.cn/gtvzisgphz.html

[U55] PHP：match 表达式
来源：http://hz.gotoacloud.top/gttrpqbtas.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.cucudq.cn/gtnsmeukzr.html

[U56] PHP：命名参数
来源：http://hz.dianchejie.cn/gtfqrbnokn.html

f(a: 1, b: 2)
来源：http://hz.xinyue.icu/gtprxdmgda.html

[U57] PHP：字符串插值
来源：http://hz.vqdsnc.cn/gtlaeswwvj.html

"值: {$a}"
来源：http://hz.zycfv.cn/gtvkgclgir.html

[U58] PHP：数组三件套
来源：http://hz.sufxvd.cn/gteekhwwtm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.shuidangran.top/gtbadavpgg.html

[U59] PHP：自定义排序
来源：http://hz.snrcjt.cn/gtarspaplq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gzhubu.top/gtwchphqdr.html

[U60] PHP：JSON 编解码
来源：http://hz.snrcjt.cn/gtakcthxll.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jqgufenzy.top/gtzgtukyxn.html

[U61] PHP：正则
来源：http://hz.wangshuangyany.cn/gtfpudehtl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hnqzz.top/gteypkzjjw.html

[U62] PHP：日期对象
来源：http://hz.pycfn.com/gtfrngyuux.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jinghuilouyu.cn/gtpprgbzka.html

[U63] PHP：文件读写
来源：http://hz.jlsjyb.cn/gtyyvgwevb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jinqigufen.top/gtbcqwjgcs.html

[U64] PHP：目录遍历
来源：http://hz.xylfe.cn/gtsquuhkmm.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.wangshuangyany.cn/gttviwnzso.html

[U65] PHP：会话
来源：http://hz.yueranfly.top/gthwumqupd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jiagoushi.top/gtsrmwherr.html

[U66] PHP：设置 Cookie
来源：http://hz.daria6918.cn/gtrnznfexs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhixingplan.top/gtokcuwiua.html

[U67] PHP：处理文件上传
来源：http://hz.zhijiandao.cn/gtflllnvre.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.xylfe.cn/gtspcpigjg.html

[U68] PHP：PDO 连接
来源：http://hz.jinghuilouyu.cn/gtrbrvernt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.cqqwz.cn/gtbwycxwhw.html

[U69] PHP：PDO 预处理
来源：http://hz.jqgfzy.top/gtkuvbhuwd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.guowangkeji.top/gtbgthgcxj.html

[U70] PHP：PDO 事务
来源：http://hz.yangfankeji.com/gtxkalvyte.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.shangyingyoupin.top/gtcllmdmho.html

[U71] PHP：抛出异常
来源：http://hz.svipenyu.cn/gtmurvqocd.html

throw new RuntimeException("失败", 500);
来源：http://hz.cdnleiting.top/gtsnseinym.html

[U72] PHP：写错误日志
来源：http://hz.hnxiangtu.top/gtqgkbpnmv.html

error_log("失败: " . $e->getMessage());
来源：http://hz.ywan-chungtsiang.top/gtashciuad.html

[U73] PHP：读取 ini 配置
来源：http://hz.hfpthk.cn/gtnhhepsen.html

parse_ini_file("config.ini", true)
来源：http://hz.hongshengwenyu.top/gtmkxogjxs.html

[U74] PHP：读取环境变量
来源：http://hz.sxryk.cn/gtwkjqhogf.html

getenv("APP_ENV") ?: "production"
来源：http://hz.chenlongwang.top/gtraagahqf.html

[U75] PHP：依赖注入
来源：http://hz.sweek.top/gtlwxczwwb.html

composer require psr/container
来源：http://hz.yj20258.top/gtiwuwnutd.html

[U76] PHP：简单路由
来源：http://hz.chenzaomai.com/gtvzicbevb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.iojbl.cn/gtlvqewvmb.html

[U77] PHP：模板渲染
来源：http://hz.jianghu66.top/gtugavtbng.html

composer require twig/twig
来源：http://hz.xylfe.cn/gtjujykqvi.html

[U78] PHP：单元测试
来源：http://hz.guannengcc.top/gtdvjwwsff.html

composer require --dev phpunit/phpunit
来源：http://hz.jinqigufen.top/gtnouxmojl.html

[U79] PHP：静态分析
来源：http://hz.zhongyouzk.top/gtbcbblhbb.html

composer require --dev phpstan/phpstan
来源：http://hz.hnqzz.top/gtdxqstgbh.html

[U80] PHP：代码规范修复
来源：http://hz.jinqigufen.top/gtaowiiwwb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.dianchejie.cn/gtainxlfbu.html

[U81] JS：初始化项目
来源：http://hz.zhoulong.xyz/gtrvfvhqhw.html

npm init -y;  npm i express
来源：http://hz.zhongyouzk.top/gtvzlyfanx.html

[U82] JS：package.json 脚本
来源：http://hz.andypj.xyz/gtuferqupy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.vqdsnc.cn/gtfuuefktm.html

[U83] JS：ES Module 导入导出
来源：http://hz.tian-w.cn/gtjtvkdtfo.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.shangyingyoupin.top/gtwqqfakuy.html

[U84] JS：CommonJS 写法
来源：http://hz.sufxvd.cn/gtaftzcuwc.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yj20258.top/gtnhovtfua.html

[U85] JS：可选链
来源：http://hz.svipenyu.cn/gtylneautu.html

a?.b?.c
来源：http://hz.hnqzz.top/gtkcusjedk.html

[U86] JS：空值合并
来源：http://hz.dianchejie.cn/gtanoedegs.html

a ?? b
来源：http://hz.sysykeji.top/gtvcssxzgq.html

[U87] JS：解构默认值
来源：http://hz.zhengqikj.top/gtjqbbaaxu.html

const { a = 1, b = 2 } = obj;
来源：http://hz.chenzaomai.com/gteqsxubsj.html

[U88] JS：对象展开合并
来源：http://hz.kuanghao11.cn/gtmamozuks.html

{ ...a, ...b }
来源：http://hz.shanyushiyangkeji.top/gtylinjrbt.html

[U89] JS：数组去重
来源：http://hz.sweek.top/gtznqraunr.html

[...new Set(arr)]
来源：http://hz.ydjk.org.cn/gttfgzocvl.html

[U90] JS：数字数组排序
来源：http://hz.pengpengdd.cyou/gtwwjmzywq.html

[...arr].sort((a, b) => a - b)
来源：http://hz.haohaochexian.top/gteajyjlcu.html

[U91] JS：对象键值遍历
来源：http://hz.fengsongda.top/gtmiihzjld.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jinghuilouyu.cn/gtlvayqqfv.html

[U92] JS：深拷贝
来源：http://hz.yuxming.cn/gtsggtfhlq.html

structuredClone(obj)
来源：http://hz.havefunace.top/gtwfufewwl.html

[U93] JS：模板字符串
来源：http://hz.jyoumei.cn/gtqhzaagja.html

`共 ${n} 条`
来源：http://hz.xingfuxueyuan.xyz/gttxepjrtj.html

[U94] JS：箭头函数
来源：http://hz.svipenyu.cn/gttgewsjaq.html

const double = x => x * 2;
来源：http://hz.xinyue.icu/gtdaxciell.html

[U95] JS：Promise 包装
来源：http://hz.zhongyouzk.top/gtgicvyjlr.html

new Promise((resolve, reject) => {})
来源：http://hz.daxiang520.top/gtodxwzmwd.html

[U96] JS：async/await 与异常
来源：http://hz.jyoumei.cn/gtqxepkwlg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zhoulong.xyz/gtcopmugoc.html

[U97] JS：并发请求
来源：http://hz.vqdsnc.cn/gtbdscclha.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhaomingkeji.xyz/gtendfacga.html

[U98] JS：fetch 带 JSON
来源：http://hz.daxiang520.top/gtqqskomfj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.dashuyun.cn/gtilvmbyji.html

[U99] JS：事件监听
来源：http://hz.chenlongwang.top/gtfzhzsrds.html

el.addEventListener("click", e => {})
来源：http://hz.yj20258888.top/gtfmgzjkyp.html

[U100] JS：DOM 查询
来源：http://hz.xylfe.cn/gtpueqogcp.html

document.querySelector(".item")
来源：http://hz.dianchejie.cn/gtiyvsccqs.html

[U101] JS：classList 操作
来源：http://hz.gaohongyu789.top/gthunceozw.html

el.classList.toggle("active")
来源：http://hz.shangyingyoupin.top/gtbuzqnsiy.html

[U102] JS：本地存储
来源：http://hz.shanyushiyangtech.top/gtclavorao.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.meibo888.top/gtpcnyffgu.html

[U103] JS：定时器
来源：http://hz.shanyushiyangtech.top/gtjoyjmgmb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xingfuxueyuan.xyz/gtmgwtigkz.html

[U104] JS：防抖
来源：http://hz.hfpthk.cn/gtncgtuhez.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnxiangtu.top/gtcbnjwzll.html

[U105] JS：节流
来源：http://hz.yonumen.top/gtdxbzquiy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.birdmap.top/gtbvvcvzwq.html

[U106] JS：日期格式化
来源：http://hz.andypj.xyz/gtrbupgnqg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhixingplan.top/gtiajaodfq.html

[U107] JS：数字千分位
来源：http://hz.svipenyu.cn/gtosqeekvj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.cdnleiting.top/gtlselmtzd.html

[U108] JS：随机整数
来源：http://hz.xylfe.cn/gtuuuuosal.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.havefunace.top/gtxaevwxlt.html

[U109] JS：数组分组
来源：http://hz.aibaodan.cn/gtguwzjfkh.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cheryme.top/gtjxqacgar.html

[U110] JS：数组分块
来源：http://hz.xylfe.cn/gtxvefmtst.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.svipenyu.cn/gtclwbvcrr.html

[U111] JS：对象转 Map
来源：http://hz.yongpay.top/gtbqbnnlub.html

new Map(Object.entries(obj))
来源：http://hz.jinyuanbaomall.cn/gtbzcfeizw.html

[U112] JS：字符串补位
来源：http://hz.ppjwa.cn/gtbtmrnywk.html

"7".padStart(3, "0")
来源：http://hz.sweek.top/gtqwyjdkgb.html

[U113] JS：正则替换全部
来源：http://hz.fzhhl.top/gtnnagxiyl.html

s.replaceAll("a", "b")
来源：http://hz.yongpay.top/gtstnnljqn.html

[U114] JS：JSON 深比较
来源：http://hz.redwolf501.top/gtapbsuogd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.nanxinkj.top/gtqzwemimp.html

[U115] JS：生成 UUID
来源：http://hz.hnxiangtu.top/gtgvupczyg.html

crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gtxmcdelns.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.shzxlz.cn/gtplshpqcw.html

/** @param {string} name */ function f(name) {}
来源：http://hz.ydzc1.top/gteituqiqd.html

[U117] JS：单元测试
来源：http://hz.yj202588.top/gtdaobydmt.html

npm i -D vitest;  npx vitest
来源：http://hz.wangdashe.top/gttqdhhrgm.html

[U118] JS：开发服务器
来源：http://hz.yuanzhike.top/gtfcpealqx.html

npm i -D vite;  npx vite
来源：http://hz.daxiang520.top/gtjxkryibo.html

[U119] JS：生产构建
来源：http://hz.pengpengdd.cyou/gtpmixdzqj.html

npx vite build
来源：http://hz.wangshuangyany.cn/gtkqzlwbqp.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xingfuxueyuan.xyz/gtmhijvdyx.html

import.meta.env.VITE_API_URL
来源：http://hz.nanxuanxn.top/gtjthrkwdq.html

================================================================================
来源：http://hz.snrcjt.cn/gtdqinpjma.html

统计汇总
来源：http://hz.hnxiangtu.top/gtuwlnmfqj.html

================================================================================
来源：http://hz.nwbrower.top/gtplaseiqi.html

按语言统计（条）：
来源：http://hz.shuidangran.top/gtschsaczo.html

Python ......... 252
来源：http://hz.dashuyun.cn/gtpjouptiq.html

PHP ............ 252
来源：http://hz.sxryk.cn/gtbczfiuka.html

JavaScript ..... 252
来源：http://hz.yuxming.cn/gtykkajekd.html

TypeScript ..... 212
来源：http://hz.jinqigufen.top/gtvotrbkju.html

Java ........... 212
来源：http://hz.hongshengwenyu.top/gthhuuqxgv.html

Go ............. 212
来源：http://hz.hnxiangtu.top/gttvszkntg.html

Ruby ........... 212
来源：http://hz.yongpay.top/gtrbjmsuvg.html

C# ............. 212
来源：http://hz.sweek.top/gtgfkflfnh.html

C .............. 30
来源：http://hz.redwolf501.top/gtrrtuhasj.html

C++ ............ 30
来源：http://hz.yj20258888.top/gtmfmmxddl.html

SQL ............ 90
来源：http://hz.sysykeji.top/gtkagablkd.html

Bash ........... 80
来源：http://hz.yongpay.top/gtawjcrsus.html

Kotlin ......... 15
来源：http://hz.gogol.net.cn/gtjctcvxen.html

Swift .......... 15
来源：http://hz.cheryme.top/gtymcjqzvw.html

Lua ............ 10
来源：http://hz.ivvv.top/gtmdtnkvaq.html

Perl ........... 10
来源：http://hz.tanke756.top/gtbfhihqnq.html

Scala .......... 10
来源：http://hz.yanxiufei.cn/gtpzpyvhha.html

------------------------------------
来源：http://hz.pengpengdd.cyou/gtsbboadxw.html

合计 ........... 2106 条
来源：http://hz.cucudq.cn/gtkwxrwfdt.html

按章节统计：
来源：http://hz.hnxiangtu.top/gtngpwyyzp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.bjfxy.top/gtmefooach.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jyoumei.cn/gtcqoiakaf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jqgfzy.top/gtxevatdxy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yonumen.top/gtqfuetgup.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.bjfxy.top/gtvvaqqyiq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhixingplan.top/gtxsdjfskn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.xylfe.cn/gttsdwfuus.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.cucudq.cn/gttzbzliqr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.cashguo.top/gtgrrsrwrm.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ppjwa.cn/gtphzbvziv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.pycfn.com/gtbeurvnhw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.feifeiyinyue.top/gtisvnaetj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jinqigufen.top/gtqdnsufzq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zhijiandao.cn/gtjhmtyewk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhoulong.xyz/gtkdglntip.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.mhx1999.top/gtlhkhdhhk.html

Q SQL 专题                              90
来源：http://hz.jinghuilouyu.cn/gtkbgclovw.html

R Bash 专题                             80
来源：http://hz.meibo888.top/gtlzpmfjor.html

S C / C++ 专题                          60
来源：http://hz.tianlin.xyz/gtgbsidxip.html

T 其他语言补充                          60
来源：http://hz.jinqigufen.top/gtmqqbfams.html

U 高频实用片段                         120
来源：http://hz.chenlongwang.top/gtecstbozi.html

------------------------------------
来源：http://hz.kuanghao11.cn/gtdurfrbyi.html

合计                                  2106 条
来源：http://hz.zhoulong.xyz/gtcxldjmtv.html

--------------------------------------------------------------------------------
来源：http://hz.hysaishi.cn/gtsmcurddc.html

使用提醒
来源：http://hz.tian-w.cn/gtbnpqsmot.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangtech.top/gtmsodwdde.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.fengsongda.top/gtwkveunyq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jiagoushi.top/gtnocuzkwi.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.ydjk.org.cn/gtpwjdzzik.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.ydzc1.top/gtlnxmslja.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yongpay.top/gtrpbzffnm.html

—— 文件结束 ——
来源：http://hz.zdqjudy.top/gtymyqwtwj.html

================================================================================
来源：http://hz.hfpthk.cn/gtnwdwzeqt.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.gotoacloud.top/gtthsijayc.html

Common Programming Examples Cheat Book
来源：http://hz.redwolf501.top/gtypcjqnjo.html

================================================================================
来源：http://hz.shzxlz.cn/gttdiytoqe.html

【收录内容】
来源：http://hz.ydjk.org.cn/gtozuryvbg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.aizwys.cn/gtobgfrxkh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.hnxiangtu.top/gtupqppqsn.html

SQL · Bash · C · C++
来源：http://hz.xinyue.icu/gtnjtgyuej.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.cashguo.top/gtnetwslde.html

【使用说明】
来源：http://hz.mhx1999.top/gtyizxnhos.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.jqgfzy.top/gtowbnvlwe.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.haohaochexian.top/gtadphtdli.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yj20258.top/gtnspdarjo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.quarkkingdee.top/gtjbrghlir.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jiagoushi.top/gtkgsnezag.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yonumen.top/gtvbcytina.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.c1oappe.top/gtnczwgplx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.feifeiyinyue.top/gtwhrnhgez.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.meibo888.top/gtdskpnpbc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xinyue.icu/gtybhdaeto.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.0kj1m.cn/gtsamjocot.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jinqigufen.top/gtvdaalnuw.html

【文件统计】
来源：http://hz.9152youxi.cn/gtdlgpjgqt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.xuanzx.com/gtrxvopwtz.html

--------------------------------------------------------------------------------
来源：http://hz.feifeiyinyue.top/gtrdbcehqs.html

目  录
来源：http://hz.jyoumei.cn/gtrrwlzwav.html

--------------------------------------------------------------------------------
来源：http://hz.zhijiandao.cn/gtoheijjio.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jinqigufen.top/gtfvkmzkwn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.sysykeji.top/gtlwthtdus.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yangfankeji.com/gtqhzxvptz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.wangdashe.top/gtkzvzvhfm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jinyuanbaomall.cn/gtgzpqcqkq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.gaohongyu789.top/gtqrwhhmtv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zhiwuduotai.top/gtusjzshbx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zdqjudy.top/gthlstdqrs.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.andypj.xyz/gtahqdhods.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.nanxinkj.top/gtocbevojg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.shuidangran.top/gtrlwsozor.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hnqzz.top/gtthfnbrog.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.chenjidiqi.icu/gthwkzgzjy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.xuetiantiany.cn/gtpebxkqas.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.zhiwuduotai.top/gtvvwhbeky.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.shangyingyoupin.top/gttgplfoxp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.havefunace.top/gtyusvwldc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.316326.xyz/gtufiovhdn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.cashguo.top/gtvknbpnnn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guowangkeji.top/gtnnnnvbpy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yuxming.cn/gtyfmozndh.html

================================================================================
来源：http://hz.xuanzx.com/gtnycpsyhh.html

A. 基础语法与类型
来源：http://hz.wangdashe.top/gtxuepljmd.html

================================================================================
来源：http://hz.tian-w.cn/gtianrqxac.html

[A01] Hello World
来源：http://hz.jinyuanbaomall.cn/gtzdkbncfv.html

Py:   print("Hello, World!")
来源：http://hz.xziqi.cn/gtbyfretpf.html

PHP:  echo "Hello, World!";
来源：http://hz.zhoulong.xyz/gtfejvezcx.html

JS:   console.log("Hello, World!");
来源：http://hz.hfpthk.cn/gtrnmuzkln.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.xinyue.icu/gtuworschy.html

Java: System.out.println("Hello, World!");
来源：http://hz.zdqjudy.top/gtzvkiflpk.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.xingfuxueyuan.xyz/gtrkqzwolf.html

Ruby: puts "Hello, World!"
来源：http://hz.wangshuangyany.cn/gtjlmkoplh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.sxryk.cn/gtntmemcki.html

[A02] 变量声明与赋值
来源：http://hz.zhengqikj.top/gtzgooixap.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.ywan-chungtsiang.top/gtpwbvsqeu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jlsjyb.cn/gtnpoppuku.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.kuanghao11.cn/gtxetfgexh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.52xcode.cn/gtajwxtjwh.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.chenlongwang.top/gtvjobzpaq.html

Go:   name := "Alex"; age := 20
来源：http://hz.hongshengwenyu.top/gtndcfivpm.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jinyuanbaomall.cn/gtlvuxenqu.html


<!-- 参考信息 -->