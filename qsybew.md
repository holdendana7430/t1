代发 wailian999

[U17] Py：初始化日志
来源：http://hz.wangshuangyany.cn/gtlwzgxkpb.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.haohaochexian.top/gtkciyddye.html

[U18] Py：预编译正则
来源：http://hz.jinqigfzy.top/gtmattqxbv.html

pat = re.compile(r"\d+")
来源：http://hz.snrcjt.cn/gtgiacvkle.html

[U19] Py：正则替换带回调
来源：http://hz.jinghuilouyu.cn/gtlosbhclt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.0kj1m.cn/gtdhxyzgup.html

[U20] Py：缓存函数结果
来源：http://hz.xuanzx.com/gteyfslajv.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yj20258888.top/gtwjidwlei.html

[U21] Py：自定义上下文管理器
来源：http://hz.ydzc1.top/gtaeynnkhp.html

@contextlib.contextmanager
来源：http://hz.dashuyun.cn/gtneciwblk.html

[U22] Py：矩阵转置
来源：http://hz.cucudq.cn/gtheesazro.html

list(zip(*m))
来源：http://hz.guowangkeji.top/gtufxnvidt.html

[U23] Py：分块读取大文件
来源：http://hz.shuidangran.top/gtoufzypxy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.redwolf501.top/gtlofwbiel.html

[U24] Py：路径操作
来源：http://hz.sufxvd.cn/gtppmqewdx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.shzxlz.cn/gtwxtfhhrt.html

[U25] Py：CSV 按字典读
来源：http://hz.gogol.net.cn/gtnpjusogs.html

csv.DictReader(f)
来源：http://hz.shanyushiyangkeji.top/gtvrnpvezg.html

[U26] Py：并发下载
来源：http://hz.xuanzx.com/gtsdemiarw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhiwuduotai.top/gtphecavnp.html

[U27] Py：异步 HTTP
来源：http://hz.feifeiyinyue.top/gtyphhiabo.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.chenjidiqi.icu/gttayclmtb.html

[U28] Py：类型别名
来源：http://hz.gzhubu.top/gtyuadhzmj.html

UserId = int
来源：http://hz.jiagoushi.top/gtbfsgogde.html

[U29] Py：属性校验
来源：http://hz.feifeiyinyue.top/gtnwbbmorj.html

@property 与 @x.setter 配合
来源：http://hz.chenzaomai.com/gthmqgehiu.html

[U30] Py：数据类
来源：http://hz.yj20258.top/gtejzttfjp.html

@dataclass(slots=True)
来源：http://hz.jianghu66.top/gtpvdklues.html

[U31] Py：单测
来源：http://hz.ivvv.top/gtqzhmeics.html

python -m pytest -q
来源：http://hz.svipenyu.cn/gthagkcoax.html

[U32] Py：代码格式化
来源：http://hz.ywan-chungtsiang.top/gtoqiklldi.html

ruff format . && ruff check --fix .
来源：http://hz.9152youxi.cn/gtnxsmhjhg.html

[U33] Py：打包发布
来源：http://hz.ydzc1.top/gtpskxabdi.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.sysykeji.top/gtaforikml.html

[U34] Py：判断编码
来源：http://hz.yangfankeji.com/gtshwuwlll.html

chardet.detect(raw)
来源：http://hz.jinyuanbaomall.cn/gtszjkvzym.html

[U35] Py：发送邮件
来源：http://hz.hnxiangtu.top/gtbyxjqfei.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.gaohongyu789.top/gtoivqzlmy.html

[U36] Py：定时任务
来源：http://hz.shanyushiyangkeji.top/gtfzxjtobf.html

schedule.every(10).minutes.do(job)
来源：http://hz.ywan-chungtsiang.top/gtbiwlaavc.html

[U37] Py：读写 Excel
来源：http://hz.kuanghao11.cn/gtuqoufsbj.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jinghuilouyu.cn/gtognvojmt.html

[U38] Py：获取脚本所在目录
来源：http://hz.iojbl.cn/gtksefznzh.html

Path(__file__).resolve().parent
来源：http://hz.fengsongda.top/gthmgdqzba.html

[U39] Py：判断是否在交互环境
来源：http://hz.xuetiantiany.cn/gtsdelborx.html

