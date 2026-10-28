代发 wailian999

[U17] Py：初始化日志
来源：http://hz.zdqjudy.top/gtgwafpkyh.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.feifeiyinyue.top/gtcjnbfptz.html

[U18] Py：预编译正则
来源：http://hz.xziqi.cn/gtbcisupxz.html

pat = re.compile(r"\d+")
来源：http://hz.iojbl.cn/gtoxuymtgf.html

[U19] Py：正则替换带回调
来源：http://hz.nwbrower.top/gtlpgicsem.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xylfe.cn/gtpsnhwpng.html

[U20] Py：缓存函数结果
来源：http://hz.guannengcc.top/gtdvbsofxf.html

@functools.lru_cache(maxsize=None)
来源：http://hz.ydjk.org.cn/gtkxhiubuu.html

[U21] Py：自定义上下文管理器
来源：http://hz.52xcode.cn/gtofevbnew.html

@contextlib.contextmanager
来源：http://hz.daria6918.cn/gtspuyxvzq.html

[U22] Py：矩阵转置
来源：http://hz.smart0.xyz/gtyvfakojo.html

list(zip(*m))
来源：http://hz.sxryk.cn/gtqlgbppvj.html

[U23] Py：分块读取大文件
来源：http://hz.xingfuxueyuan.xyz/gtsgztnjvi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jqgufenzy.top/gtnnhqdgez.html

[U24] Py：路径操作
来源：http://hz.jinqigufen.top/gtezuytzde.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.shangyingyoupin.top/gtrnutjehl.html

[U25] Py：CSV 按字典读
来源：http://hz.cdnleiting.top/gtyxtsrerj.html

csv.DictReader(f)
来源：http://hz.xuetiantiany.cn/gtakmjfeyy.html

[U26] Py：并发下载
来源：http://hz.dianchejie.cn/gtgesokvoe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yonumen.top/gtdifcmmjg.html

[U27] Py：异步 HTTP
来源：http://hz.yongpay.top/gtqzeazgnn.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.guannengcc.top/gtslqnovra.html

[U28] Py：类型别名
来源：http://hz.chenjidiqi.icu/gtsvwwqyhq.html

UserId = int
来源：http://hz.jinghuilouyu.cn/gthctxmjxs.html

[U29] Py：属性校验
来源：http://hz.fzhhl.top/gtzcvwwknu.html

@property 与 @x.setter 配合
来源：http://hz.316326.xyz/gtwhlilhrn.html

[U30] Py：数据类
来源：http://hz.ydzc1.top/gtkblzpfvu.html

@dataclass(slots=True)
来源：http://hz.guannengcc.top/gtkfbdktek.html

[U31] Py：单测
来源：http://hz.yueranfly.top/gtzfhvrajl.html

python -m pytest -q
来源：http://hz.jiagoushi.top/gtdftqgadk.html

[U32] Py：代码格式化
来源：http://hz.yj20258.top/gtqdopmvrq.html

ruff format . && ruff check --fix .
来源：http://hz.tanke756.top/gtpsixnkne.html

[U33] Py：打包发布
来源：http://hz.hfpthk.cn/gtjonkengm.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ydzc1.top/gtgxkxddpq.html

[U34] Py：判断编码
来源：http://hz.hongshengwenyu.top/gtnxrbupfz.html

chardet.detect(raw)
来源：http://hz.jinyuanbaomall.cn/gtsimonabn.html

[U35] Py：发送邮件
来源：http://hz.yuxming.cn/gtpkwqrgfv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.nwbrower.top/gtfhxexpui.html

[U36] Py：定时任务
来源：http://hz.hnqzz.top/gtqwcmqane.html

schedule.every(10).minutes.do(job)
来源：http://hz.vqdsnc.cn/gtntiiloxt.html

[U37] Py：读写 Excel
来源：http://hz.shuidangran.top/gtvwwuxver.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.gogol.net.cn/gtjnuatefn.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhengqikj.top/gtdpukfqkk.html

Path(__file__).resolve().parent
来源：http://hz.feifeiyinyue.top/gttdpkjdfv.html

[U39] Py：判断是否在交互环境
来源：http://hz.jinqigfzy.top/gtfszibwdj.html

