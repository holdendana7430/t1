代发 wailian999

[U25] Py：CSV 按字典读
来源：http://hz.yuxming.cn/gttaskdgoj.html

csv.DictReader(f)
来源：http://hz.chenjidiqi.icu/gtccibhzee.html

[U26] Py：并发下载
来源：http://hz.chenlongwang.top/gtbaiuwwur.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hysaishi.cn/gtghcxsgjt.html

[U27] Py：异步 HTTP
来源：http://hz.xingfuxueyuan.xyz/gtljlgbwnq.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.daria6918.cn/gtdlvbtjfi.html

[U28] Py：类型别名
来源：http://hz.dianchejie.cn/gtflcsvoor.html

UserId = int
来源：http://hz.tanke756.top/gthnjlwcxt.html

[U29] Py：属性校验
来源：http://hz.tanke756.top/gtihaqivqo.html

@property 与 @x.setter 配合
来源：http://hz.andypj.xyz/gthkepywnn.html

[U30] Py：数据类
来源：http://hz.cucudq.cn/gtszbzoupp.html

@dataclass(slots=True)
来源：http://hz.ydzc1.top/gtuvtqgrde.html

[U31] Py：单测
来源：http://hz.nwbrower.top/gtjncdvnmm.html

python -m pytest -q
来源：http://hz.9152youxi.cn/gtxzlwbhwg.html

[U32] Py：代码格式化
来源：http://hz.hnxiangtu.top/gtlvgskswp.html

ruff format . && ruff check --fix .
来源：http://hz.52xcode.cn/gtldbvobqn.html

[U33] Py：打包发布
来源：http://hz.andypj.xyz/gtdoikzpnx.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.gaohongyu789.top/gtoqabboel.html

[U34] Py：判断编码
来源：http://hz.fengsongda.top/gtcpwbtixz.html

chardet.detect(raw)
来源：http://hz.sweek.top/gtsyqjwhhm.html

[U35] Py：发送邮件
来源：http://hz.zhijiandao.cn/gtwhazdrfj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.gogol.net.cn/gtpbijybnl.html

[U36] Py：定时任务
来源：http://hz.daria6918.cn/gtwdjxhait.html

schedule.every(10).minutes.do(job)
来源：http://hz.hammf.cn/gtvkcevwzo.html

[U37] Py：读写 Excel
来源：http://hz.daxiang520.top/gtbkeepawr.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.shanyushiyangkeji.top/gtfhfpmdlw.html

[U38] Py：获取脚本所在目录
来源：http://hz.svipenyu.cn/gtgttdkgcl.html

Path(__file__).resolve().parent
来源：http://hz.redwolf501.top/gtgphnqcmt.html

[U39] Py：判断是否在交互环境
来源：http://hz.xingfuxueyuan.xyz/gtkvxairpe.html

sys.stdout.isatty()
来源：http://hz.316326.xyz/gtlvjukbkx.html

[U40] Py：打印到标准错误
来源：http://hz.shangyingyoupin.top/gtkcytjgxd.html

print("err", file=sys.stderr)
来源：http://hz.yvedp.cn/gtbxnaftla.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.0kj1m.cn/gttorzvttf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ehwqpu.com/gthkjuqgvt.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.pengpengdd.cyou/gtxpdkvmwe.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.meibo888.top/gtobjnmhtx.html

[U43] PHP：声明命名空间
来源：http://hz.316326.xyz/gtygnreavd.html

namespace App\Http;
来源：http://hz.yj202588.top/gtmnpltclq.html

[U44] PHP：开启严格类型
来源：http://hz.52xcode.cn/gturttnylr.html

declare(strict_types=1);
来源：http://hz.daxiang520.top/gtuznnogln.html

[U45] PHP：类型声明与返回类型
来源：http://hz.meibo888.top/gtxeuvcehz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sxryk.cn/gtxlerypsi.html

[U46] PHP：可空类型
来源：http://hz.dashuyun.cn/gtabplriny.html

?string $name = null
来源：http://hz.xingfuxueyuan.xyz/gtvnusjtld.html

[U47] PHP：联合类型
来源：http://hz.52xcode.cn/gtmfywynba.html