sys.stdout.isatty()
来源：http://hz.jinyuanbaomall.cn/gtzidophkt.html

[U40] Py：打印到标准错误
来源：http://hz.svipenyu.cn/gttgmcxcjk.html

print("err", file=sys.stderr)
来源：http://hz.yonumen.top/gtkcnibeox.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.pengpengdd.cyou/gtdqcutirx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.chenlongwang.top/gtafyyuwgh.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xylfe.cn/gtqzfqkaye.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.dashuyun.cn/gtddbkjdad.html

[U43] PHP：声明命名空间
来源：http://hz.cdnleiting.top/gthtohnmgl.html

namespace App\Http;
来源：http://hz.mhx1999.top/gttwewrqzn.html

[U44] PHP：开启严格类型
来源：http://hz.quarkkingdee.top/gttoandhoi.html

declare(strict_types=1);
来源：http://hz.jyoumei.cn/gtpmvschkp.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ppjwa.cn/gtvkkprkzz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gtpbnhtqwr.html

[U46] PHP：可空类型
来源：http://hz.ppjwa.cn/gthiqpmkeu.html

?string $name = null
来源：http://hz.jyoumei.cn/gtbybeldql.html

[U47] PHP：联合类型
来源：http://hz.hnqzz.top/gtmoajdqmr.html

int|string $id
来源：http://hz.shuidangran.top/gtzsudqktv.html

[U48] PHP：纯枚举
来源：http://hz.sxryk.cn/gthqnpxyef.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jinghuilouyu.cn/gtefwjityr.html

[U49] PHP：只读属性
来源：http://hz.pengpengdd.cyou/gttcecnfgi.html

public readonly string $name
来源：http://hz.shanyushiyangkeji.top/gtifcmbnqi.html

[U50] PHP：构造器属性提升
来源：http://hz.hnqzz.top/gtywixffvi.html

public function __construct(private int $id) {}
来源：http://hz.yongpay.top/gtxhvoxgek.html

[U51] PHP：数组解构
来源：http://hz.zdqjudy.top/gtqlawjkcb.html

[$a, $b] = $arr;
来源：http://hz.wangdashe.top/gtgjejliaw.html

[U52] PHP：箭头函数
来源：http://hz.redwolf501.top/gtkpgjzlpn.html

$double = fn($x) => $x * 2;
来源：http://hz.ywan-chungtsiang.top/gthalwpzsz.html

[U53] PHP：空合并运算符
来源：http://hz.shuidangran.top/gtdyofywjg.html

$v = $a ?? $b ?? "default";
来源：http://hz.birdmap.top/gtqqhqmoii.html

[U54] PHP：空安全调用
来源：http://hz.pengpengdd.cyou/gtudfmzaid.html

$obj?->method()
来源：http://hz.haohaochexian.top/gtlohvihkq.html

[U55] PHP：match 表达式
来源：http://hz.guannengcc.top/gtpfbpqvqd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.hnxiangtu.top/gtubnmoscj.html

[U56] PHP：命名参数
来源：http://hz.ywan-chungtsiang.top/gtuwcxayvs.html

f(a: 1, b: 2)
来源：http://hz.guowangkeji.top/gtqclwijgy.html

[U57] PHP：字符串插值
来源：http://hz.zdqjudy.top/gtwpivqnvp.html

"值: {$a}"
来源：http://hz.zycfv.cn/gtlnpgryji.html

[U58] PHP：数组三件套
来源：http://hz.jinghuilouyu.cn/gtzcxbreiq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.sweek.top/gtoynvyasi.html

[U59] PHP：自定义排序
来源：http://hz.yueranfly.top/gtlwijdspu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tianlin.xyz/gtllxupqqe.html

[U60] PHP：JSON 编解码
来源：http://hz.yuxming.cn/gtkpjailiy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.cqqwz.cn/gtjevkffeu.html

[U61] PHP：正则
来源：http://hz.52xcode.cn/gtlddhbbpp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.andypj.xyz/gtoheoetjm.html

[U62] PHP：日期对象
来源：http://hz.yonumen.top/gtfkhynove.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.aibaodan.cn/gtqxduugsr.html

[U63] PHP：文件读写
来源：http://hz.jqgfzy.top/gtlwjbkhww.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.chenzaomai.com/gtpwscfvem.html

