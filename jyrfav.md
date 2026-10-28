代发 wailian999

[U17] Py：初始化日志
来源：http://hz.hnxiangtu.top/gtthwsggag.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.fengsongda.top/gtygiykeec.html

[U18] Py：预编译正则
来源：http://hz.316326.xyz/gtapgppjxv.html

pat = re.compile(r"\d+")
来源：http://hz.zhengqikj.top/gtruvlzqjr.html

[U19] Py：正则替换带回调
来源：http://hz.haohaochexian.top/gtqaraposm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jianghu66.top/gtgekjvwfe.html

[U20] Py：缓存函数结果
来源：http://hz.9152youxi.cn/gtqgapklyb.html

@functools.lru_cache(maxsize=None)
来源：http://hz.cdnleiting.top/gtpczdpbgm.html

[U21] Py：自定义上下文管理器
来源：http://hz.ywan-chungtsiang.top/gthpgykgdf.html

@contextlib.contextmanager
来源：http://hz.yj20258.top/gtinuvjrxe.html

[U22] Py：矩阵转置
来源：http://hz.cdnleiting.top/gtgzvwuxlj.html

list(zip(*m))
来源：http://hz.cucudq.cn/gtyahmmkwl.html

[U23] Py：分块读取大文件
来源：http://hz.birdmap.top/gtbyeccvnu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.fzhhl.top/gtnvesoqaq.html

[U24] Py：路径操作
来源：http://hz.zhiwuduotai.top/gtyqzjhiky.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.tian-w.cn/gtkuizlxds.html

[U25] Py：CSV 按字典读
来源：http://hz.hammf.cn/gtauaxchgx.html

csv.DictReader(f)
来源：http://hz.xylfe.cn/gtwmxcllgt.html

[U26] Py：并发下载
来源：http://hz.0kj1m.cn/gtfmsjrgft.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jlsjyb.cn/gtwvniyoam.html

[U27] Py：异步 HTTP
来源：http://hz.ivvv.top/gtwcqeambk.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.hammf.cn/gtzrogrryv.html

[U28] Py：类型别名
来源：http://hz.hongshengwenyu.top/gtvqchcpxt.html

UserId = int
来源：http://hz.chenzaomai.com/gtahjikgdg.html

[U29] Py：属性校验
来源：http://hz.sysykeji.top/gtynmguuai.html

@property 与 @x.setter 配合
来源：http://hz.sxryk.cn/gtfbrziawb.html

[U30] Py：数据类
来源：http://hz.wangdashe.top/gtrgnjsbmb.html

@dataclass(slots=True)
来源：http://hz.zhengqikj.top/gthcydguor.html

[U31] Py：单测
来源：http://hz.dashuyun.cn/gtzninxwqy.html

python -m pytest -q
来源：http://hz.jiagoushi.top/gthmijepnc.html

[U32] Py：代码格式化
来源：http://hz.hfpthk.cn/gtstkonylj.html

ruff format . && ruff check --fix .
来源：http://hz.quarkkingdee.top/gtrhlhdssu.html

[U33] Py：打包发布
来源：http://hz.xuetiantiany.cn/gtjwgkcpuu.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ywan-chungtsiang.top/gtwcarimps.html

[U34] Py：判断编码
来源：http://hz.gotoacloud.top/gtfbvpjvxx.html

chardet.detect(raw)
来源：http://hz.haohaochexian.top/gtvpdvglio.html

[U35] Py：发送邮件
来源：http://hz.hywenlv.cn/gtnpjfwwmh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.quarkkingdee.top/gtxhbvsful.html

[U36] Py：定时任务
来源：http://hz.cashguo.top/gtmmwnjpuv.html

schedule.every(10).minutes.do(job)
来源：http://hz.yvedp.cn/gtudkrlibv.html

[U37] Py：读写 Excel
来源：http://hz.yj20258888.top/gtrkcdatgw.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.quarkkingdee.top/gtkshpovdq.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhixingplan.top/gtuclxbimq.html

Path(__file__).resolve().parent
来源：http://hz.jyoumei.cn/gtdmlcmfkp.html

[U39] Py：判断是否在交互环境
来源：http://hz.tian-w.cn/gtxlafxgos.html

