代发 wailian999

[U13] Py：固定长度队列
来源：http://hz.zhiwuduotai.top/gttggatpua.html

deque(maxlen=10)
来源：http://hz.c1oappe.top/gtpbrceacq.html

[U14] Py：分组收集到列表
来源：http://hz.ppjwa.cn/gtxopmcfzg.html

defaultdict(list)
来源：http://hz.gotoacloud.top/gtmekvxaqm.html

[U15] Py：高精度计时
来源：http://hz.pengpengdd.cyou/gtoktomerv.html

t = time.perf_counter()
来源：http://hz.fengsongda.top/gtyjeouelt.html

[U16] Py：命令行参数解析
来源：http://hz.zhixingplan.top/gtwbvrwjkn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.52xcode.cn/gtiommwzxz.html

[U17] Py：初始化日志
来源：http://hz.daxiang520.top/gtcutlrkul.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yj20258888.top/gtuyreddid.html

[U18] Py：预编译正则
来源：http://hz.zycfv.cn/gtxnkyyhuw.html

pat = re.compile(r"\d+")
来源：http://hz.hfpthk.cn/gtuxvvussq.html

[U19] Py：正则替换带回调
来源：http://hz.yongpay.top/gtezmdooll.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yueranfly.top/gtxjuxdubc.html

[U20] Py：缓存函数结果
来源：http://hz.daxiang520.top/gtmmikesbl.html

@functools.lru_cache(maxsize=None)
来源：http://hz.ppjwa.cn/gtrnmrrfis.html

[U21] Py：自定义上下文管理器
来源：http://hz.yj20258.top/gtksnafqok.html

@contextlib.contextmanager
来源：http://hz.hammf.cn/gtpccqewkp.html

[U22] Py：矩阵转置
来源：http://hz.tian-w.cn/gtzwjinnux.html

list(zip(*m))
来源：http://hz.haohaochexian.top/gtfgxqoulh.html

[U23] Py：分块读取大文件
来源：http://hz.shanyushiyangkeji.top/gtikjepgff.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yangfankeji.com/gtpuxlriph.html

[U24] Py：路径操作
来源：http://hz.pengpengdd.cyou/gtqjcugwty.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.cashguo.top/gtwgqspbkg.html

[U25] Py：CSV 按字典读
来源：http://hz.chenjidiqi.icu/gtavqpetkn.html

csv.DictReader(f)
来源：http://hz.gzhubu.top/gtjbrevyiv.html

[U26] Py：并发下载
来源：http://hz.bjfxy.top/gtsecpncab.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhijiandao.cn/gtypcopnja.html

[U27] Py：异步 HTTP
来源：http://hz.gogol.net.cn/gtrkgvcgqa.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jinqigufen.top/gtthxkgvag.html

[U28] Py：类型别名
来源：http://hz.shuidangran.top/gtudfhovwb.html

UserId = int
来源：http://hz.zhaomingkeji.xyz/gtpkjxzlot.html

[U29] Py：属性校验
来源：http://hz.316326.xyz/gtjbiimzar.html

@property 与 @x.setter 配合
来源：http://hz.mhx1999.top/gtlrnnxayw.html

[U30] Py：数据类
来源：http://hz.sufxvd.cn/gtubsfyjny.html

@dataclass(slots=True)
来源：http://hz.hywenlv.cn/gtcvzbhfjl.html

[U31] Py：单测
来源：http://hz.meibo888.top/gtqyvhffsy.html

python -m pytest -q
来源：http://hz.vqdsnc.cn/gtqpdvywuu.html

[U32] Py：代码格式化
来源：http://hz.cheryme.top/gteauwgbse.html

ruff format . && ruff check --fix .
来源：http://hz.pengpengdd.cyou/gtlfiozjam.html

[U33] Py：打包发布
来源：http://hz.9152youxi.cn/gtsbirniab.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.snrcjt.cn/gtrbmcaqrq.html

[U34] Py：判断编码
来源：http://hz.jianghu66.top/gtbyaojvyf.html

chardet.detect(raw)
来源：http://hz.sufxvd.cn/gtpvgnbvwb.html

[U35] Py：发送邮件
来源：http://hz.zhaomingkeji.xyz/gtcffusyvq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.shangyingyoupin.top/gtbgllidmm.html