[U64] PHP：目录遍历
来源：http://hz.jianghu66.top/gtdruijjsu.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.sweek.top/gtnzwrlgbd.html

[U65] PHP：会话
来源：http://hz.chenlongwang.top/gtblgiseyz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.shangyingyoupin.top/gttvrnlico.html

[U66] PHP：设置 Cookie
来源：http://hz.cucudq.cn/gtcqjteoru.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.hnxiangtu.top/gtxahharsy.html

[U67] PHP：处理文件上传
来源：http://hz.ydzc1.top/gtgybjxpal.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.feifeiyinyue.top/gteiyhmeed.html

[U68] PHP：PDO 连接
来源：http://hz.svipenyu.cn/gtvfhltvpk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.shuidangran.top/gtefwudocj.html

[U69] PHP：PDO 预处理
来源：http://hz.shanyushiyangtech.top/gtdkjorhyu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.tianlin.xyz/gtjatrxyfq.html

[U70] PHP：PDO 事务
来源：http://hz.zhiwuduotai.top/gtznqjbuaq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.cqqwz.cn/gtkcpxgwmv.html

[U71] PHP：抛出异常
来源：http://hz.ybcxt.top/gtrmipyjsq.html

throw new RuntimeException("失败", 500);
来源：http://hz.smart0.xyz/gtywkbyvkt.html

[U72] PHP：写错误日志
来源：http://hz.daria6918.cn/gtboimspld.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yonumen.top/gtqvsisgcr.html

[U73] PHP：读取 ini 配置
来源：http://hz.gaohongyu789.top/gtnfledfju.html

parse_ini_file("config.ini", true)
来源：http://hz.xziqi.cn/gtfmhghggj.html

[U74] PHP：读取环境变量
来源：http://hz.cashguo.top/gtlndnreac.html

getenv("APP_ENV") ?: "production"
来源：http://hz.ywan-chungtsiang.top/gtjqddhlsz.html

[U75] PHP：依赖注入
来源：http://hz.nanxinkj.top/gtmnxoqygu.html

composer require psr/container
来源：http://hz.zhengqikj.top/gthfizjryg.html

[U76] PHP：简单路由
来源：http://hz.zdqjudy.top/gttknhptyi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.ivvv.top/gthkvbuslm.html

[U77] PHP：模板渲染
来源：http://hz.iojbl.cn/gttaofrwpy.html

composer require twig/twig
来源：http://hz.pycfn.com/gtyfceqdiq.html

[U78] PHP：单元测试
来源：http://hz.guannengcc.top/gtjglhnffp.html

composer require --dev phpunit/phpunit
来源：http://hz.zhaomingkeji.xyz/gtlquujgqg.html

[U79] PHP：静态分析
来源：http://hz.shanyushiyangtech.top/gtekxzvttk.html

composer require --dev phpstan/phpstan
来源：http://hz.pengpengdd.cyou/gtxbdkpagf.html

[U80] PHP：代码规范修复
来源：http://hz.0kj1m.cn/gtukhhtige.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.sxryk.cn/gtsqjmxhph.html

[U81] JS：初始化项目
来源：http://hz.xingfuxueyuan.xyz/gtvpxwuibf.html

npm init -y;  npm i express
来源：http://hz.xziqi.cn/gtjrwuydjb.html

[U82] JS：package.json 脚本
来源：http://hz.jqgfzy.top/gtlejrrvay.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zdqjudy.top/gtnswwpemi.html

[U83] JS：ES Module 导入导出
来源：http://hz.shangyingyoupin.top/gtegvfgmby.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.hfpthk.cn/gtbpyxhfhs.html

[U84] JS：CommonJS 写法
来源：http://hz.zhixingplan.top/gtqlykduie.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.aibaodan.cn/gtbvqcliwc.html

[U85] JS：可选链
来源：http://hz.gotoacloud.top/gtaoccgavw.html

a?.b?.c
来源：http://hz.ehwqpu.com/gtocgyfkyf.html

[U86] JS：空值合并
来源：http://hz.gzhubu.top/gtzhfrmafh.html

a ?? b
来源：http://hz.hnqzz.top/gttotqyxfz.html

[U87] JS：解构默认值
来源：http://hz.316326.xyz/gtcqiypptd.html

