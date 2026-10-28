代发 wailian999

[U11] Py：生成器表达式
来源：http://hz.ehwqpu.com/gtmspnfrsb.html

(x * 2 for x in arr)
来源：http://hz.xingfuxueyuan.xyz/gtxkflplem.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.sxryk.cn/gtqjuxjpzv.html

Counter(arr).most_common(3)
来源：http://hz.daria6918.cn/gtwhhiazgr.html

[U13] Py：固定长度队列
来源：http://hz.quarkkingdee.top/gtthmrhkzs.html

deque(maxlen=10)
来源：http://hz.yuanzhike.top/gtkfcmnsjr.html

[U14] Py：分组收集到列表
来源：http://hz.shangyingyoupin.top/gtxinpwjle.html

defaultdict(list)
来源：http://hz.haohaochexian.top/gtwfzycmwu.html

[U15] Py：高精度计时
来源：http://hz.guannengcc.top/gtopnwtqgd.html

t = time.perf_counter()
来源：http://hz.aibaodan.cn/gtfbnlgiqs.html

[U16] Py：命令行参数解析
来源：http://hz.shanyushiyangtech.top/gtjhvhfsod.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.chenlongwang.top/gtrtphjhdl.html

[U17] Py：初始化日志
来源：http://hz.jianghu66.top/gtizzfchme.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.xziqi.cn/gtizugifzd.html

[U18] Py：预编译正则
来源：http://hz.nanxinkj.top/gtyjkuwmfi.html

pat = re.compile(r"\d+")
来源：http://hz.jianghu66.top/gtaemddrtx.html

[U19] Py：正则替换带回调
来源：http://hz.yonumen.top/gtcigkbobh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhiwuduotai.top/gtwrissjwl.html

[U20] Py：缓存函数结果
来源：http://hz.cqqwz.cn/gtwmwrwean.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yonumen.top/gtjrhyekyo.html

[U21] Py：自定义上下文管理器
来源：http://hz.xuetiantiany.cn/gtbarokylj.html

@contextlib.contextmanager
来源：http://hz.jyoumei.cn/gtxwzsrhkb.html

[U22] Py：矩阵转置
来源：http://hz.52xcode.cn/gtvvqrmpji.html

list(zip(*m))
来源：http://hz.zycfv.cn/gtgaevbecp.html

[U23] Py：分块读取大文件
来源：http://hz.hywenlv.cn/gtkmnytvrj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ybcxt.top/gtkhobnvqw.html

[U24] Py：路径操作
来源：http://hz.zycfv.cn/gtfligirzb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.daria6918.cn/gtckvkirpb.html

[U25] Py：CSV 按字典读
来源：http://hz.hammf.cn/gtefvvngvu.html

csv.DictReader(f)
来源：http://hz.fzhhl.top/gtcxlbiksp.html

[U26] Py：并发下载
来源：http://hz.quarkkingdee.top/gtivuljweq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.nwbrower.top/gtblcvnyov.html

[U27] Py：异步 HTTP
来源：http://hz.aibaodan.cn/gtsnxekclk.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ivvv.top/gtetqvphey.html

[U28] Py：类型别名
来源：http://hz.haohaochexian.top/gtrmmpwwnk.html

UserId = int
来源：http://hz.cheryme.top/gtxyvkdegy.html

[U29] Py：属性校验
来源：http://hz.cucudq.cn/gthbuvhwfs.html

@property 与 @x.setter 配合
来源：http://hz.zhongyouzk.top/gtqsebmetm.html

[U30] Py：数据类
来源：http://hz.9152youxi.cn/gtfihfgvcq.html

@dataclass(slots=True)
来源：http://hz.zhongyouzk.top/gtxdlsepac.html

[U31] Py：单测
来源：http://hz.xinyue.icu/gtzgjcpgtr.html

python -m pytest -q
来源：http://hz.shzxlz.cn/gttchnihyf.html

[U32] Py：代码格式化
来源：http://hz.hnxiangtu.top/gtxsfodwgl.html

ruff format . && ruff check --fix .
来源：http://hz.yj20258.top/gtphdnwoue.html

[U33] Py：打包发布
来源：http://hz.meibo888.top/gtldltwryp.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.gaohongyu789.top/gtgfkijqsp.html

[U34] Py：判断编码
来源：http://hz.jinqigfzy.top/gtzxsfsjmh.html