int|string $id
来源：http://hz.yj20258888.top/gtbgjeviyf.html

[U48] PHP：纯枚举
来源：http://hz.andypj.xyz/gthixomlps.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.sufxvd.cn/gtgvgqpezr.html

[U49] PHP：只读属性
来源：http://hz.gzhubu.top/gtlfveijej.html

public readonly string $name
来源：http://hz.yueranfly.top/gtegmtqzqf.html

[U50] PHP：构造器属性提升
来源：http://hz.haohaochexian.top/gtpjurewdx.html

public function __construct(private int $id) {}
来源：http://hz.gotoacloud.top/gttfkmaehu.html

[U51] PHP：数组解构
来源：http://hz.jyoumei.cn/gtbpxncfhg.html

[$a, $b] = $arr;
来源：http://hz.tianlin.xyz/gtiwkkybsk.html

[U52] PHP：箭头函数
来源：http://hz.jqgufenzy.top/gtidjkxerr.html

$double = fn($x) => $x * 2;
来源：http://hz.hfpthk.cn/gtojmqxfra.html

[U53] PHP：空合并运算符
来源：http://hz.yvedp.cn/gtmugmxxvd.html

$v = $a ?? $b ?? "default";
来源：http://hz.yonumen.top/gtitbsproz.html

[U54] PHP：空安全调用
来源：http://hz.yj202588.top/gtulpqayne.html

$obj?->method()
来源：http://hz.gogol.net.cn/gtmmputwfs.html

[U55] PHP：match 表达式
来源：http://hz.daria6918.cn/gtbvzzyafl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.hfpthk.cn/gtzdtxkrke.html

[U56] PHP：命名参数
来源：http://hz.jlsjyb.cn/gtyofgovbz.html

f(a: 1, b: 2)
来源：http://hz.hnqzz.top/gthiocklet.html

[U57] PHP：字符串插值
来源：http://hz.daxiang520.top/gtgamxjiut.html

"值: {$a}"
来源：http://hz.jinqigufen.top/gtkgfowrfr.html

[U58] PHP：数组三件套
来源：http://hz.zycfv.cn/gtbxnerbus.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.xylfe.cn/gtmtcynkee.html

[U59] PHP：自定义排序
来源：http://hz.zhixingplan.top/gtkhwwkpop.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nanxuanxn.top/gtjooyrcdi.html

[U60] PHP：JSON 编解码
来源：http://hz.sysykeji.top/gtzojsethz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yj20258.top/gtrkbgcpxu.html

[U61] PHP：正则
来源：http://hz.yanxiufei.cn/gtkpoemcar.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jyoumei.cn/gtsqxvnpes.html

[U62] PHP：日期对象
来源：http://hz.bjfxy.top/gtdlozvjxz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.nanxuanxn.top/gtrlnsphnt.html

[U63] PHP：文件读写
来源：http://hz.gaohongyu789.top/gtlvpaayre.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.vqdsnc.cn/gtzeegtgda.html

[U64] PHP：目录遍历
来源：http://hz.ivvv.top/gtoyezmnql.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.mhx1999.top/gtfqrjkmex.html

[U65] PHP：会话
来源：http://hz.zhiwuduotai.top/gtjnmlvmbw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zhixingplan.top/gtdvesojav.html

[U66] PHP：设置 Cookie
来源：http://hz.aibaodan.cn/gtamfpljam.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.snrcjt.cn/gtgfkwdrsk.html

[U67] PHP：处理文件上传
来源：http://hz.gaohongyu789.top/gtojrxxkrb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yongpay.top/gtmcllwrmo.html

[U68] PHP：PDO 连接
来源：http://hz.xinyue.icu/gtuqmstclk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.fzhhl.top/gtxplnxkjy.html

[U69] PHP：PDO 预处理
来源：http://hz.hnxiangtu.top/gtawcrfvlh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jyoumei.cn/gtmjaewoha.html

[U70] PHP：PDO 事务
来源：http://hz.ehwqpu.com/gtsevhpadh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.shanyushiyangtech.top/gtjzanypqu.html