[U36] Py：定时任务
来源：http://hz.aizwys.cn/gtkihoaxww.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhiwuduotai.top/gtizscgnxs.html

[U37] Py：读写 Excel
来源：http://hz.sweek.top/gtzqnmwujs.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xuetiantiany.cn/gttiywtrss.html

[U38] Py：获取脚本所在目录
来源：http://hz.xuanzx.com/gtaymjzbcz.html

Path(__file__).resolve().parent
来源：http://hz.0kj1m.cn/gtrqzakfvh.html

[U39] Py：判断是否在交互环境
来源：http://hz.pycfn.com/gtcvpvblil.html

sys.stdout.isatty()
来源：http://hz.ydjk.org.cn/gtfmcirvdv.html

[U40] Py：打印到标准错误
来源：http://hz.shanyushiyangtech.top/gtbovaxdii.html

print("err", file=sys.stderr)
来源：http://hz.xuanzx.com/gtcgraorfk.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.havefunace.top/gtlvkptmpa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jqgufenzy.top/gtckczmham.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.meibo888.top/gttdmnfstp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.pengpengdd.cyou/gtjhgjkqaa.html

[U43] PHP：声明命名空间
来源：http://hz.jlsjyb.cn/gtccwoqacp.html

namespace App\Http;
来源：http://hz.birdmap.top/gtgaungfdp.html

[U44] PHP：开启严格类型
来源：http://hz.9152youxi.cn/gtqsisraem.html

declare(strict_types=1);
来源：http://hz.chenjidiqi.icu/gtwhwnwout.html

[U45] PHP：类型声明与返回类型
来源：http://hz.daxiang520.top/gtwvosqasm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cqqwz.cn/gtlbqybsha.html

[U46] PHP：可空类型
来源：http://hz.nanxinkj.top/gtunnlzutu.html

?string $name = null
来源：http://hz.ivvv.top/gtbxyfbmao.html

[U47] PHP：联合类型
来源：http://hz.vqdsnc.cn/gtlxhsqwos.html

int|string $id
来源：http://hz.tian-w.cn/gtitjkfihj.html

[U48] PHP：纯枚举
来源：http://hz.cqqwz.cn/gtolcwhohd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.shangyingyoupin.top/gtaxmarcjb.html

[U49] PHP：只读属性
来源：http://hz.yangfankeji.com/gtxpujspjs.html

public readonly string $name
来源：http://hz.pycfn.com/gteriiaawf.html

[U50] PHP：构造器属性提升
来源：http://hz.shzxlz.cn/gtqealtheu.html

public function __construct(private int $id) {}
来源：http://hz.smart0.xyz/gtihgpatim.html

[U51] PHP：数组解构
来源：http://hz.fzhhl.top/gttkhunrzf.html

[$a, $b] = $arr;
来源：http://hz.birdmap.top/gtxjipxvao.html

[U52] PHP：箭头函数
来源：http://hz.gogol.net.cn/gtmhtllibk.html

$double = fn($x) => $x * 2;
来源：http://hz.iojbl.cn/gtomuggitr.html

[U53] PHP：空合并运算符
来源：http://hz.jinghuilouyu.cn/gtplclibzr.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhongyouzk.top/gtzwbnkuuq.html

[U54] PHP：空安全调用
来源：http://hz.jinyuanbaomall.cn/gtvopqfvrw.html

$obj?->method()
来源：http://hz.ppjwa.cn/gtwkgfkltb.html

[U55] PHP：match 表达式
来源：http://hz.birdmap.top/gtglmkquhd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhengqikj.top/gtlfutijch.html

[U56] PHP：命名参数
来源：http://hz.shuidangran.top/gthrdsnepd.html

f(a: 1, b: 2)
来源：http://hz.gotoacloud.top/gtxjvxljij.html

[U57] PHP：字符串插值
来源：http://hz.birdmap.top/gtkgptasfa.html

"值: {$a}"
来源：http://hz.hnxiangtu.top/gtnzgkzspc.html

[U58] PHP：数组三件套
来源：http://hz.yj20258.top/gtxpyvwfns.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jiagoushi.top/gtokzavzgg.html

[U59] PHP：自定义排序
来源：http://hz.zhiwuduotai.top/gtnhepfksj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuanzhike.top/gtlhmycurs.html