sys.stdout.isatty()
来源：http://hz.havefunace.top/gtpytqqaru.html

[U40] Py：打印到标准错误
来源：http://hz.hnxiangtu.top/gtlunpzesd.html

print("err", file=sys.stderr)
来源：http://hz.gotoacloud.top/gtifcserdo.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.daxiang520.top/gtpoojjnwm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.birdmap.top/gtqqvlmytz.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.iojbl.cn/gtnzkjhpnj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.dashuyun.cn/gtwactwtkz.html

[U43] PHP：声明命名空间
来源：http://hz.jiagoushi.top/gtcqmelxao.html

namespace App\Http;
来源：http://hz.vqdsnc.cn/gtxmuetnbm.html

[U44] PHP：开启严格类型
来源：http://hz.tian-w.cn/gtbfmrnagf.html

declare(strict_types=1);
来源：http://hz.sxryk.cn/gtjleheqjp.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yanxiufei.cn/gtjdwuevlp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhiwuduotai.top/gtmopszxtg.html

[U46] PHP：可空类型
来源：http://hz.hfpthk.cn/gtolkevoos.html

?string $name = null
来源：http://hz.yueranfly.top/gtesyqdrai.html

[U47] PHP：联合类型
来源：http://hz.hammf.cn/gtmqudcfgj.html

int|string $id
来源：http://hz.mhx1999.top/gttdnzfrsw.html

[U48] PHP：纯枚举
来源：http://hz.52xcode.cn/gtuayfotet.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.tian-w.cn/gtgkdsokqe.html

[U49] PHP：只读属性
来源：http://hz.aizwys.cn/gtpnptosgx.html

public readonly string $name
来源：http://hz.cdnleiting.top/gtiyaivzzn.html

[U50] PHP：构造器属性提升
来源：http://hz.jqgfzy.top/gtgopuzyxt.html

public function __construct(private int $id) {}
来源：http://hz.shzxlz.cn/gtdzwwlrdg.html

[U51] PHP：数组解构
来源：http://hz.redwolf501.top/gtvfsmtoap.html

[$a, $b] = $arr;
来源：http://hz.nwbrower.top/gtfcpgqpat.html

[U52] PHP：箭头函数
来源：http://hz.feifeiyinyue.top/gtuagbpyqt.html

$double = fn($x) => $x * 2;
来源：http://hz.yanxiufei.cn/gttpkbqfoz.html

[U53] PHP：空合并运算符
来源：http://hz.jyoumei.cn/gtvkrumhvk.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhengqikj.top/gtgeylxvek.html

[U54] PHP：空安全调用
来源：http://hz.hysaishi.cn/gtybpqlvcv.html

$obj?->method()
来源：http://hz.wangshuangyany.cn/gtheksabkz.html

[U55] PHP：match 表达式
来源：http://hz.hnxiangtu.top/gtzluuiwey.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.tanke756.top/gtlpvjbdus.html

[U56] PHP：命名参数
来源：http://hz.aibaodan.cn/gtwweyehmb.html

f(a: 1, b: 2)
来源：http://hz.yvedp.cn/gtpevdolbw.html

[U57] PHP：字符串插值
来源：http://hz.svipenyu.cn/gtarkjsjzt.html

"值: {$a}"
来源：http://hz.xylfe.cn/gtsqbxxzkg.html

[U58] PHP：数组三件套
来源：http://hz.gogol.net.cn/gttznujgto.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.ydzc1.top/gtqoogqbgt.html

[U59] PHP：自定义排序
来源：http://hz.jinqigufen.top/gtwrluddqi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gotoacloud.top/gttnblzfsc.html

[U60] PHP：JSON 编解码
来源：http://hz.cashguo.top/gtamfbrcvn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.shuidangran.top/gterjxhvpc.html

[U61] PHP：正则
来源：http://hz.vqdsnc.cn/gtdowqrdxq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yangfankeji.com/gtlqdbgkur.html

[U62] PHP：日期对象
来源：http://hz.wangshuangyany.cn/gtpmyjfzuo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.iojbl.cn/gtobnznrca.html

[U63] PHP：文件读写
来源：http://hz.vqdsnc.cn/gtdimmjvfh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.bjfxy.top/gtfcancpqb.html