sys.stdout.isatty()
来源：http://hz.cqqwz.cn/gtblyrbawm.html

[U40] Py：打印到标准错误
来源：http://hz.0kj1m.cn/gtwsojzbcb.html

print("err", file=sys.stderr)
来源：http://hz.snrcjt.cn/gtpmsnrgfs.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.ywan-chungtsiang.top/gtsqukcwqu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhixingplan.top/gtzmvljmgn.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.ivvv.top/gtclxyxrcj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.xinyue.icu/gtlmhgghpw.html

[U43] PHP：声明命名空间
来源：http://hz.feifeiyinyue.top/gtlzwltbnb.html

namespace App\Http;
来源：http://hz.zhoulong.xyz/gtlgjrygkc.html

[U44] PHP：开启严格类型
来源：http://hz.cdnleiting.top/gthizewhrk.html

declare(strict_types=1);
来源：http://hz.gogol.net.cn/gtkrfksuip.html

[U45] PHP：类型声明与返回类型
来源：http://hz.svipenyu.cn/gtqyxbfzue.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.haohaochexian.top/gtploneuzx.html

[U46] PHP：可空类型
来源：http://hz.hywenlv.cn/gtglvytgbr.html

?string $name = null
来源：http://hz.meibo888.top/gtaqsfaele.html

[U47] PHP：联合类型
来源：http://hz.sysykeji.top/gttspnrhqp.html

int|string $id
来源：http://hz.xingfuxueyuan.xyz/gtwxxilfyg.html

[U48] PHP：纯枚举
来源：http://hz.pycfn.com/gtvokmongf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.hywenlv.cn/gtczuzqnuv.html

[U49] PHP：只读属性
来源：http://hz.pengpengdd.cyou/gtsnwbkmpd.html

public readonly string $name
来源：http://hz.birdmap.top/gtwjtxccef.html

[U50] PHP：构造器属性提升
来源：http://hz.0kj1m.cn/gtpgeyszvc.html

public function __construct(private int $id) {}
来源：http://hz.sxryk.cn/gtacowbkgz.html

[U51] PHP：数组解构
来源：http://hz.bjfxy.top/gtxaysgnlr.html

[$a, $b] = $arr;
来源：http://hz.zhaomingkeji.xyz/gtccrdfqwf.html

[U52] PHP：箭头函数
来源：http://hz.feifeiyinyue.top/gtbjwwsrrf.html

$double = fn($x) => $x * 2;
来源：http://hz.c1oappe.top/gtmnhhauuj.html

[U53] PHP：空合并运算符
来源：http://hz.yvedp.cn/gtjxngpxkf.html

$v = $a ?? $b ?? "default";
来源：http://hz.yuxming.cn/gtyteowujk.html

[U54] PHP：空安全调用
来源：http://hz.ppjwa.cn/gtbgjmvsdg.html

$obj?->method()
来源：http://hz.sysykeji.top/gtepmpfnzn.html

[U55] PHP：match 表达式
来源：http://hz.yuxming.cn/gtnsmsizvz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.sufxvd.cn/gtbhspxbzr.html

[U56] PHP：命名参数
来源：http://hz.jyoumei.cn/gtqbtqgyuz.html

f(a: 1, b: 2)
来源：http://hz.jinyuanbaomall.cn/gtsiobmhib.html

[U57] PHP：字符串插值
来源：http://hz.jqgufenzy.top/gtpxexoeha.html

"值: {$a}"
来源：http://hz.316326.xyz/gtgsinudre.html

[U58] PHP：数组三件套
来源：http://hz.jinqigufen.top/gtxxxaelfm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.gogol.net.cn/gtpkmmyksc.html

[U59] PHP：自定义排序
来源：http://hz.gotoacloud.top/gtiscmmzlg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.chenjidiqi.icu/gtmsotrzya.html

[U60] PHP：JSON 编解码
来源：http://hz.daxiang520.top/gtjxdejdzg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhijiandao.cn/gtegntcebb.html

[U61] PHP：正则
来源：http://hz.zhijiandao.cn/gtmccbesed.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.sufxvd.cn/gthbttwopu.html

[U62] PHP：日期对象
来源：http://hz.yongpay.top/gtvomkdxjc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.meibo888.top/gtqbptboqf.html