[U71] PHP：抛出异常
来源：http://hz.pengpengdd.cyou/gtliokioxt.html

throw new RuntimeException("失败", 500);
来源：http://hz.zhixingplan.top/gtfensffkq.html

[U72] PHP：写错误日志
来源：http://hz.yj20258888.top/gtrjbigmti.html

error_log("失败: " . $e->getMessage());
来源：http://hz.guannengcc.top/gtnqkdytje.html

[U73] PHP：读取 ini 配置
来源：http://hz.dashuyun.cn/gtctnrxrge.html

parse_ini_file("config.ini", true)
来源：http://hz.aizwys.cn/gtagfxhahd.html

[U74] PHP：读取环境变量
来源：http://hz.daxiang520.top/gttamnrkwt.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yangfankeji.com/gtffxvsjde.html

[U75] PHP：依赖注入
来源：http://hz.jqgufenzy.top/gtwhplbvqr.html

composer require psr/container
来源：http://hz.aibaodan.cn/gtoxieajgl.html

[U76] PHP：简单路由
来源：http://hz.jinqigufen.top/gtkhqgjual.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.guowangkeji.top/gtashspvbd.html

[U77] PHP：模板渲染
来源：http://hz.meibo888.top/gtohfxohtm.html

composer require twig/twig
来源：http://hz.nanxuanxn.top/gtnqldqrxl.html

[U78] PHP：单元测试
来源：http://hz.jinghuilouyu.cn/gtebkkolvm.html

composer require --dev phpunit/phpunit
来源：http://hz.daria6918.cn/gtpzhrjnnp.html

[U79] PHP：静态分析
来源：http://hz.aizwys.cn/gttrmznqjl.html

composer require --dev phpstan/phpstan
来源：http://hz.cheryme.top/gtojdfiylj.html

[U80] PHP：代码规范修复
来源：http://hz.chenlongwang.top/gtrcskhsct.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.cdnleiting.top/gtluvgzdul.html

[U81] JS：初始化项目
来源：http://hz.dianchejie.cn/gtufvbqvbo.html

npm init -y;  npm i express
来源：http://hz.tanke756.top/gtuzuspssm.html

[U82] JS：package.json 脚本
来源：http://hz.havefunace.top/gtewkslsqq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.pengpengdd.cyou/gtdulscjky.html

[U83] JS：ES Module 导入导出
来源：http://hz.zdqjudy.top/gtomobeeij.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.sxryk.cn/gtymqtfxia.html

[U84] JS：CommonJS 写法
来源：http://hz.chenzaomai.com/gtelgmqhmd.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jinyuanbaomall.cn/gtnhqygbfa.html

[U85] JS：可选链
来源：http://hz.sufxvd.cn/gtwxaprcjc.html

a?.b?.c
来源：http://hz.dashuyun.cn/gtnwmbyreo.html

[U86] JS：空值合并
来源：http://hz.shuidangran.top/gtuztwgadb.html

a ?? b
来源：http://hz.zhaomingkeji.xyz/gtyyxgrfik.html

[U87] JS：解构默认值
来源：http://hz.cdnleiting.top/gtkwfiguvy.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhixingplan.top/gtpfacfdxz.html

[U88] JS：对象展开合并
来源：http://hz.yj202588.top/gthvkuzfuh.html

{ ...a, ...b }
来源：http://hz.guannengcc.top/gtzooupatq.html

[U89] JS：数组去重
来源：http://hz.zhongyouzk.top/gttuvaoveg.html

[...new Set(arr)]
来源：http://hz.svipenyu.cn/gtbtdjtzpi.html

[U90] JS：数字数组排序
来源：http://hz.cqqwz.cn/gtfwnwokbl.html

[...arr].sort((a, b) => a - b)
来源：http://hz.c1oappe.top/gtxnlxbvym.html

[U91] JS：对象键值遍历
来源：http://hz.sysykeji.top/gtnpeqvuxg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.nanxuanxn.top/gtsvdfsvdx.html

[U92] JS：深拷贝
来源：http://hz.52xcode.cn/gtgrbnofsz.html

structuredClone(obj)
来源：http://hz.ywan-chungtsiang.top/gtzvkbbybm.html