[U60] PHP：JSON 编解码
来源：http://hz.hnxiangtu.top/gtkisladaf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.guannengcc.top/gtrwmryhop.html

[U61] PHP：正则
来源：http://hz.sysykeji.top/gtskxkwatz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.pengpengdd.cyou/gtlrfwxhgd.html

[U62] PHP：日期对象
来源：http://hz.zycfv.cn/gtkgwhmbdk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.pycfn.com/gtdlaiyuxm.html

[U63] PHP：文件读写
来源：http://hz.hfpthk.cn/gtqafrywlo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.gogol.net.cn/gtwisjokly.html

[U64] PHP：目录遍历
来源：http://hz.sxryk.cn/gtfsbyjfjn.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.0kj1m.cn/gtedljrkgf.html

[U65] PHP：会话
来源：http://hz.xingfuxueyuan.xyz/gtwlcvptjv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.dashuyun.cn/gtweyafkgi.html

[U66] PHP：设置 Cookie
来源：http://hz.pycfn.com/gtunijpred.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.gzhubu.top/gtpqehbthz.html

[U67] PHP：处理文件上传
来源：http://hz.ppjwa.cn/gtznhgdzzh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jlsjyb.cn/gttkxejjfu.html

[U68] PHP：PDO 连接
来源：http://hz.ydjk.org.cn/gtitprkmsi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.mhx1999.top/gtcurfhozm.html

[U69] PHP：PDO 预处理
来源：http://hz.shanyushiyangtech.top/gtuufiawed.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jlsjyb.cn/gtlajlddzr.html

[U70] PHP：PDO 事务
来源：http://hz.gotoacloud.top/gtdyxszteh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.cqqwz.cn/gtujohnvvr.html

[U71] PHP：抛出异常
来源：http://hz.tian-w.cn/gtxtemwloc.html

throw new RuntimeException("失败", 500);
来源：http://hz.gogol.net.cn/gtyjlhfgoe.html

[U72] PHP：写错误日志
来源：http://hz.cdnleiting.top/gtcpfkhway.html

error_log("失败: " . $e->getMessage());
来源：http://hz.daxiang520.top/gtqulegimy.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhixingplan.top/gttznhgoco.html

parse_ini_file("config.ini", true)
来源：http://hz.sysykeji.top/gtyckuijuc.html

[U74] PHP：读取环境变量
来源：http://hz.jqgufenzy.top/gthcjeexnn.html

getenv("APP_ENV") ?: "production"
来源：http://hz.daria6918.cn/gtiqfancrc.html

[U75] PHP：依赖注入
来源：http://hz.jinyuanbaomall.cn/gtlrzwbutu.html

composer require psr/container
来源：http://hz.jinqigufen.top/gtiehkkqeg.html

[U76] PHP：简单路由
来源：http://hz.cashguo.top/gtkrlxeurz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zhengqikj.top/gtmxzzjfzs.html

[U77] PHP：模板渲染
来源：http://hz.daxiang520.top/gtuojvrcqr.html

composer require twig/twig
来源：http://hz.nanxuanxn.top/gtfdmvehzb.html

[U78] PHP：单元测试
来源：http://hz.jinghuilouyu.cn/gtpndofxjg.html

composer require --dev phpunit/phpunit
来源：http://hz.shanyushiyangkeji.top/gtrebdjwce.html

[U79] PHP：静态分析
来源：http://hz.gzhubu.top/gtouqfpkyb.html

composer require --dev phpstan/phpstan
来源：http://hz.aibaodan.cn/gtmpshrzei.html

[U80] PHP：代码规范修复
来源：http://hz.sweek.top/gtnprotcqm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhijiandao.cn/gtgztliuod.html

[U81] JS：初始化项目
来源：http://hz.aibaodan.cn/gtcmqsfvvy.html

npm init -y;  npm i express
来源：http://hz.kuanghao11.cn/gtpglrkcyh.html

[U82] JS：package.json 脚本
来源：http://hz.hongshengwenyu.top/gtodmeexhc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.chenzaomai.com/gtmivgeieq.html

[U83] JS：ES Module 导入导出
来源：http://hz.jinghuilouyu.cn/gtpslhrcms.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.0kj1m.cn/gtnevuykdh.html