[U63] PHP：文件读写
来源：http://hz.dianchejie.cn/gtqqsezwwa.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.ybcxt.top/gtwjbzsrbf.html

[U64] PHP：目录遍历
来源：http://hz.daxiang520.top/gtbgzmazla.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.sysykeji.top/gtddusyrgl.html

[U65] PHP：会话
来源：http://hz.gogol.net.cn/gtwyursnkk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.gaohongyu789.top/gtjwsjjmnc.html

[U66] PHP：设置 Cookie
来源：http://hz.chenzaomai.com/gttxjzypvd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.quarkkingdee.top/gttygbdmqs.html

[U67] PHP：处理文件上传
来源：http://hz.fzhhl.top/gtemtzuifn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.kuanghao11.cn/gtptezpuqy.html

[U68] PHP：PDO 连接
来源：http://hz.dashuyun.cn/gtvukmhpel.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jinqigufen.top/gtiyrjvzml.html

[U69] PHP：PDO 预处理
来源：http://hz.xylfe.cn/gtjlbewfjt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hongshengwenyu.top/gtizafekva.html

[U70] PHP：PDO 事务
来源：http://hz.jqgfzy.top/gtfumcenpv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.mhx1999.top/gtozasxnrj.html

[U71] PHP：抛出异常
来源：http://hz.pengpengdd.cyou/gtmqrtngti.html

throw new RuntimeException("失败", 500);
来源：http://hz.shuidangran.top/gtgvuptgkn.html

[U72] PHP：写错误日志
来源：http://hz.birdmap.top/gtczjvmwzc.html

error_log("失败: " . $e->getMessage());
来源：http://hz.kuanghao11.cn/gtzfnlwkib.html

[U73] PHP：读取 ini 配置
来源：http://hz.ydjk.org.cn/gttmqldiay.html

parse_ini_file("config.ini", true)
来源：http://hz.jyoumei.cn/gtmpyosajk.html

[U74] PHP：读取环境变量
来源：http://hz.gzhubu.top/gtaoqzblhg.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yonumen.top/gtpcygrcef.html

[U75] PHP：依赖注入
来源：http://hz.svipenyu.cn/gtgozbrsny.html

composer require psr/container
来源：http://hz.ywan-chungtsiang.top/gtjgkrhsmb.html

[U76] PHP：简单路由
来源：http://hz.shuidangran.top/gtkwzzqpwl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.sysykeji.top/gtzzhmhxsx.html

[U77] PHP：模板渲染
来源：http://hz.yuanzhike.top/gtrzmbqvti.html

composer require twig/twig
来源：http://hz.xziqi.cn/gttzbnpmlb.html

[U78] PHP：单元测试
来源：http://hz.andypj.xyz/gtzidbxauk.html

composer require --dev phpunit/phpunit
来源：http://hz.xylfe.cn/gtijzttknd.html

[U79] PHP：静态分析
来源：http://hz.meibo888.top/gttonpnmnb.html

composer require --dev phpstan/phpstan
来源：http://hz.guannengcc.top/gtjgpetgff.html

[U80] PHP：代码规范修复
来源：http://hz.xuetiantiany.cn/gtsgoghzqd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.aizwys.cn/gtegupszrg.html

[U81] JS：初始化项目
来源：http://hz.jinqigufen.top/gtpozqudcn.html

npm init -y;  npm i express
来源：http://hz.shanyushiyangkeji.top/gtumzwysoy.html

[U82] JS：package.json 脚本
来源：http://hz.gzhubu.top/gtrabomuzq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.birdmap.top/gtsyrnioka.html

[U83] JS：ES Module 导入导出
来源：http://hz.meibo888.top/gtzscvyood.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yj202588.top/gtmlhgejus.html

[U84] JS：CommonJS 写法
来源：http://hz.yuanzhike.top/gtzbyzlnso.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.ivvv.top/gtnlrhblnj.html

[U85] JS：可选链
来源：http://hz.shanyushiyangtech.top/gtgkttxpxb.html

a?.b?.c
来源：http://hz.snrcjt.cn/gtyagzksvm.html

[U86] JS：空值合并
来源：http://hz.hysaishi.cn/gtwisplghf.html

a ?? b
来源：http://hz.aibaodan.cn/gtwntfjzot.html