chardet.detect(raw)
来源：http://hz.fengsongda.top/gtbktakmud.html

[U35] Py：发送邮件
来源：http://hz.hysaishi.cn/gtanqdffbw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.wangdashe.top/gtwpdwsygt.html

[U36] Py：定时任务
来源：http://hz.chenzaomai.com/gtzulihttc.html

schedule.every(10).minutes.do(job)
来源：http://hz.iojbl.cn/gtzpxgrfdy.html

[U37] Py：读写 Excel
来源：http://hz.ydzc1.top/gtcsbwucln.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.daxiang520.top/gtjmfnwvfk.html

[U38] Py：获取脚本所在目录
来源：http://hz.zdqjudy.top/gtqybsbwfu.html

Path(__file__).resolve().parent
来源：http://hz.yonumen.top/gteidyqeox.html

[U39] Py：判断是否在交互环境
来源：http://hz.yvedp.cn/gtkodhzcnc.html

sys.stdout.isatty()
来源：http://hz.zycfv.cn/gtvpvmsyul.html

[U40] Py：打印到标准错误
来源：http://hz.nwbrower.top/gttyjjcfgg.html

print("err", file=sys.stderr)
来源：http://hz.c1oappe.top/gtcharduim.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.vqdsnc.cn/gtolntqnmt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.nanxuanxn.top/gtoxruqvai.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.chenlongwang.top/gtqxzsubbp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.quarkkingdee.top/gtsfmscalm.html

[U43] PHP：声明命名空间
来源：http://hz.wangdashe.top/gtohjimxzd.html

namespace App\Http;
来源：http://hz.ppjwa.cn/gtdblxfzsn.html

[U44] PHP：开启严格类型
来源：http://hz.0kj1m.cn/gtbgkohadk.html

declare(strict_types=1);
来源：http://hz.hammf.cn/gttukdhjnk.html

[U45] PHP：类型声明与返回类型
来源：http://hz.chenzaomai.com/gtvneqmfbx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tanke756.top/gtoedokrgy.html

[U46] PHP：可空类型
来源：http://hz.sufxvd.cn/gtckaiukxx.html

?string $name = null
来源：http://hz.jinqigfzy.top/gtyynxmqly.html

[U47] PHP：联合类型
来源：http://hz.ydzc1.top/gtakujttuj.html

int|string $id
来源：http://hz.sufxvd.cn/gtkuqnopcy.html

[U48] PHP：纯枚举
来源：http://hz.zhoulong.xyz/gtqiatsqku.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.sufxvd.cn/gtsnaagrij.html

[U49] PHP：只读属性
来源：http://hz.ivvv.top/gtzueityco.html

public readonly string $name
来源：http://hz.sysykeji.top/gttcqhugvc.html

[U50] PHP：构造器属性提升
来源：http://hz.birdmap.top/gtzodnpwfj.html

public function __construct(private int $id) {}
来源：http://hz.vqdsnc.cn/gtbkhdhwlw.html

[U51] PHP：数组解构
来源：http://hz.daxiang520.top/gtvywoqeae.html

[$a, $b] = $arr;
来源：http://hz.ehwqpu.com/gtnabmltjp.html

[U52] PHP：箭头函数
来源：http://hz.zhiwuduotai.top/gtofpffjxr.html

$double = fn($x) => $x * 2;
来源：http://hz.hfpthk.cn/gtqcvxqwgw.html

[U53] PHP：空合并运算符
来源：http://hz.gogol.net.cn/gtmbtunjeo.html

$v = $a ?? $b ?? "default";
来源：http://hz.birdmap.top/gtcrffktjv.html

[U54] PHP：空安全调用
来源：http://hz.hammf.cn/gtanuqldmi.html

$obj?->method()
来源：http://hz.yangfankeji.com/gtnlqidprj.html

[U55] PHP：match 表达式
来源：http://hz.hongshengwenyu.top/gtxgzijirb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.haohaochexian.top/gtrymxamsi.html

[U56] PHP：命名参数
来源：http://hz.ivvv.top/gtbywpsvur.html

f(a: 1, b: 2)
来源：http://hz.dashuyun.cn/gtskrvirhb.html

[U57] PHP：字符串插值
来源：http://hz.jinqigufen.top/gtuwhglhrr.html