[U93] JS：模板字符串
来源：http://hz.gotoacloud.top/gtrgrovylu.html

`共 ${n} 条`
来源：http://hz.snrcjt.cn/gtbtaziiig.html

[U94] JS：箭头函数
来源：http://hz.jqgfzy.top/gtvdqazbjh.html

const double = x => x * 2;
来源：http://hz.gaohongyu789.top/gtsqhgybxo.html

[U95] JS：Promise 包装
来源：http://hz.9152youxi.cn/gtbguvakcf.html

new Promise((resolve, reject) => {})
来源：http://hz.xylfe.cn/gtxtblizxo.html

[U96] JS：async/await 与异常
来源：http://hz.jianghu66.top/gttbqvkmfl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jiagoushi.top/gtkjdhpffs.html

[U97] JS：并发请求
来源：http://hz.ybcxt.top/gtzkckbfqg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sysykeji.top/gtkyayiltj.html

[U98] JS：fetch 带 JSON
来源：http://hz.xuetiantiany.cn/gtpybaalmn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.svipenyu.cn/gtomtraotd.html

[U99] JS：事件监听
来源：http://hz.ywan-chungtsiang.top/gtiylyutad.html

el.addEventListener("click", e => {})
来源：http://hz.zhijiandao.cn/gtsardzzvb.html

[U100] JS：DOM 查询
来源：http://hz.mhx1999.top/gtdtsnbheq.html

document.querySelector(".item")
来源：http://hz.aibaodan.cn/gtmwyiseya.html

[U101] JS：classList 操作
来源：http://hz.shuidangran.top/gtisavmmtl.html

el.classList.toggle("active")
来源：http://hz.fzhhl.top/gtniaclaat.html

[U102] JS：本地存储
来源：http://hz.chenjidiqi.icu/gtulhngjwp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yuanzhike.top/gtikxprcsl.html

[U103] JS：定时器
来源：http://hz.mhx1999.top/gtvbpnwtcn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.havefunace.top/gtpiscpdtz.html

[U104] JS：防抖
来源：http://hz.zhengqikj.top/gtjshuslha.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ywan-chungtsiang.top/gtxhfcduje.html

[U105] JS：节流
来源：http://hz.zhixingplan.top/gtgazlrdgy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.birdmap.top/gtdmcqbjfx.html

[U106] JS：日期格式化
来源：http://hz.birdmap.top/gtumgnehth.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yuxming.cn/gtxunbeqkx.html

[U107] JS：数字千分位
来源：http://hz.yonumen.top/gtigbkexbo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yvedp.cn/gtkgdflzbb.html

[U108] JS：随机整数
来源：http://hz.tianlin.xyz/gtpafcqjne.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yangfankeji.com/gtajqogxhr.html

[U109] JS：数组分组
来源：http://hz.fzhhl.top/gtpcszbpfb.html

Object.groupBy(arr, x => x.type)
来源：http://hz.dashuyun.cn/gtxtljxtof.html

[U110] JS：数组分块
来源：http://hz.c1oappe.top/gtjhywpqar.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.gotoacloud.top/gtesvgzvxa.html

[U111] JS：对象转 Map
来源：http://hz.jiagoushi.top/gtqhbwwqta.html

new Map(Object.entries(obj))
来源：http://hz.iojbl.cn/gtanoqdkfh.html

[U112] JS：字符串补位
来源：http://hz.yj20258888.top/gtygvnezrv.html

"7".padStart(3, "0")
来源：http://hz.yuxming.cn/gtujgokjmw.html

[U113] JS：正则替换全部
来源：http://hz.andypj.xyz/gtblxajxip.html

s.replaceAll("a", "b")
来源：http://hz.zhixingplan.top/gtnoahkdmm.html

[U114] JS：JSON 深比较
来源：http://hz.zhixingplan.top/gtnigkkhdr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xziqi.cn/gtuhzerrbt.html

[U115] JS：生成 UUID
来源：http://hz.havefunace.top/gtnerkmtef.html

crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtqcufnujd.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.52xcode.cn/gtjtgdndmu.html