[U64] PHP：目录遍历
来源：http://hz.vqdsnc.cn/gtzqjtaooh.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.pengpengdd.cyou/gtecafdyka.html

[U65] PHP：会话
来源：http://hz.chenlongwang.top/gteyfvoxiu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jianghu66.top/gtfyswolcr.html

[U66] PHP：设置 Cookie
来源：http://hz.yangfankeji.com/gtpyufdzhv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.hammf.cn/gtwhftwzsl.html

[U67] PHP：处理文件上传
来源：http://hz.jianghu66.top/gtoibhztqi.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.52xcode.cn/gtrittnmoz.html

[U68] PHP：PDO 连接
来源：http://hz.wangshuangyany.cn/gtklptoqts.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.chenlongwang.top/gtyzqzybbw.html

[U69] PHP：PDO 预处理
来源：http://hz.quarkkingdee.top/gtufocspmo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zhixingplan.top/gtwmmxnctm.html

[U70] PHP：PDO 事务
来源：http://hz.aizwys.cn/gtzkfvrmhu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zdqjudy.top/gtyvuxjcsj.html

[U71] PHP：抛出异常
来源：http://hz.52xcode.cn/gtmxhtlafd.html

throw new RuntimeException("失败", 500);
来源：http://hz.nwbrower.top/gtweidthgv.html

[U72] PHP：写错误日志
来源：http://hz.zhiwuduotai.top/gtvdfzrlov.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yj20258.top/gtvwnjwnea.html

[U73] PHP：读取 ini 配置
来源：http://hz.shuidangran.top/gtgvjpepyt.html

parse_ini_file("config.ini", true)
来源：http://hz.feifeiyinyue.top/gtehmgpior.html

[U74] PHP：读取环境变量
来源：http://hz.pengpengdd.cyou/gtlfjbyqzf.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hnqzz.top/gtudchsvjw.html

[U75] PHP：依赖注入
来源：http://hz.sweek.top/gthnmflqox.html

composer require psr/container
来源：http://hz.feifeiyinyue.top/gticgompol.html

[U76] PHP：简单路由
来源：http://hz.guowangkeji.top/gtgginydfe.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hfpthk.cn/gtndyreaxi.html

[U77] PHP：模板渲染
来源：http://hz.zhijiandao.cn/gtydkoliea.html

composer require twig/twig
来源：http://hz.cucudq.cn/gtnsnsamjz.html

[U78] PHP：单元测试
来源：http://hz.shanyushiyangkeji.top/gtptioihqc.html

composer require --dev phpunit/phpunit
来源：http://hz.jinyuanbaomall.cn/gtisvezxme.html

[U79] PHP：静态分析
来源：http://hz.iojbl.cn/gtfmkkoudz.html

composer require --dev phpstan/phpstan
来源：http://hz.ybcxt.top/gthxltvjqq.html

[U80] PHP：代码规范修复
来源：http://hz.chenjidiqi.icu/gtwgswgdby.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.wangdashe.top/gtkvczvzgt.html

[U81] JS：初始化项目
来源：http://hz.pycfn.com/gtpepltsul.html

npm init -y;  npm i express
来源：http://hz.gzhubu.top/gtueawapfo.html

[U82] JS：package.json 脚本
来源：http://hz.ydzc1.top/gtwywudfpi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.gaohongyu789.top/gtctrrsruu.html

[U83] JS：ES Module 导入导出
来源：http://hz.yonumen.top/gtwsgffcyt.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.cashguo.top/gtxkcgexha.html

[U84] JS：CommonJS 写法
来源：http://hz.shangyingyoupin.top/gtqshraiiu.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.aibaodan.cn/gtptzuuhak.html

[U85] JS：可选链
来源：http://hz.316326.xyz/gtdbiepzcr.html

a?.b?.c
来源：http://hz.yueranfly.top/gtuzktujhu.html

[U86] JS：空值合并
来源：http://hz.fengsongda.top/gtcykufwsb.html

a ?? b
来源：http://hz.chenjidiqi.icu/gtahobbgvp.html

[U87] JS：解构默认值
来源：http://hz.c1oappe.top/gtqcmpmgmw.html