"值: {$a}"
来源：http://hz.316326.xyz/gtfczqiwpn.html

[U58] PHP：数组三件套
来源：http://hz.hysaishi.cn/gtndzqnvnn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.smart0.xyz/gtfcytlrfl.html

[U59] PHP：自定义排序
来源：http://hz.fzhhl.top/gtuyrconjc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tanke756.top/gttnyntlpp.html

[U60] PHP：JSON 编解码
来源：http://hz.jqgufenzy.top/gtqblzyxgd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yj20258888.top/gtbwagainr.html

[U61] PHP：正则
来源：http://hz.cucudq.cn/gtlyeyfbfq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yanxiufei.cn/gtykjxfopw.html

[U62] PHP：日期对象
来源：http://hz.sysykeji.top/gtbtnrlyrd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.birdmap.top/gtithuurbf.html

[U63] PHP：文件读写
来源：http://hz.havefunace.top/gtfrkoysvz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.shangyingyoupin.top/gtpodelfto.html

[U64] PHP：目录遍历
来源：http://hz.yj20258888.top/gtssvvmxiq.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.chenjidiqi.icu/gthzigpvny.html

[U65] PHP：会话
来源：http://hz.shanyushiyangkeji.top/gtiyhlfmwd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.52xcode.cn/gtxvghmlga.html

[U66] PHP：设置 Cookie
来源：http://hz.bjfxy.top/gtffjwtxlt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jqgufenzy.top/gtrmqgiybq.html

[U67] PHP：处理文件上传
来源：http://hz.ehwqpu.com/gtigxhanjm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.hammf.cn/gtdzvpfzcp.html

[U68] PHP：PDO 连接
来源：http://hz.0kj1m.cn/gtskwdokdj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.meibo888.top/gtljqceeel.html

[U69] PHP：PDO 预处理
来源：http://hz.cashguo.top/gtlxzafwuw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.sufxvd.cn/gtgtkebnzl.html

[U70] PHP：PDO 事务
来源：http://hz.yanxiufei.cn/gtffqcddzr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.pengpengdd.cyou/gtzplnsxrn.html

[U71] PHP：抛出异常
来源：http://hz.cucudq.cn/gtpgnsntyn.html

throw new RuntimeException("失败", 500);
来源：http://hz.tian-w.cn/gtpqmlpnum.html

[U72] PHP：写错误日志
来源：http://hz.cdnleiting.top/gtimobsstm.html

error_log("失败: " . $e->getMessage());
来源：http://hz.cashguo.top/gtsxwqaovp.html

[U73] PHP：读取 ini 配置
来源：http://hz.meibo888.top/gtcsadmczq.html

parse_ini_file("config.ini", true)
来源：http://hz.xuetiantiany.cn/gtnnsdfdsk.html

[U74] PHP：读取环境变量
来源：http://hz.ydjk.org.cn/gtonfjzmxf.html

getenv("APP_ENV") ?: "production"
来源：http://hz.gzhubu.top/gtbgsnkltz.html

[U75] PHP：依赖注入
来源：http://hz.jinqigfzy.top/gtbxegrric.html

composer require psr/container
来源：http://hz.ppjwa.cn/gtohuzusal.html

[U76] PHP：简单路由
来源：http://hz.cdnleiting.top/gtobmdxmaz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.0kj1m.cn/gtrghgwzqw.html

[U77] PHP：模板渲染
来源：http://hz.sysykeji.top/gturjdecgw.html

composer require twig/twig
来源：http://hz.zhixingplan.top/gtiqtmodcx.html

[U78] PHP：单元测试
来源：http://hz.chenjidiqi.icu/gtrcrkcnyq.html

composer require --dev phpunit/phpunit
来源：http://hz.guannengcc.top/gtqwblykgi.html

[U79] PHP：静态分析
来源：http://hz.tian-w.cn/gtwaklsiov.html

composer require --dev phpstan/phpstan
来源：http://hz.chenjidiqi.icu/gtxkibwdgi.html

[U80] PHP：代码规范修复
来源：http://hz.tianlin.xyz/gtboabcpfd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.cashguo.top/gtsvumpcgc.html

[U81] JS：初始化项目
来源：http://hz.sxryk.cn/gtcshovnyp.html

npm init -y;  npm i express
来源：http://hz.zhaomingkeji.xyz/gtapftoltq.html