const { a = 1, b = 2 } = obj;
来源：http://hz.ehwqpu.com/gtgjbuzcvu.html

[U88] JS：对象展开合并
来源：http://hz.ydjk.org.cn/gtunpdazaa.html

{ ...a, ...b }
来源：http://hz.sysykeji.top/gthxwqwpzn.html

[U89] JS：数组去重
来源：http://hz.ehwqpu.com/gtwimqfian.html

[...new Set(arr)]
来源：http://hz.tanke756.top/gtmfhowgdj.html

[U90] JS：数字数组排序
来源：http://hz.yonumen.top/gtjlerwupi.html

[...arr].sort((a, b) => a - b)
来源：http://hz.sysykeji.top/gtwjqrkiiv.html

[U91] JS：对象键值遍历
来源：http://hz.9152youxi.cn/gtprwqyyes.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.xuetiantiany.cn/gtdemfvmeq.html

[U92] JS：深拷贝
来源：http://hz.zhongyouzk.top/gttxwronrd.html

structuredClone(obj)
来源：http://hz.yuanzhike.top/gtdqvxnomd.html

[U93] JS：模板字符串
来源：http://hz.gogol.net.cn/gteuqkdtmn.html

`共 ${n} 条`
来源：http://hz.guannengcc.top/gtifqopyot.html

[U94] JS：箭头函数
来源：http://hz.chenjidiqi.icu/gtruyggkql.html

const double = x => x * 2;
来源：http://hz.guannengcc.top/gtxbmnwlbd.html

[U95] JS：Promise 包装
来源：http://hz.havefunace.top/gtvepkzeyd.html

new Promise((resolve, reject) => {})
来源：http://hz.fengsongda.top/gtgtbhjhzk.html

[U96] JS：async/await 与异常
来源：http://hz.guowangkeji.top/gtarthwgzz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yanxiufei.cn/gttqdmmkij.html

[U97] JS：并发请求
来源：http://hz.fzhhl.top/gtzrkykuld.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuxming.cn/gtjhkclain.html

[U98] JS：fetch 带 JSON
来源：http://hz.yj20258.top/gtodfwedth.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.guowangkeji.top/gtfqtchtku.html

[U99] JS：事件监听
来源：http://hz.ybcxt.top/gtwkpxwaxg.html

el.addEventListener("click", e => {})
来源：http://hz.shzxlz.cn/gtlqxyynrl.html

[U100] JS：DOM 查询
来源：http://hz.feifeiyinyue.top/gtqkqdablx.html

document.querySelector(".item")
来源：http://hz.aibaodan.cn/gthrfqdsis.html

[U101] JS：classList 操作
来源：http://hz.jqgufenzy.top/gtrdxbajgk.html

el.classList.toggle("active")
来源：http://hz.hnxiangtu.top/gtoujxlgud.html

[U102] JS：本地存储
来源：http://hz.gogol.net.cn/gtaztmhapo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jinqigufen.top/gtotwbayib.html

[U103] JS：定时器
来源：http://hz.yongpay.top/gtvnrhulrl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jiagoushi.top/gtyzwcvgkr.html

[U104] JS：防抖
来源：http://hz.gzhubu.top/gtzfiennpt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnxiangtu.top/gtuhndhnzs.html

[U105] JS：节流
来源：http://hz.mhx1999.top/gtzqbsxmoh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhaomingkeji.xyz/gtfwxpovig.html

[U106] JS：日期格式化
来源：http://hz.sxryk.cn/gtovlahfeh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.guowangkeji.top/gtjhxpovml.html

[U107] JS：数字千分位
来源：http://hz.bjfxy.top/gtglndrdps.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yuxming.cn/gtmegnagsy.html

[U108] JS：随机整数
来源：http://hz.0kj1m.cn/gtabvxxbmz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.fengsongda.top/gtplemqsws.html

[U109] JS：数组分组
来源：http://hz.dashuyun.cn/gtvhwrdxpb.html

Object.groupBy(arr, x => x.type)
来源：http://hz.iojbl.cn/gtagynvrxd.html

[U110] JS：数组分块
来源：http://hz.yj20258.top/gtnkyilxny.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.iojbl.cn/gtqpzfpaer.html