[U87] JS：解构默认值
来源：http://hz.chenlongwang.top/gtzlcnbdot.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jinqigufen.top/gtirfzseji.html

[U88] JS：对象展开合并
来源：http://hz.yangfankeji.com/gtglhiodoo.html

{ ...a, ...b }
来源：http://hz.kuanghao11.cn/gtbtzyglcj.html

[U89] JS：数组去重
来源：http://hz.chenjidiqi.icu/gtmtpjzqcp.html

[...new Set(arr)]
来源：http://hz.gotoacloud.top/gtufxamqed.html

[U90] JS：数字数组排序
来源：http://hz.yueranfly.top/gtklocipkz.html

[...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gtfwdbwjcz.html

[U91] JS：对象键值遍历
来源：http://hz.wangdashe.top/gtjcjxtnda.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.aibaodan.cn/gtoogcyauo.html

[U92] JS：深拷贝
来源：http://hz.hysaishi.cn/gtlqyqtkai.html

structuredClone(obj)
来源：http://hz.yongpay.top/gtwdudygui.html

[U93] JS：模板字符串
来源：http://hz.shuidangran.top/gtstyrgoip.html

`共 ${n} 条`
来源：http://hz.yangfankeji.com/gtojxaxzlc.html

[U94] JS：箭头函数
来源：http://hz.ppjwa.cn/gtaqrrhqkg.html

const double = x => x * 2;
来源：http://hz.316326.xyz/gtpqrscvsn.html

[U95] JS：Promise 包装
来源：http://hz.pengpengdd.cyou/gtnzuzxdog.html

new Promise((resolve, reject) => {})
来源：http://hz.havefunace.top/gtnpjnnurw.html

[U96] JS：async/await 与异常
来源：http://hz.zhengqikj.top/gtrkxwsogf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xylfe.cn/gthlbgmmsx.html

[U97] JS：并发请求
来源：http://hz.zdqjudy.top/gtzsikelbe.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ehwqpu.com/gtvnzzyegb.html

[U98] JS：fetch 带 JSON
来源：http://hz.chenlongwang.top/gtzhzuxqyl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hywenlv.cn/gtkkdfeeoo.html

[U99] JS：事件监听
来源：http://hz.tian-w.cn/gtknxluqfn.html

el.addEventListener("click", e => {})
来源：http://hz.zhijiandao.cn/gthwjxltwr.html

[U100] JS：DOM 查询
来源：http://hz.gogol.net.cn/gtwjympsrt.html

document.querySelector(".item")
来源：http://hz.daxiang520.top/gtydmhiage.html

[U101] JS：classList 操作
来源：http://hz.hysaishi.cn/gtdevkiatc.html

el.classList.toggle("active")
来源：http://hz.havefunace.top/gtwjmkjkow.html

[U102] JS：本地存储
来源：http://hz.yueranfly.top/gttqcwzmmg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.shangyingyoupin.top/gthzekngfp.html

[U103] JS：定时器
来源：http://hz.nwbrower.top/gthdoferdl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.nanxuanxn.top/gtyjwszbyr.html

[U104] JS：防抖
来源：http://hz.chenjidiqi.icu/gtwvzkbecr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shuidangran.top/gtkighwvxt.html

[U105] JS：节流
来源：http://hz.pengpengdd.cyou/gtdcqsklwp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.xinyue.icu/gtvuixhggg.html

[U106] JS：日期格式化
来源：http://hz.zhongyouzk.top/gtvywdlaol.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.guowangkeji.top/gtwnmxdwle.html

[U107] JS：数字千分位
来源：http://hz.cdnleiting.top/gtfnmukigw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.tanke756.top/gtjffjxahh.html

[U108] JS：随机整数
来源：http://hz.yj20258888.top/gtkcllglqe.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.bjfxy.top/gtirwfldjq.html

[U109] JS：数组分组
来源：http://hz.xinyue.icu/gtavtzqngn.html

Object.groupBy(arr, x => x.type)
来源：http://hz.nanxuanxn.top/gtjdexfyhd.html

[U110] JS：数组分块
来源：http://hz.mhx1999.top/gtgjwcknov.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.gogol.net.cn/gtclkeniwz.html

[U111] JS：对象转 Map
来源：http://hz.tian-w.cn/gtonhjvxsq.html

new Map(Object.entries(obj))
来源：http://hz.fengsongda.top/gtvlmgbkko.html

[U112] JS：字符串补位
来源：http://hz.jinqigfzy.top/gtwuwslrmk.html

"7".padStart(3, "0")
来源：http://hz.jinqigufen.top/gtwwainurr.html

[U113] JS：正则替换全部
来源：http://hz.xinyue.icu/gtjwmzazha.html

s.replaceAll("a", "b")
来源：http://hz.vqdsnc.cn/gtqzobltsh.html

[U114] JS：JSON 深比较
来源：http://hz.fengsongda.top/gtcoqupluo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenjidiqi.icu/gtvmwwexac.html

[U115] JS：生成 UUID
来源：http://hz.sysykeji.top/gtcggxdaig.html

crypto.randomUUID()
来源：http://hz.aizwys.cn/gtzegiowpy.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hammf.cn/gtjaogufux.html

/** @param {string} name */ function f(name) {}
来源：http://hz.chenzaomai.com/gtajozwzdw.html

[U117] JS：单元测试
来源：http://hz.9152youxi.cn/gtjafejcsc.html

npm i -D vitest;  npx vitest
来源：http://hz.9152youxi.cn/gtnxggqihl.html

[U118] JS：开发服务器
来源：http://hz.cucudq.cn/gtcuotpozp.html

npm i -D vite;  npx vite
来源：http://hz.ivvv.top/gtbqvwffzx.html

[U119] JS：生产构建
来源：http://hz.jinqigufen.top/gtyxoyouws.html

npx vite build
来源：http://hz.ivvv.top/gtwlwpkqqn.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yuanzhike.top/gtvskflwim.html

import.meta.env.VITE_API_URL
来源：http://hz.zhiwuduotai.top/gtagczgvta.html

================================================================================
来源：http://hz.wangdashe.top/gtcswywrzm.html

统计汇总
来源：http://hz.ydzc1.top/gtujmcxtxf.html

================================================================================
来源：http://hz.jqgufenzy.top/gttscxpnpu.html

按语言统计（条）：
来源：http://hz.andypj.xyz/gtkhmslknk.html

Python ......... 252
来源：http://hz.mhx1999.top/gtajzjsgyq.html

PHP ............ 252
来源：http://hz.xuanzx.com/gttmzrvber.html

JavaScript ..... 252
来源：http://hz.shangyingyoupin.top/gtvvvuipge.html

TypeScript ..... 212
来源：http://hz.pycfn.com/gtqasmmxyr.html

Java ........... 212
来源：http://hz.zhongyouzk.top/gtxmpcqzgq.html

Go ............. 212
来源：http://hz.tianlin.xyz/gtjthfufuf.html

Ruby ........... 212
来源：http://hz.zhijiandao.cn/gtcdmfgvju.html

C# ............. 212
来源：http://hz.shzxlz.cn/gtozfnwmui.html

C .............. 30
来源：http://hz.tanke756.top/gthpdnhwjf.html

C++ ............ 30
来源：http://hz.feifeiyinyue.top/gtorkrahxz.html

SQL ............ 90
来源：http://hz.tianlin.xyz/gtikpozznd.html

Bash ........... 80
来源：http://hz.gotoacloud.top/gtcetxkowj.html

Kotlin ......... 15
来源：http://hz.xuetiantiany.cn/gtpukudyyf.html

Swift .......... 15
来源：http://hz.yangfankeji.com/gtebrdlhne.html

Lua ............ 10
来源：http://hz.jlsjyb.cn/gtcvqhspcb.html

Perl ........... 10
来源：http://hz.zhaomingkeji.xyz/gtvebisnmw.html

Scala .......... 10
来源：http://hz.ehwqpu.com/gttpplwdyv.html

------------------------------------
来源：http://hz.yueranfly.top/gtdwwxttxs.html

合计 ........... 2106 条
来源：http://hz.shanyushiyangkeji.top/gtlkipukcr.html

按章节统计：
来源：http://hz.xylfe.cn/gttvglbzmq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jqgufenzy.top/gthmvqafkw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.aizwys.cn/gtatcqrhvn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zycfv.cn/gttxsarwiv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zhaomingkeji.xyz/gtslxdlrap.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.ivvv.top/gtjjcjrrit.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yuxming.cn/gtttuetyts.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.gogol.net.cn/gtruxqcfpi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhixingplan.top/gtjktdhqng.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.chenzaomai.com/gtszpwwsxr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.svipenyu.cn/gtdiruowlh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jinghuilouyu.cn/gtbkasbwnn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jinghuilouyu.cn/gthlnszcal.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.dianchejie.cn/gtpfjvyqmw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yangfankeji.com/gtvmgrixch.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yonumen.top/gtgmqvhhpq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.cheryme.top/gtzximbhjc.html

Q SQL 专题                              90
来源：http://hz.gzhubu.top/gtjlugawzd.html

R Bash 专题                             80
来源：http://hz.cashguo.top/gtsjixeoxi.html

S C / C++ 专题                          60
来源：http://hz.jinqigufen.top/gtqdolyosa.html

T 其他语言补充                          60
来源：http://hz.jiagoushi.top/gtsfuivrjy.html

U 高频实用片段                         120
来源：http://hz.jiagoushi.top/gtusytaxgq.html

------------------------------------
来源：http://hz.xinyue.icu/gtficllojk.html

合计                                  2106 条
来源：http://hz.ydzc1.top/gtuodlwzpx.html

--------------------------------------------------------------------------------
来源：http://hz.zhiwuduotai.top/gtxvkzegds.html

使用提醒
来源：http://hz.wangdashe.top/gtcgsoqhsr.html

--------------------------------------------------------------------------------
来源：http://hz.xuanzx.com/gtrtadjkmg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.bjfxy.top/gtrqmrdzvs.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yonumen.top/gtjcbklqiy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zycfv.cn/gtqonsgpov.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.sxryk.cn/gtdlhiafvq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.aizwys.cn/gtejaqciit.html

—— 文件结束 ——
来源：http://hz.nanxinkj.top/gtvczlyuxt.html

================================================================================
来源：http://hz.yj20258888.top/gtxltzxvnk.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.fzhhl.top/gtmwpyjrdf.html

Common Programming Examples Cheat Book
来源：http://hz.yvedp.cn/gtojmzzhag.html

================================================================================
来源：http://hz.gaohongyu789.top/gtothjdouo.html

【收录内容】
来源：http://hz.nanxinkj.top/gteqcmvrgq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zycfv.cn/gtzsuqkcbv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jiagoushi.top/gtgelqgqyz.html

SQL · Bash · C · C++
来源：http://hz.dianchejie.cn/gtbapbvnka.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.shangyingyoupin.top/gtxjzithwy.html

【使用说明】
来源：http://hz.aizwys.cn/gtjopbedov.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.shanyushiyangkeji.top/gtckypzqty.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.nwbrower.top/gtqjogjpwl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.shangyingyoupin.top/gtmwpwltnb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.wangdashe.top/gtcusfsbmt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.guowangkeji.top/gtjqjlyxcz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.shangyingyoupin.top/gtqytwowpz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.zhoulong.xyz/gtotibihih.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.cheryme.top/gtpzocbipe.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.zhengqikj.top/gttgrnupqg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.andypj.xyz/gtekttfmvg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.havefunace.top/gtdlkqdcly.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.pycfn.com/gtwlalcntk.html

【文件统计】
来源：http://hz.xinyue.icu/gtdjvwhvvu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yangfankeji.com/gtnrynbysk.html

--------------------------------------------------------------------------------
来源：http://hz.tanke756.top/gtlrrgmwyz.html

目  录
来源：http://hz.xuanzx.com/gtdyzjuqvj.html

--------------------------------------------------------------------------------
来源：http://hz.jinghuilouyu.cn/gtulatzxmn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.pycfn.com/gtbsyfatkl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.ydzc1.top/gtzxhtnkib.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.sxryk.cn/gtshypyqaw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.52xcode.cn/gtutzpiclb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yongpay.top/gtfnbhtfuw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.pycfn.com/gtfgesbvfy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.hywenlv.cn/gtkogswgda.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zhijiandao.cn/gtjhmedstu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.wangshuangyany.cn/gtvxyfzfwo.html


<!-- 参考信息 -->