const { a = 1, b = 2 } = obj;
来源：http://hz.sufxvd.cn/gtdlephoqx.html

[U88] JS：对象展开合并
来源：http://hz.jlsjyb.cn/gtfoqpfymg.html

{ ...a, ...b }
来源：http://hz.zhoulong.xyz/gtyovdwtrr.html

[U89] JS：数组去重
来源：http://hz.yueranfly.top/gtcvxcncub.html

[...new Set(arr)]
来源：http://hz.vqdsnc.cn/gtmezuzxzw.html

[U90] JS：数字数组排序
来源：http://hz.mhx1999.top/gtwzmazscj.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zhoulong.xyz/gtjpklguqa.html

[U91] JS：对象键值遍历
来源：http://hz.316326.xyz/gttxkxhbyc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.aibaodan.cn/gtzreueqgr.html

[U92] JS：深拷贝
来源：http://hz.zhongyouzk.top/gtojyvydxf.html

structuredClone(obj)
来源：http://hz.xingfuxueyuan.xyz/gttrwcuyjj.html

[U93] JS：模板字符串
来源：http://hz.yj20258888.top/gtjmguovgu.html

`共 ${n} 条`
来源：http://hz.sweek.top/gtcyptdyaw.html

[U94] JS：箭头函数
来源：http://hz.yvedp.cn/gtcnffxtmn.html

const double = x => x * 2;
来源：http://hz.zhoulong.xyz/gtoftuljpb.html

[U95] JS：Promise 包装
来源：http://hz.cucudq.cn/gtygonzsdm.html

new Promise((resolve, reject) => {})
来源：http://hz.dashuyun.cn/gtmpuathtq.html

[U96] JS：async/await 与异常
来源：http://hz.zycfv.cn/gtzmtabkrb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xuanzx.com/gtcocmtnfj.html

[U97] JS：并发请求
来源：http://hz.fzhhl.top/gtkylvbmet.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hysaishi.cn/gttwgkcmcm.html

[U98] JS：fetch 带 JSON
来源：http://hz.mhx1999.top/gtoqifetzh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.xingfuxueyuan.xyz/gtidnjmypj.html

[U99] JS：事件监听
来源：http://hz.tanke756.top/gtlqjjarik.html

el.addEventListener("click", e => {})
来源：http://hz.yanxiufei.cn/gttlieoxhg.html

[U100] JS：DOM 查询
来源：http://hz.yangfankeji.com/gtcxgyehow.html

document.querySelector(".item")
来源：http://hz.jlsjyb.cn/gtwksqhewz.html

[U101] JS：classList 操作
来源：http://hz.hfpthk.cn/gtdzoachzc.html

el.classList.toggle("active")
来源：http://hz.gzhubu.top/gtfnpobdvw.html

[U102] JS：本地存储
来源：http://hz.shanyushiyangtech.top/gtmufcopzh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ehwqpu.com/gtjfmvaofr.html

[U103] JS：定时器
来源：http://hz.jinghuilouyu.cn/gtrzeaksgn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jinqigufen.top/gtbjynovpo.html

[U104] JS：防抖
来源：http://hz.jyoumei.cn/gthstwjste.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shuidangran.top/gtkkfwgadz.html

[U105] JS：节流
来源：http://hz.cashguo.top/gtezbindvu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.shanyushiyangkeji.top/gttdwwccqy.html

[U106] JS：日期格式化
来源：http://hz.yanxiufei.cn/gtpnmmvkgb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.hnqzz.top/gtgbgchhxf.html

[U107] JS：数字千分位
来源：http://hz.xziqi.cn/gtjzmmwopl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.0kj1m.cn/gtknxggzks.html

[U108] JS：随机整数
来源：http://hz.bjfxy.top/gtlsiqinak.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.shanyushiyangtech.top/gtyfsluqhm.html

[U109] JS：数组分组
来源：http://hz.cdnleiting.top/gthrvakgev.html

Object.groupBy(arr, x => x.type)
来源：http://hz.9152youxi.cn/gtakikaive.html

[U110] JS：数组分块
来源：http://hz.zhixingplan.top/gtekfvimrm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jyoumei.cn/gttvfzuzgs.html