[U111] JS：对象转 Map
来源：http://hz.9152youxi.cn/gtuqbwofrb.html

new Map(Object.entries(obj))
来源：http://hz.yj20258888.top/gtkpjkakok.html

[U112] JS：字符串补位
来源：http://hz.snrcjt.cn/gtamxoqcwn.html

"7".padStart(3, "0")
来源：http://hz.zhaomingkeji.xyz/gtunafcncf.html

[U113] JS：正则替换全部
来源：http://hz.gogol.net.cn/gtadqedrmk.html

s.replaceAll("a", "b")
来源：http://hz.hysaishi.cn/gtbeeajtcf.html

[U114] JS：JSON 深比较
来源：http://hz.cucudq.cn/gtmawyuuob.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ybcxt.top/gtbbvnlrax.html

[U115] JS：生成 UUID
来源：http://hz.jlsjyb.cn/gtaiyjlorz.html

crypto.randomUUID()
来源：http://hz.fengsongda.top/gtfchsxulz.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hysaishi.cn/gtwoylsjtu.html

/** @param {string} name */ function f(name) {}
来源：http://hz.redwolf501.top/gtspsyzqfc.html

[U117] JS：单元测试
来源：http://hz.sweek.top/gtcmnfepfv.html

npm i -D vitest;  npx vitest
来源：http://hz.vqdsnc.cn/gtopfohach.html

[U118] JS：开发服务器
来源：http://hz.ydjk.org.cn/gtpkkrtkfn.html

npm i -D vite;  npx vite
来源：http://hz.yueranfly.top/gtwfvfbdom.html

[U119] JS：生产构建
来源：http://hz.svipenyu.cn/gtowslpyvb.html

npx vite build
来源：http://hz.pycfn.com/gthrtckkox.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hammf.cn/gtdgpwyrng.html

import.meta.env.VITE_API_URL
来源：http://hz.nanxuanxn.top/gtiqeaozly.html

================================================================================
来源：http://hz.jianghu66.top/gtfnhymhox.html

统计汇总
来源：http://hz.xylfe.cn/gtldydzowj.html

================================================================================
来源：http://hz.gotoacloud.top/gtttrgpiwz.html

按语言统计（条）：
来源：http://hz.yonumen.top/gtdsohopuz.html

Python ......... 252
来源：http://hz.gogol.net.cn/gtmnkoylsq.html

PHP ............ 252
来源：http://hz.aibaodan.cn/gtvztnxsqy.html

JavaScript ..... 252
来源：http://hz.cucudq.cn/gthajmhuwu.html

TypeScript ..... 212
来源：http://hz.zhongyouzk.top/gtmkvxmyat.html

Java ........... 212
来源：http://hz.yj20258888.top/gthvxxoyac.html

Go ............. 212
来源：http://hz.nwbrower.top/gtqxemcukx.html

Ruby ........... 212
来源：http://hz.0kj1m.cn/gtuvrgaqeg.html

C# ............. 212
来源：http://hz.tianlin.xyz/gtpckmsesq.html

C .............. 30
来源：http://hz.zhongyouzk.top/gtxdiymoau.html

C++ ............ 30
来源：http://hz.ivvv.top/gtzuxvbfoa.html

SQL ............ 90
来源：http://hz.ydjk.org.cn/gtbenjqbae.html

Bash ........... 80
来源：http://hz.yonumen.top/gtpmfxghrr.html

Kotlin ......... 15
来源：http://hz.hammf.cn/gtdsnvezsc.html

Swift .......... 15
来源：http://hz.wangdashe.top/gtgdwxcuwl.html

Lua ............ 10
来源：http://hz.pycfn.com/gtjqoakznz.html

Perl ........... 10
来源：http://hz.meibo888.top/gtrcadehao.html

Scala .......... 10
来源：http://hz.zhengqikj.top/gtpxprswjr.html

------------------------------------
来源：http://hz.xziqi.cn/gtmudseogc.html

合计 ........... 2106 条
来源：http://hz.aizwys.cn/gtnzfhvqkg.html