[U84] JS：CommonJS 写法
来源：http://hz.shanyushiyangtech.top/gtizoweuxi.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.ydjk.org.cn/gtrloinmhk.html

[U85] JS：可选链
来源：http://hz.yangfankeji.com/gtspdnhelv.html

a?.b?.c
来源：http://hz.shanyushiyangtech.top/gtrllcciez.html

[U86] JS：空值合并
来源：http://hz.xuanzx.com/gtvboqmonw.html

a ?? b
来源：http://hz.ybcxt.top/gtouavcojb.html

[U87] JS：解构默认值
来源：http://hz.chenlongwang.top/gtkdmjgvie.html

const { a = 1, b = 2 } = obj;
来源：http://hz.shanyushiyangkeji.top/gtlvxqupuf.html

[U88] JS：对象展开合并
来源：http://hz.jinghuilouyu.cn/gtbfoupvqc.html

{ ...a, ...b }
来源：http://hz.c1oappe.top/gtqctydjfm.html

[U89] JS：数组去重
来源：http://hz.yvedp.cn/gtrkndglsx.html

[...new Set(arr)]
来源：http://hz.yongpay.top/gtvbadsqtl.html

[U90] JS：数字数组排序
来源：http://hz.iojbl.cn/gttcqxsddo.html

[...arr].sort((a, b) => a - b)
来源：http://hz.smart0.xyz/gtlnpermqj.html

[U91] JS：对象键值遍历
来源：http://hz.yj202588.top/gtkrlspaio.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.pengpengdd.cyou/gtiphayjsr.html

[U92] JS：深拷贝
来源：http://hz.zhixingplan.top/gtkqzmahah.html

structuredClone(obj)
来源：http://hz.zhiwuduotai.top/gtlccndqlw.html

[U93] JS：模板字符串
来源：http://hz.zhengqikj.top/gtfuhlhcza.html

`共 ${n} 条`
来源：http://hz.tianlin.xyz/gtybdlovjo.html

[U94] JS：箭头函数
来源：http://hz.xziqi.cn/gtwwjhtdhc.html

const double = x => x * 2;
来源：http://hz.hongshengwenyu.top/gtpyfqvyca.html

[U95] JS：Promise 包装
来源：http://hz.shangyingyoupin.top/gtbxejtxfm.html

new Promise((resolve, reject) => {})
来源：http://hz.yj20258888.top/gtqgtnoshs.html

[U96] JS：async/await 与异常
来源：http://hz.tanke756.top/gtcjoeaken.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.mhx1999.top/gtfkwgsyws.html

[U97] JS：并发请求
来源：http://hz.yongpay.top/gtvyrbpsjg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gtnqwtmevf.html

[U98] JS：fetch 带 JSON
来源：http://hz.gogol.net.cn/gtpjyzrmfl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yueranfly.top/gthgwybbgl.html

[U99] JS：事件监听
来源：http://hz.c1oappe.top/gtbublmhyu.html

el.addEventListener("click", e => {})
来源：http://hz.nanxuanxn.top/gtlecpnowm.html

[U100] JS：DOM 查询
来源：http://hz.hywenlv.cn/gtvekaxagy.html

document.querySelector(".item")
来源：http://hz.ivvv.top/gtmuiyjdmh.html

[U101] JS：classList 操作
来源：http://hz.sufxvd.cn/gtjsbwxomu.html

el.classList.toggle("active")
来源：http://hz.yangfankeji.com/gtlmsjdxfu.html

[U102] JS：本地存储
来源：http://hz.sweek.top/gtolefemce.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.hnqzz.top/gtwqmumbmz.html

[U103] JS：定时器
来源：http://hz.daxiang520.top/gtcpyvaudg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zycfv.cn/gtrprenjhv.html

[U104] JS：防抖
来源：http://hz.cucudq.cn/gtilvwckhj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.9152youxi.cn/gtxqkadnbk.html

[U105] JS：节流
来源：http://hz.zhixingplan.top/gtdoloxqtj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.shuidangran.top/gtlgnepvls.html

[U106] JS：日期格式化
来源：http://hz.havefunace.top/gtwqkzrhfx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ydzc1.top/gtqlvovsre.html