[U111] JS：对象转 Map
来源：http://hz.xylfe.cn/gtovwoewfo.html

new Map(Object.entries(obj))
来源：http://hz.shuidangran.top/gtpkneinix.html

[U112] JS：字符串补位
来源：http://hz.ivvv.top/gtxxdrbqjo.html

"7".padStart(3, "0")
来源：http://hz.fzhhl.top/gteydotkbr.html

[U113] JS：正则替换全部
来源：http://hz.9152youxi.cn/gtexnhceav.html

s.replaceAll("a", "b")
来源：http://hz.dianchejie.cn/gtyyzjvedb.html

[U114] JS：JSON 深比较
来源：http://hz.xingfuxueyuan.xyz/gthgyhyzzg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.snrcjt.cn/gthablpzuj.html

[U115] JS：生成 UUID
来源：http://hz.zhoulong.xyz/gthvtddwns.html

crypto.randomUUID()
来源：http://hz.hfpthk.cn/gtjvsgadzu.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.nanxuanxn.top/gtndsiptns.html

/** @param {string} name */ function f(name) {}
来源：http://hz.316326.xyz/gtmyzstxmz.html

[U117] JS：单元测试
来源：http://hz.shuidangran.top/gtklryolsi.html

npm i -D vitest;  npx vitest
来源：http://hz.yangfankeji.com/gtskawaopp.html

[U118] JS：开发服务器
来源：http://hz.zhaomingkeji.xyz/gtjxhetvcu.html

npm i -D vite;  npx vite
来源：http://hz.jinyuanbaomall.cn/gtisnoyhvn.html

[U119] JS：生产构建
来源：http://hz.guannengcc.top/gttwkaozrp.html

npx vite build
来源：http://hz.c1oappe.top/gtqziuwvgr.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yanxiufei.cn/gttmrkgtbd.html

import.meta.env.VITE_API_URL
来源：http://hz.feifeiyinyue.top/gtrlwwicmi.html

================================================================================
来源：http://hz.0kj1m.cn/gtpccttbcy.html

统计汇总
来源：http://hz.gogol.net.cn/gtazabmylr.html

================================================================================
来源：http://hz.xylfe.cn/gteytcjbfn.html

按语言统计（条）：
来源：http://hz.jlsjyb.cn/gthyjgsmay.html

Python ......... 252
来源：http://hz.cqqwz.cn/gtvktparph.html

PHP ............ 252
来源：http://hz.hywenlv.cn/gteqqyrtou.html

JavaScript ..... 252
来源：http://hz.quarkkingdee.top/gteklybyfh.html

TypeScript ..... 212
来源：http://hz.guowangkeji.top/gtnjgkevll.html

Java ........... 212
来源：http://hz.bjfxy.top/gtemgbqqkz.html

Go ............. 212
来源：http://hz.sxryk.cn/gtaqzwmfxp.html

Ruby ........... 212
来源：http://hz.jinyuanbaomall.cn/gtrdqefequ.html

C# ............. 212
来源：http://hz.ywan-chungtsiang.top/gtreojcmxi.html

C .............. 30
来源：http://hz.tian-w.cn/gtrtragezm.html

C++ ............ 30
来源：http://hz.jinqigufen.top/gtmrdxrmvv.html

SQL ............ 90
来源：http://hz.snrcjt.cn/gtqgzrvsur.html

Bash ........... 80
来源：http://hz.pycfn.com/gtgoafxrul.html

Kotlin ......... 15
来源：http://hz.cdnleiting.top/gtytixfeqi.html

Swift .......... 15
来源：http://hz.tian-w.cn/gtripcltwl.html

Lua ............ 10
来源：http://hz.ybcxt.top/gtmcofefox.html

Perl ........... 10
来源：http://hz.svipenyu.cn/gtodjesepg.html

Scala .......... 10
来源：http://hz.ppjwa.cn/gtdpqjnzjq.html

------------------------------------
来源：http://hz.sysykeji.top/gtytfsgcbt.html

合计 ........... 2106 条
来源：http://hz.hnxiangtu.top/gtfruwkdtr.html