/** @param {string} name */ function f(name) {}
来源：http://hz.hnqzz.top/gtrqytmyww.html

[U117] JS：单元测试
来源：http://hz.mhx1999.top/gtpiujfscy.html

npm i -D vitest;  npx vitest
来源：http://hz.ybcxt.top/gtpryqdngl.html

[U118] JS：开发服务器
来源：http://hz.gotoacloud.top/gtphivgsox.html

npm i -D vite;  npx vite
来源：http://hz.jinqigufen.top/gtggfowgcf.html

[U119] JS：生产构建
来源：http://hz.sysykeji.top/gtzhsxqwhv.html

npx vite build
来源：http://hz.chenjidiqi.icu/gtdjchgbid.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jlsjyb.cn/gtugwgjijc.html

import.meta.env.VITE_API_URL
来源：http://hz.jinqigfzy.top/gtyamvmygx.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtljlitqfa.html

统计汇总
来源：http://hz.jinghuilouyu.cn/gtsjdrfyeq.html

================================================================================
来源：http://hz.iojbl.cn/gtbpwltmqw.html

按语言统计（条）：
来源：http://hz.hammf.cn/gtwzsvzdar.html

Python ......... 252
来源：http://hz.tanke756.top/gtjsvnxfox.html

PHP ............ 252
来源：http://hz.jianghu66.top/gtqtwiunwx.html

JavaScript ..... 252
来源：http://hz.zhoulong.xyz/gtqrmtpvtf.html

TypeScript ..... 212
来源：http://hz.daxiang520.top/gtsyhbatvi.html

Java ........... 212
来源：http://hz.hnxiangtu.top/gtvciuhkfk.html

Go ............. 212
来源：http://hz.nanxuanxn.top/gtbvfsglam.html

Ruby ........... 212
来源：http://hz.nwbrower.top/gtkthqugss.html

C# ............. 212
来源：http://hz.aibaodan.cn/gtnegtxcst.html

C .............. 30
来源：http://hz.guowangkeji.top/gtwfsxmxlx.html

C++ ............ 30
来源：http://hz.hnxiangtu.top/gtyjmdxyxj.html

SQL ............ 90
来源：http://hz.jiagoushi.top/gtmpgglrpy.html

Bash ........... 80
来源：http://hz.zhijiandao.cn/gtzezujhni.html

Kotlin ......... 15
来源：http://hz.c1oappe.top/gtxyrmfzxd.html

Swift .......... 15
来源：http://hz.mhx1999.top/gtdbjtzxcf.html

Lua ............ 10
来源：http://hz.yj20258.top/gtvokqfzxn.html

Perl ........... 10
来源：http://hz.9152youxi.cn/gtcfaxbimk.html

Scala .......... 10
来源：http://hz.ivvv.top/gtccrtewne.html

------------------------------------
来源：http://hz.fengsongda.top/gtcawmtsgg.html

合计 ........... 2106 条
来源：http://hz.svipenyu.cn/gtqerbvnrk.html

按章节统计：
来源：http://hz.svipenyu.cn/gtsmcwsrxt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yvedp.cn/gtllvzthuz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.sweek.top/gtfvfengxq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.c1oappe.top/gtmtemeesh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.pengpengdd.cyou/gtnktalbmv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.shanyushiyangtech.top/gtjahfkrzp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yongpay.top/gtttjlravd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.mhx1999.top/gtseevilcp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yangfankeji.com/gtxvjfwhvt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jqgfzy.top/gtdpximgjd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.wangshuangyany.cn/gtlrnslcgr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.gogol.net.cn/gtfaagwgyu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.chenlongwang.top/gtiaezefvf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.sufxvd.cn/gtzfmyltof.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jyoumei.cn/gtwfrnyras.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.tanke756.top/gthljwtijy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangkeji.top/gtsilkopbq.html

Q SQL 专题                              90
来源：http://hz.redwolf501.top/gtaagvuact.html

R Bash 专题                             80
来源：http://hz.yj20258.top/gtwmllfzpn.html

S C / C++ 专题                          60
来源：http://hz.nanxuanxn.top/gtjociasiu.html

T 其他语言补充                          60
来源：http://hz.hammf.cn/gtdafqmktm.html