[U107] JS：数字千分位
来源：http://hz.daxiang520.top/gtqqxggvcu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yuxming.cn/gtgblwewox.html

[U108] JS：随机整数
来源：http://hz.sweek.top/gtghrozsaw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.wangdashe.top/gtxfwgackm.html

[U109] JS：数组分组
来源：http://hz.redwolf501.top/gtnrmkcuyq.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yuxming.cn/gtocdeclgt.html

[U110] JS：数组分块
来源：http://hz.fzhhl.top/gtezakvbvx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.gotoacloud.top/gteripsdzj.html

[U111] JS：对象转 Map
来源：http://hz.chenjidiqi.icu/gtyfswjojq.html

new Map(Object.entries(obj))
来源：http://hz.shangyingyoupin.top/gtvgsopizw.html

[U112] JS：字符串补位
来源：http://hz.zhoulong.xyz/gtgjmywydy.html

"7".padStart(3, "0")
来源：http://hz.sysykeji.top/gtfnbjvlaz.html

[U113] JS：正则替换全部
来源：http://hz.chenzaomai.com/gtqttrhfsi.html

s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gtustadkre.html

[U114] JS：JSON 深比较
来源：http://hz.iojbl.cn/gtrjansbht.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.pycfn.com/gtpczyutlw.html

[U115] JS：生成 UUID
来源：http://hz.aizwys.cn/gtuzbxlapt.html

crypto.randomUUID()
来源：http://hz.dashuyun.cn/gtwnfrzsqz.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.chenjidiqi.icu/gtjxxodvbc.html

/** @param {string} name */ function f(name) {}
来源：http://hz.xziqi.cn/gtmnibmwng.html

[U117] JS：单元测试
来源：http://hz.vqdsnc.cn/gtrunbgzct.html

npm i -D vitest;  npx vitest
来源：http://hz.zdqjudy.top/gtwtwakkaj.html

[U118] JS：开发服务器
来源：http://hz.nwbrower.top/gtkhjdssjd.html

npm i -D vite;  npx vite
来源：http://hz.nanxuanxn.top/gtzeguictr.html

[U119] JS：生产构建
来源：http://hz.c1oappe.top/gtowkqiyjj.html

npx vite build
来源：http://hz.zhongyouzk.top/gtfnrgorbr.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.guowangkeji.top/gtlfgiatvt.html

import.meta.env.VITE_API_URL
来源：http://hz.zhiwuduotai.top/gtvwcgtkoy.html

================================================================================
来源：http://hz.kuanghao11.cn/gtibugwlhl.html

统计汇总
来源：http://hz.yangfankeji.com/gtsclsxfwy.html

================================================================================
来源：http://hz.jyoumei.cn/gtqepyubse.html

按语言统计（条）：
来源：http://hz.hnxiangtu.top/gtgjvhxtos.html

Python ......... 252
来源：http://hz.hnqzz.top/gtmvkxsbud.html

PHP ............ 252
来源：http://hz.chenzaomai.com/gtvwmqgbww.html

JavaScript ..... 252
来源：http://hz.yonumen.top/gtmfxkmqdp.html

TypeScript ..... 212
来源：http://hz.kuanghao11.cn/gtklugixbm.html

Java ........... 212
来源：http://hz.ehwqpu.com/gtlvrnmzjn.html

Go ............. 212
来源：http://hz.aibaodan.cn/gtxrfqzpqv.html

Ruby ........... 212
来源：http://hz.jqgufenzy.top/gtjiszaqcg.html

C# ............. 212
来源：http://hz.zhixingplan.top/gtsqoiasxn.html

C .............. 30
来源：http://hz.dashuyun.cn/gtpqtdqnwa.html

C++ ............ 30
来源：http://hz.cashguo.top/gtgvzwvgsj.html

SQL ............ 90
来源：http://hz.jqgfzy.top/gtpautfjal.html

Bash ........... 80
来源：http://hz.xylfe.cn/gtsgzwueyt.html

Kotlin ......... 15
来源：http://hz.havefunace.top/gtaocyrlrf.html

Swift .......... 15
来源：http://hz.daria6918.cn/gtmakyhtgx.html

Lua ............ 10
来源：http://hz.fzhhl.top/gtbseovcwn.html

Perl ........... 10
来源：http://hz.316326.xyz/gtekrljcrw.html