按章节统计：
来源：http://hz.cashguo.top/gtpjqnqykk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xingfuxueyuan.xyz/gtggxjodqp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.sxryk.cn/gtqyfccuym.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.smart0.xyz/gtezrboszx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.xinyue.icu/gtbtgwgzgz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.ydzc1.top/gtkeoxdixr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.mhx1999.top/gtcjrgoxip.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.shanyushiyangtech.top/gtpordzgzs.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhaomingkeji.xyz/gtpeghbmzl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yongpay.top/gtrruibbnu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.wangdashe.top/gtyibamnin.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.ydjk.org.cn/gtizpvwgiv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.ppjwa.cn/gtdsksyise.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.tianlin.xyz/gtlwbobeyw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.daria6918.cn/gtzkyuamvs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.shangyingyoupin.top/gtyyvmccka.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.sweek.top/gtdjpyktbl.html

Q SQL 专题                              90
来源：http://hz.nwbrower.top/gtrcnlnprh.html

R Bash 专题                             80
来源：http://hz.haohaochexian.top/gtryhetfns.html

S C / C++ 专题                          60
来源：http://hz.chenjidiqi.icu/gthcrrcnmu.html

T 其他语言补充                          60
来源：http://hz.nanxuanxn.top/gtzblpueoz.html

U 高频实用片段                         120
来源：http://hz.chenzaomai.com/gtwmvnlist.html

------------------------------------
来源：http://hz.bjfxy.top/gtsddoxxij.html

合计                                  2106 条
来源：http://hz.zhaomingkeji.xyz/gtnpbzbgst.html

--------------------------------------------------------------------------------
来源：http://hz.kuanghao11.cn/gtghbqrcqr.html

使用提醒
来源：http://hz.gotoacloud.top/gtjcredamh.html

--------------------------------------------------------------------------------
来源：http://hz.hywenlv.cn/gtffsrrsgr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.birdmap.top/gtnurivzgt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.xuanzx.com/gtnpbfzryq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.svipenyu.cn/gtarnicoox.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zhoulong.xyz/gthlwxnume.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.shanyushiyangkeji.top/gtbfhpvlav.html

—— 文件结束 ——
来源：http://hz.hnxiangtu.top/gtwcxnlqgi.html

================================================================================
来源：http://hz.jyoumei.cn/gtzmoeiebl.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ehwqpu.com/gtvsqrizyv.html

Common Programming Examples Cheat Book
来源：http://hz.ywan-chungtsiang.top/gtojbxerda.html

================================================================================
来源：http://hz.havefunace.top/gtyvlebdph.html

【收录内容】
来源：http://hz.aizwys.cn/gtbrzxcutw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.feifeiyinyue.top/gtqdydxoul.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.birdmap.top/gtggqvmlwf.html

SQL · Bash · C · C++
来源：http://hz.sxryk.cn/gtqencgiuw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.c1oappe.top/gtaolstgqo.html

【使用说明】
来源：http://hz.ydjk.org.cn/gtazuqyztf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhixingplan.top/gtbiqjsnvm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.c1oappe.top/gtxjqeowyn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.gogol.net.cn/gtbdoubbdl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.hfpthk.cn/gtwkxxzjis.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.kuanghao11.cn/gtopbepshd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.tanke756.top/gtieabtexz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.c1oappe.top/gtjgrogixe.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yueranfly.top/gtxuoalsue.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jiagoushi.top/gtfjmuadmt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.ydjk.org.cn/gtojufoaao.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.52xcode.cn/gtbhoyhzfd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.zhijiandao.cn/gtznvlgsja.html

【文件统计】
来源：http://hz.gzhubu.top/gttciuladg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.guowangkeji.top/gtppqoqmod.html

--------------------------------------------------------------------------------
来源：http://hz.mhx1999.top/gtczinkxhl.html

目  录
来源：http://hz.nanxuanxn.top/gthhmcbmzv.html

--------------------------------------------------------------------------------
来源：http://hz.zhaomingkeji.xyz/gtzwntvhkk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.chenzaomai.com/gtnjlzlrch.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.shanyushiyangtech.top/gtkcrrfvhc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.haohaochexian.top/gtzbicbiqg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.havefunace.top/gtvnxcubrs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.52xcode.cn/gtgrewpbxj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yongpay.top/gtufixrbkl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jianghu66.top/gtrxvvlsic.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zhoulong.xyz/gtdyuqmbzk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jinqigufen.top/gtyweeugqe.html


<!-- 参考信息 -->