U 高频实用片段                         120
来源：http://hz.wangshuangyany.cn/gthsjuxweu.html

------------------------------------
来源：http://hz.yuanzhike.top/gtjfmlnjwh.html

合计                                  2106 条
来源：http://hz.cashguo.top/gtrkcmjgtv.html

--------------------------------------------------------------------------------
来源：http://hz.tanke756.top/gtwjvkbjjl.html

使用提醒
来源：http://hz.yanxiufei.cn/gtzgkhnspg.html

--------------------------------------------------------------------------------
来源：http://hz.xingfuxueyuan.xyz/gtdcpwxjgx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.shanyushiyangkeji.top/gtyjxfwcpr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jinqigfzy.top/gtpoykqfyw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.dashuyun.cn/gtgghycukk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.cqqwz.cn/gtfjazxvzc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.shzxlz.cn/gtcltqomrb.html

—— 文件结束 ——
来源：http://hz.havefunace.top/gtwknmnrxr.html

================================================================================
来源：http://hz.fengsongda.top/gtqfwmsptp.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jiagoushi.top/gtxcxfizjl.html

Common Programming Examples Cheat Book
来源：http://hz.yvedp.cn/gtiatdgpjy.html

================================================================================
来源：http://hz.jinqigfzy.top/gtkjbzulnx.html

【收录内容】
来源：http://hz.zhengqikj.top/gttuxwzjuj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.nwbrower.top/gtunjnjwmo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.tian-w.cn/gtbczypfyi.html

SQL · Bash · C · C++
来源：http://hz.daria6918.cn/gtkucosjkw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zycfv.cn/gtttuevepv.html

【使用说明】
来源：http://hz.yonumen.top/gtfyrvutqq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhaomingkeji.xyz/gtnqrhyibp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.cdnleiting.top/gtfxxkxryb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zhoulong.xyz/gtfvymtyal.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.gogol.net.cn/gttdycstvw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yonumen.top/gththovpfy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.hnqzz.top/gtvilxekyi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hammf.cn/gtxmncephr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.havefunace.top/gtphdjdryd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.kuanghao11.cn/gthlfikegr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.chenlongwang.top/gtajeehzzz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.ydzc1.top/gtlpoyypnv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yuxming.cn/gtefkschbz.html

【文件统计】
来源：http://hz.jinyuanbaomall.cn/gtxrgyxouq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.shuidangran.top/gtisecxxei.html

--------------------------------------------------------------------------------
来源：http://hz.meibo888.top/gtjznmowof.html

目  录
来源：http://hz.jinqigfzy.top/gtbulvusbr.html

--------------------------------------------------------------------------------
来源：http://hz.jlsjyb.cn/gtkqruomgc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.yueranfly.top/gtrfpboowa.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.xingfuxueyuan.xyz/gtpqfmrbdt.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yj202588.top/gtftnfvkis.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.ppjwa.cn/gtdqdlibzp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.ehwqpu.com/gtpdvkncxo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.haohaochexian.top/gtaqvzdeja.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.ydjk.org.cn/gtgpkyipor.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.kuanghao11.cn/gtweoowwlv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.tianlin.xyz/gtmbrwomzm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jiagoushi.top/gtivruocwg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.gotoacloud.top/gtclipdxdh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.dianchejie.cn/gtebtbpbzx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.feifeiyinyue.top/gtbljxgnvm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.jlsjyb.cn/gtudanpirl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.daxiang520.top/gtvgakroos.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.jlsjyb.cn/gtpduymeux.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhixingplan.top/gtdblhlneg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.yuanzhike.top/gtkhikrzko.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.c1oappe.top/gtllvcgpxh.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.kuanghao11.cn/gtpvjmjbut.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yuanzhike.top/gtnnhzrrgp.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtgdihywnt.html

A. 基础语法与类型
来源：http://hz.yvedp.cn/gtduxwjyxw.html

================================================================================
来源：http://hz.jinqigfzy.top/gtuihzhhbd.html

[A01] Hello World
来源：http://hz.tian-w.cn/gtuacapbdn.html


<!-- 参考信息 -->