按章节统计：
来源：http://hz.hfpthk.cn/gtotjibvhq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.dashuyun.cn/gtlicxcgmf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jlsjyb.cn/gtblqotqtm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.shuidangran.top/gtqyozjdiw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yuanzhike.top/gtvgejukcv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yueranfly.top/gthsbgjjkc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jianghu66.top/gtkghvaazj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.xylfe.cn/gtfmybhxat.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.cdnleiting.top/gtttrabiai.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zhixingplan.top/gtuvvgjkaz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.c1oappe.top/gtqovxpsyp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.chenzaomai.com/gtoygnezxh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jlsjyb.cn/gttfvpfirp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhongyouzk.top/gtggnztsfi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yvedp.cn/gtijadzqmy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.meibo888.top/gtejwthfau.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yuanzhike.top/gtunxfyaqa.html

Q SQL 专题                              90
来源：http://hz.jinyuanbaomall.cn/gtvqfknann.html

R Bash 专题                             80
来源：http://hz.xuanzx.com/gtytuplmdd.html

S C / C++ 专题                          60
来源：http://hz.jlsjyb.cn/gtgndicwzj.html

T 其他语言补充                          60
来源：http://hz.xuanzx.com/gtjdgzrifq.html

U 高频实用片段                         120
来源：http://hz.ivvv.top/gtevdliqxz.html

------------------------------------
来源：http://hz.zycfv.cn/gtqlmnegbt.html

合计                                  2106 条
来源：http://hz.sufxvd.cn/gtqerioklp.html

--------------------------------------------------------------------------------
来源：http://hz.jqgfzy.top/gtxhfzzrlp.html

使用提醒
来源：http://hz.sufxvd.cn/gtvghufcmy.html

--------------------------------------------------------------------------------
来源：http://hz.hywenlv.cn/gtunyquckm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.daria6918.cn/gtltyoggba.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zdqjudy.top/gtthrsjizz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hywenlv.cn/gtevsdhbkh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.316326.xyz/gtgxxcynpa.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.gogol.net.cn/gtwnbjrzxg.html

—— 文件结束 ——
来源：http://hz.nanxuanxn.top/gtqvppamrn.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtobrnpzwp.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ehwqpu.com/gtofwmqdak.html

Common Programming Examples Cheat Book
来源：http://hz.yueranfly.top/gtgtyruuwu.html

================================================================================
来源：http://hz.cashguo.top/gtxfjonsya.html

【收录内容】
来源：http://hz.jinghuilouyu.cn/gtjjuzaeqo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.gzhubu.top/gtvbltcvmx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.ywan-chungtsiang.top/gtambyrwpp.html

SQL · Bash · C · C++
来源：http://hz.meibo888.top/gtjuqiwbnb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ydjk.org.cn/gtissiswxl.html

【使用说明】
来源：http://hz.pengpengdd.cyou/gtgksjmjvx.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.meibo888.top/gtprbpwjnm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.guannengcc.top/gtqykpdouy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jinghuilouyu.cn/gtncebvoch.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.wangdashe.top/gtjipgciwp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.gogol.net.cn/gtfsuzccui.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.snrcjt.cn/gtqiuztcxq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jqgufenzy.top/gtrtgfetmn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.daxiang520.top/gticvbxurv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.andypj.xyz/gtlhskpvjp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jianghu66.top/gtdqbwzixd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.xuetiantiany.cn/gtrjttlwng.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.xuanzx.com/gtzrxeabue.html

【文件统计】
来源：http://hz.redwolf501.top/gtxqxfzwic.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.cheryme.top/gtyerepfdj.html

--------------------------------------------------------------------------------
来源：http://hz.smart0.xyz/gtvkkvkqhf.html

目  录
来源：http://hz.jqgfzy.top/gtuyljsshp.html

--------------------------------------------------------------------------------
来源：http://hz.hnxiangtu.top/gtwwwoujbu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.yongpay.top/gtklswpnfy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.ydzc1.top/gtmrnjrksb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jinqigufen.top/gtlddoexyc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.birdmap.top/gtstbxqats.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.fzhhl.top/gtdppyiqid.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.cdnleiting.top/gthtgrxcjh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jinqigfzy.top/gtrihurork.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yuxming.cn/gtuuhnwoqn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.chenzaomai.com/gtsqvohbop.html


<!-- 参考信息 -->