[U82] JS：package.json 脚本
来源：http://hz.gaohongyu789.top/gtqvqfboib.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zhijiandao.cn/gtcsfxrvau.html

[U83] JS：ES Module 导入导出
来源：http://hz.zdqjudy.top/gtopptkzlh.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.wangshuangyany.cn/gtxrdaiwdu.html

[U84] JS：CommonJS 写法
来源：http://hz.havefunace.top/gtskapsqgs.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.tanke756.top/gtmfpjbxco.html

[U85] JS：可选链
来源：http://hz.jqgfzy.top/gtuybwyfly.html

a?.b?.c
来源：http://hz.gzhubu.top/gtecarbyiq.html

[U86] JS：空值合并
来源：http://hz.zhixingplan.top/gtqpjpdzyt.html

a ?? b
来源：http://hz.hnxiangtu.top/gtfcfurill.html

[U87] JS：解构默认值
来源：http://hz.meibo888.top/gtbkqyqmve.html

const { a = 1, b = 2 } = obj;
来源：http://hz.shuidangran.top/gtrosyqrij.html

[U88] JS：对象展开合并
来源：http://hz.52xcode.cn/gtdhavkjxw.html

{ ...a, ...b }
来源：http://hz.smart0.xyz/gtrasevmeo.html

[U89] JS：数组去重
来源：http://hz.zhiwuduotai.top/gtamfvwxua.html

[...new Set(arr)]
来源：http://hz.ywan-chungtsiang.top/gtenxcxscb.html

[U90] JS：数字数组排序
来源：http://hz.jlsjyb.cn/gtcmyyqaen.html

[...arr].sort((a, b) => a - b)
来源：http://hz.sufxvd.cn/gtktozylzi.html

[U91] JS：对象键值遍历
来源：http://hz.tianlin.xyz/gtxweogiyi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.shzxlz.cn/gtvshdgnab.html

[U92] JS：深拷贝
来源：http://hz.zhoulong.xyz/gtdclzjhto.html

structuredClone(obj)
来源：http://hz.ivvv.top/gtrwivdvlh.html

[U93] JS：模板字符串
来源：http://hz.guowangkeji.top/gtrjnmboow.html

`共 ${n} 条`
来源：http://hz.zycfv.cn/gtelcynnyu.html

[U94] JS：箭头函数
来源：http://hz.jinghuilouyu.cn/gtkrlsoyst.html

const double = x => x * 2;
来源：http://hz.nwbrower.top/gtnpkmlbps.html

[U95] JS：Promise 包装
来源：http://hz.shuidangran.top/gtfepkolvo.html

new Promise((resolve, reject) => {})
来源：http://hz.pengpengdd.cyou/gtiuxkdvsc.html

[U96] JS：async/await 与异常
来源：http://hz.yj20258888.top/gtxqxhgbdy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.havefunace.top/gtrmxvlsll.html

[U97] JS：并发请求
来源：http://hz.mhx1999.top/gtwwekswcn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhongyouzk.top/gthpkinfcr.html

[U98] JS：fetch 带 JSON
来源：http://hz.kuanghao11.cn/gtlqzymvzr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.guowangkeji.top/gtwiaobnmw.html

[U99] JS：事件监听
来源：http://hz.jinqigufen.top/gtqofjjvls.html

el.addEventListener("click", e => {})
来源：http://hz.redwolf501.top/gtwpnwiwbe.html

[U100] JS：DOM 查询
来源：http://hz.tanke756.top/gtfdbcgmic.html

document.querySelector(".item")
来源：http://hz.tian-w.cn/gtlfydnrtb.html

[U101] JS：classList 操作
来源：http://hz.xingfuxueyuan.xyz/gtqtabhzqy.html

el.classList.toggle("active")
来源：http://hz.daxiang520.top/gthxmwwziy.html

[U102] JS：本地存储
来源：http://hz.sweek.top/gtivauylik.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.feifeiyinyue.top/gtycmfpcwv.html

[U103] JS：定时器
来源：http://hz.yuxming.cn/gtkqukktdn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.haohaochexian.top/gtfrqoxglh.html

[U104] JS：防抖
来源：http://hz.sysykeji.top/gtsqeqwjdz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.vqdsnc.cn/gtqxgduldv.html

[U105] JS：节流
来源：http://hz.ehwqpu.com/gtasscrecf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jinyuanbaomall.cn/gtyqnzblst.html