Scala .......... 10
来源：http://hz.fengsongda.top/gtbgbkkdti.html

------------------------------------
来源：http://hz.haohaochexian.top/gtoxuvgugg.html

合计 ........... 2106 条
来源：http://hz.yuanzhike.top/gtjbqqktvn.html

按章节统计：
来源：http://hz.nanxuanxn.top/gtpcqimpqw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.haohaochexian.top/gtsytqwvkd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhijiandao.cn/gtjbigujqv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yj20258888.top/gtpqyggpof.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hammf.cn/gtrslbuszd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.vqdsnc.cn/gtzemhifww.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.xuanzx.com/gtonqarkpq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.iojbl.cn/gttkwqyymt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.cucudq.cn/gtbkwsvnvo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zhaomingkeji.xyz/gtquqlgepp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.shanyushiyangkeji.top/gtnlzgooqd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.vqdsnc.cn/gthkqnjhca.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.tian-w.cn/gtjjsdwxct.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gtmuietbov.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.chenzaomai.com/gtnlambzur.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jiagoushi.top/gtngqfbhfd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yvedp.cn/gtcgwtsdbs.html

Q SQL 专题                              90
来源：http://hz.dianchejie.cn/gthchhnxou.html

R Bash 专题                             80
来源：http://hz.guowangkeji.top/gtahylnbjz.html

S C / C++ 专题                          60
来源：http://hz.daria6918.cn/gtqjjvqdkj.html

T 其他语言补充                          60
来源：http://hz.yj20258.top/gtedfbmcvh.html

U 高频实用片段                         120
来源：http://hz.hfpthk.cn/gtuznogsae.html

------------------------------------
来源：http://hz.jyoumei.cn/gtfiqijshq.html

合计                                  2106 条
来源：http://hz.jqgufenzy.top/gtlhvjcoxo.html

--------------------------------------------------------------------------------
来源：http://hz.hnxiangtu.top/gtndcujoku.html

使用提醒
来源：http://hz.tianlin.xyz/gtcwgxbfhg.html

--------------------------------------------------------------------------------
来源：http://hz.havefunace.top/gtwmxwulkk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.guannengcc.top/gtllxideui.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.pycfn.com/gtlztiwdrd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.wangdashe.top/gtthlkhdbj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.c1oappe.top/gtneafposj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.mhx1999.top/gtyzmbfdtv.html

—— 文件结束 ——
来源：http://hz.shuidangran.top/gtyuwzrclm.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtehhugeha.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.guannengcc.top/gtvmyktvvc.html

Common Programming Examples Cheat Book
来源：http://hz.zhiwuduotai.top/gtxbukkgxy.html

================================================================================
来源：http://hz.jqgufenzy.top/gtzsiclqne.html

【收录内容】
来源：http://hz.redwolf501.top/gtlklgidiw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.c1oappe.top/gtcurwugwb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhixingplan.top/gtheyykzer.html

SQL · Bash · C · C++
来源：http://hz.daxiang520.top/gtoqibuenn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.0kj1m.cn/gtkokcbhwc.html

【使用说明】
来源：http://hz.dianchejie.cn/gtfkrfhipf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yuxming.cn/gtduazuvkw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.cashguo.top/gthutmkzbg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.shangyingyoupin.top/gtdhnbshyx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.ivvv.top/gtcymwkmqt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jqgufenzy.top/gtwwhifhms.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.aibaodan.cn/gtxdshtnlu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.gogol.net.cn/gteyvkghbo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.shanyushiyangkeji.top/gtduogweht.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.ydzc1.top/gtthmtmrhx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.wangdashe.top/gtfslubpdx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jinqigufen.top/gtbofsgwah.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yangfankeji.com/gtywzovtbr.html

【文件统计】
来源：http://hz.cqqwz.cn/gtsbwlivcr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.52xcode.cn/gtbexgfrqq.html

--------------------------------------------------------------------------------
来源：http://hz.ydzc1.top/gtonyvozgk.html

目  录
来源：http://hz.hysaishi.cn/gtuvtlswdv.html

--------------------------------------------------------------------------------
来源：http://hz.yanxiufei.cn/gtlvkcnpqs.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.svipenyu.cn/gtukdtoprn.html


<!-- 参考信息 -->