[U106] JS：日期格式化
来源：http://hz.ydjk.org.cn/gtyyxwwdjc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.cqqwz.cn/gttyxsuyxz.html

[U107] JS：数字千分位
来源：http://hz.cdnleiting.top/gtihauwihg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.aizwys.cn/gtrtgrktev.html

[U108] JS：随机整数
来源：http://hz.sxryk.cn/gtotgfdzcn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zhoulong.xyz/gtqaioozst.html

[U109] JS：数组分组
来源：http://hz.aibaodan.cn/gtpalpygxt.html

Object.groupBy(arr, x => x.type)
来源：http://hz.zycfv.cn/gtxxftsoap.html

[U110] JS：数组分块
来源：http://hz.jlsjyb.cn/gtnzfjtayr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.tanke756.top/gtlblgwicg.html

[U111] JS：对象转 Map
来源：http://hz.jinghuilouyu.cn/gtvmdiugww.html

new Map(Object.entries(obj))
来源：http://hz.ydjk.org.cn/gtgqowbjtn.html

[U112] JS：字符串补位
来源：http://hz.zhaomingkeji.xyz/gtmrrlrhcx.html

"7".padStart(3, "0")
来源：http://hz.shanyushiyangtech.top/gttskdwtwa.html

[U113] JS：正则替换全部
来源：http://hz.yongpay.top/gttjunphix.html

s.replaceAll("a", "b")
来源：http://hz.hywenlv.cn/gtlowxbuae.html

[U114] JS：JSON 深比较
来源：http://hz.shuidangran.top/gteqyakfuz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gaohongyu789.top/gtukqwlabv.html

[U115] JS：生成 UUID
来源：http://hz.sxryk.cn/gtcsrovsgi.html

crypto.randomUUID()
来源：http://hz.ppjwa.cn/gtjvbzodaw.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jinqigufen.top/gtewkmnyca.html

/** @param {string} name */ function f(name) {}
来源：http://hz.dianchejie.cn/gtlbawkjfu.html

[U117] JS：单元测试
来源：http://hz.bjfxy.top/gtvahjrfni.html

npm i -D vitest;  npx vitest
来源：http://hz.sufxvd.cn/gttnmreuqm.html

[U118] JS：开发服务器
来源：http://hz.hnxiangtu.top/gtguphgksj.html

npm i -D vite;  npx vite
来源：http://hz.cqqwz.cn/gtyyuoxuhi.html

[U119] JS：生产构建
来源：http://hz.redwolf501.top/gtgwlixgwk.html

npx vite build
来源：http://hz.zhijiandao.cn/gtpxistiiq.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.kuanghao11.cn/gtipsfjndw.html

import.meta.env.VITE_API_URL
来源：http://hz.yongpay.top/gtvitlraax.html

================================================================================
来源：http://hz.ydzc1.top/gtscahqtiv.html

统计汇总
来源：http://hz.chenlongwang.top/gtdxgfzrxk.html

================================================================================
来源：http://hz.c1oappe.top/gtucqiiniu.html

按语言统计（条）：
来源：http://hz.chenlongwang.top/gtygdgyurj.html

Python ......... 252
来源：http://hz.birdmap.top/gtyjtkexzd.html

PHP ............ 252
来源：http://hz.zhongyouzk.top/gtvasxmkzs.html

JavaScript ..... 252
来源：http://hz.zhengqikj.top/gtokpyeoeq.html

TypeScript ..... 212
来源：http://hz.dianchejie.cn/gtkvsqyalg.html

Java ........... 212
来源：http://hz.yuanzhike.top/gtxwakubag.html

Go ............. 212
来源：http://hz.52xcode.cn/gtzysuccsa.html

Ruby ........... 212
来源：http://hz.havefunace.top/gtakglubqj.html

C# ............. 212
来源：http://hz.yanxiufei.cn/gtxbdhydss.html

C .............. 30
来源：http://hz.hnxiangtu.top/gtzwsbhbev.html

C++ ............ 30
来源：http://hz.xylfe.cn/gtiqqzujzl.html

SQL ............ 90
来源：http://hz.chenlongwang.top/gtuvphxpiy.html

Bash ........... 80
来源：http://hz.hammf.cn/gtfbfqxlae.html

Kotlin ......... 15
来源：http://hz.nanxuanxn.top/gteqwlzgpj.html

Swift .......... 15
来源：http://hz.shanyushiyangkeji.top/gtyrglnfov.html

Lua ............ 10
来源：http://hz.cqqwz.cn/gtelezktst.html

Perl ........... 10
来源：http://hz.svipenyu.cn/gtaqdkbtrp.html

Scala .......... 10
来源：http://hz.bjfxy.top/gtiifvxhiw.html

------------------------------------
来源：http://hz.jyoumei.cn/gthsrdonsv.html

合计 ........... 2106 条
来源：http://hz.xuetiantiany.cn/gthobfmpms.html

按章节统计：
来源：http://hz.ydjk.org.cn/gtaweopewj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.52xcode.cn/gtvtqtxpxa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hongshengwenyu.top/gtivfioaar.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yueranfly.top/gtfijvhmaz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zhijiandao.cn/gtrxtpyzxq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.cheryme.top/gtzhtdzitm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.shangyingyoupin.top/gtzkocoszy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hysaishi.cn/gtcatftskd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.xinyue.icu/gtarferumo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.wangdashe.top/gtpdhtggfd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.meibo888.top/gtvlnluqwa.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.redwolf501.top/gtrazcbcen.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.tianlin.xyz/gtthcydmny.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.shangyingyoupin.top/gtrqnjpgxf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.hywenlv.cn/gtzxnjpmxa.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.daxiang520.top/gtqyjnwvdk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gtiihjwgmf.html

Q SQL 专题                              90
来源：http://hz.zhiwuduotai.top/gtcrreyltm.html

R Bash 专题                             80
来源：http://hz.ydjk.org.cn/gtoqohakfd.html

S C / C++ 专题                          60
来源：http://hz.zhengqikj.top/gtvmhygtoq.html

T 其他语言补充                          60
来源：http://hz.sxryk.cn/gtejjerwag.html

U 高频实用片段                         120
来源：http://hz.haohaochexian.top/gtzjrkpzti.html

------------------------------------
来源：http://hz.chenjidiqi.icu/gtvaycwvvw.html

合计                                  2106 条
来源：http://hz.nanxinkj.top/gtnnhmlzsj.html

--------------------------------------------------------------------------------
来源：http://hz.zhiwuduotai.top/gtuxlikylt.html

使用提醒
来源：http://hz.guowangkeji.top/gtfgwedkls.html

--------------------------------------------------------------------------------
来源：http://hz.gzhubu.top/gttypvqliy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.haohaochexian.top/gtnytbdipa.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.aibaodan.cn/gtgqxltcjt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.dashuyun.cn/gtlekhtezf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.xuetiantiany.cn/gtwxsdciup.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yongpay.top/gtifzcqhyx.html

—— 文件结束 ——
来源：http://hz.ybcxt.top/gtlvdfpfrc.html

================================================================================
来源：http://hz.snrcjt.cn/gtmsgitchc.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.sweek.top/gterzgdwjk.html

Common Programming Examples Cheat Book
来源：http://hz.zycfv.cn/gttfspicun.html

================================================================================
来源：http://hz.redwolf501.top/gteeurbdrg.html

【收录内容】
来源：http://hz.snrcjt.cn/gtswqfwhzs.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.shzxlz.cn/gtzdandkkn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.hfpthk.cn/gtwevljqwc.html

SQL · Bash · C · C++
来源：http://hz.guowangkeji.top/gthmcgqzdx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.nanxinkj.top/gtxxmorfiz.html

【使用说明】
来源：http://hz.guowangkeji.top/gtwpedhqua.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zycfv.cn/gtsykxvica.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jqgufenzy.top/gthcdqkhvh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jinqigfzy.top/gtwqoesfjb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yj202588.top/gtuvqoleyf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.hfpthk.cn/gtgxpfgkry.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.vqdsnc.cn/gtrboyijec.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.tian-w.cn/gtsckguvno.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.c1oappe.top/gtvcryrbgl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.chenlongwang.top/gttcsdauhu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jlsjyb.cn/gtkfeomdkw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.hywenlv.cn/gtxgryuiph.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yongpay.top/gtzibssspi.html

【文件统计】
来源：http://hz.yonumen.top/gtwrgdvmos.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.bjfxy.top/gtncxdqfgf.html


<!-- 参考信息 -->