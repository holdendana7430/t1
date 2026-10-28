代发 wailian999

[U05] Py：列表去重且保序
来源：http://hz.yueranfly.top/gttctcfoow.html

list(dict.fromkeys(arr))
来源：http://hz.zhongyouzk.top/gtpnejcpsq.html

[U06] Py：合并两个字典
来源：http://hz.shuidangran.top/gtxdbzzsoy.html

{**a, **b}
来源：http://hz.gogol.net.cn/gtiucqtbbm.html

[U07] Py：反转字典键值
来源：http://hz.wangdashe.top/gtbtwwdkvb.html

{v: k for k, v in d.items()}
来源：http://hz.yongpay.top/gtuswzaxey.html

[U08] Py：展平二维列表
来源：http://hz.yonumen.top/gtwfuhzyrc.html

[y for x in nested for y in x]
来源：http://hz.hnxiangtu.top/gtlzyeixnf.html

[U09] Py：字典取最大值的键
来源：http://hz.feifeiyinyue.top/gtpfytuxfp.html

max(d, key=d.get)
来源：http://hz.chenlongwang.top/gtdqoicezt.html

[U10] Py：按值排序字典
来源：http://hz.jinyuanbaomall.cn/gtohriadjo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.bjfxy.top/gttvfuxfep.html

[U11] Py：生成器表达式
来源：http://hz.xuetiantiany.cn/gtvopisyvr.html

(x * 2 for x in arr)
来源：http://hz.snrcjt.cn/gtmbwrilcu.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.nanxinkj.top/gtldlyqncy.html

Counter(arr).most_common(3)
来源：http://hz.cashguo.top/gtimxewted.html

[U13] Py：固定长度队列
来源：http://hz.havefunace.top/gtnvgtwham.html

deque(maxlen=10)
来源：http://hz.c1oappe.top/gtwekkcwep.html

[U14] Py：分组收集到列表
来源：http://hz.zhaomingkeji.xyz/gttliojtiv.html

defaultdict(list)
来源：http://hz.zhengqikj.top/gtagwwqyib.html

[U15] Py：高精度计时
来源：http://hz.snrcjt.cn/gtqplwdddl.html

t = time.perf_counter()
来源：http://hz.hnqzz.top/gtqpgkbekp.html

[U16] Py：命令行参数解析
来源：http://hz.yueranfly.top/gtrqymqsme.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jyoumei.cn/gtyhklfnal.html

[U17] Py：初始化日志
来源：http://hz.hammf.cn/gtloilbtgd.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.shanyushiyangtech.top/gtvijxdliy.html

[U18] Py：预编译正则
来源：http://hz.ybcxt.top/gtykvncgtl.html

pat = re.compile(r"\d+")
来源：http://hz.gaohongyu789.top/gthftztsij.html

[U19] Py：正则替换带回调
来源：http://hz.316326.xyz/gtfglrvlfd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.iojbl.cn/gtnauqrghu.html

[U20] Py：缓存函数结果
来源：http://hz.quarkkingdee.top/gtznfgipdc.html

@functools.lru_cache(maxsize=None)
来源：http://hz.c1oappe.top/gtilxmzheu.html

[U21] Py：自定义上下文管理器
来源：http://hz.yvedp.cn/gtmbrdhiex.html

@contextlib.contextmanager
来源：http://hz.sxryk.cn/gtytdiexpq.html

[U22] Py：矩阵转置
来源：http://hz.jqgufenzy.top/gtmsmgbppe.html

list(zip(*m))
来源：http://hz.smart0.xyz/gtzjqsowjn.html

[U23] Py：分块读取大文件
来源：http://hz.jiagoushi.top/gtsrdxwqui.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cdnleiting.top/gtjhmazxpu.html

[U24] Py：路径操作
来源：http://hz.cqqwz.cn/gtsyxhrkba.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hongshengwenyu.top/gtyvljqejj.html

[U25] Py：CSV 按字典读
来源：http://hz.chenlongwang.top/gtwcvctykn.html

csv.DictReader(f)
来源：http://hz.tianlin.xyz/gtnlkptlzh.html

[U26] Py：并发下载
来源：http://hz.nanxinkj.top/gtdomspaii.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.daxiang520.top/gtciohxdtg.html

[U27] Py：异步 HTTP
来源：http://hz.havefunace.top/gtjtlxcoqm.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.xuetiantiany.cn/gtighucmub.html

[U28] Py：类型别名
来源：http://hz.dashuyun.cn/gttkjfujcz.html

UserId = int
来源：http://hz.wangshuangyany.cn/gtfpjsgnzi.html

[U29] Py：属性校验
来源：http://hz.cashguo.top/gtuqbkyzav.html

@property 与 @x.setter 配合
来源：http://hz.chenlongwang.top/gtxvfwfhsk.html

[U30] Py：数据类
来源：http://hz.hnqzz.top/gtofxhwydu.html

@dataclass(slots=True)
来源：http://hz.chenjidiqi.icu/gtqhuxgfpa.html

[U31] Py：单测
来源：http://hz.yongpay.top/gtghmwkufn.html

python -m pytest -q
来源：http://hz.jqgfzy.top/gtkmopflsf.html

[U32] Py：代码格式化
来源：http://hz.zycfv.cn/gtkymdhbuk.html

ruff format . && ruff check --fix .
来源：http://hz.redwolf501.top/gtgcfxhnto.html

[U33] Py：打包发布
来源：http://hz.shanyushiyangtech.top/gtmluxapbv.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.gzhubu.top/gtxnfypdez.html

[U34] Py：判断编码
来源：http://hz.jianghu66.top/gtnhgnsggk.html

chardet.detect(raw)
来源：http://hz.tanke756.top/gtijxwswbq.html

[U35] Py：发送邮件
来源：http://hz.daxiang520.top/gtucrvhwfm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jinqigufen.top/gtmqycupww.html

[U36] Py：定时任务
来源：http://hz.sysykeji.top/gtqwqhrvpf.html

schedule.every(10).minutes.do(job)
来源：http://hz.yj202588.top/gthetgjhxm.html

[U37] Py：读写 Excel
来源：http://hz.chenjidiqi.icu/gtcrnznczv.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yongpay.top/gtrufqsind.html

[U38] Py：获取脚本所在目录
来源：http://hz.chenjidiqi.icu/gtyihwjbfa.html

Path(__file__).resolve().parent
来源：http://hz.havefunace.top/gtumzvhoky.html

[U39] Py：判断是否在交互环境
来源：http://hz.jinghuilouyu.cn/gtwgwtwesh.html

sys.stdout.isatty()
来源：http://hz.nanxinkj.top/gtwlpfeyos.html

[U40] Py：打印到标准错误
来源：http://hz.zhengqikj.top/gtesvulnkl.html

print("err", file=sys.stderr)
来源：http://hz.shuidangran.top/gtlhlwetbu.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.shangyingyoupin.top/gtjxnqcvdg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhaomingkeji.xyz/gtfvfwvsmr.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.shanyushiyangtech.top/gtwszbmmyz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.xinyue.icu/gttlmhljjn.html

[U43] PHP：声明命名空间
来源：http://hz.pycfn.com/gttprxetuw.html

namespace App\Http;
来源：http://hz.jinyuanbaomall.cn/gthdqzupfa.html

[U44] PHP：开启严格类型
来源：http://hz.sysykeji.top/gtkueweror.html

declare(strict_types=1);
来源：http://hz.ybcxt.top/gtwyskgvim.html

[U45] PHP：类型声明与返回类型
来源：http://hz.cqqwz.cn/gtqdntgmep.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zycfv.cn/gtiuxjeuce.html

[U46] PHP：可空类型
来源：http://hz.gzhubu.top/gtqgrzpkfu.html

?string $name = null
来源：http://hz.meibo888.top/gtwffnecql.html

[U47] PHP：联合类型
来源：http://hz.yuanzhike.top/gticjshjwl.html

int|string $id
来源：http://hz.nanxinkj.top/gtivyheftc.html

[U48] PHP：纯枚举
来源：http://hz.zhongyouzk.top/gtgqmqmmcb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhaomingkeji.xyz/gtvjvygqsk.html

[U49] PHP：只读属性
来源：http://hz.cdnleiting.top/gthuifubkl.html

public readonly string $name
来源：http://hz.cqqwz.cn/gtybqkdqrz.html

[U50] PHP：构造器属性提升
来源：http://hz.meibo888.top/gtrazwsaci.html

public function __construct(private int $id) {}
来源：http://hz.gotoacloud.top/gtdloeejrx.html

[U51] PHP：数组解构
来源：http://hz.yuanzhike.top/gtvfewqmdo.html

[$a, $b] = $arr;
来源：http://hz.cheryme.top/gtzxzsadup.html

[U52] PHP：箭头函数
来源：http://hz.zhiwuduotai.top/gtpopqaamu.html

$double = fn($x) => $x * 2;
来源：http://hz.guowangkeji.top/gtrqkvukdn.html

[U53] PHP：空合并运算符
来源：http://hz.xingfuxueyuan.xyz/gtmljswgdk.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhixingplan.top/gtpsrursal.html

[U54] PHP：空安全调用
来源：http://hz.yongpay.top/gtotokysgp.html

$obj?->method()
来源：http://hz.aizwys.cn/gtvpfqoyqc.html

[U55] PHP：match 表达式
来源：http://hz.xingfuxueyuan.xyz/gtdhdegrzy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.wangshuangyany.cn/gtjabngpdb.html

[U56] PHP：命名参数
来源：http://hz.zhengqikj.top/gtqfiebfhs.html

f(a: 1, b: 2)
来源：http://hz.birdmap.top/gtdfbdxtcg.html

[U57] PHP：字符串插值
来源：http://hz.zhiwuduotai.top/gttjtrimaw.html

"值: {$a}"
来源：http://hz.andypj.xyz/gtisdmxmlv.html

[U58] PHP：数组三件套
来源：http://hz.dianchejie.cn/gtqpxclbjm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.316326.xyz/gtxyezlioz.html

[U59] PHP：自定义排序
来源：http://hz.jqgfzy.top/gtmyjgxbja.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jianghu66.top/gtvdbxwjud.html

[U60] PHP：JSON 编解码
来源：http://hz.wangdashe.top/gtjjltgpdz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.nanxinkj.top/gtwsskclig.html

[U61] PHP：正则
来源：http://hz.chenlongwang.top/gtnvplzbjw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.gogol.net.cn/gtxsyualzg.html

[U62] PHP：日期对象
来源：http://hz.hongshengwenyu.top/gtdmmplykv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.ivvv.top/gteohherin.html

[U63] PHP：文件读写
来源：http://hz.zhiwuduotai.top/gtmjhcxgpq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.smart0.xyz/gtvfvqnhnq.html

[U64] PHP：目录遍历
来源：http://hz.sweek.top/gtuxjtizvf.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yangfankeji.com/gtsqymcntu.html

[U65] PHP：会话
来源：http://hz.yueranfly.top/gtqahttqrr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.ydjk.org.cn/gtrweybzim.html

[U66] PHP：设置 Cookie
来源：http://hz.daxiang520.top/gtkxnewgdh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.xylfe.cn/gtsvyqxoux.html

[U67] PHP：处理文件上传
来源：http://hz.xinyue.icu/gtateohsvu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.iojbl.cn/gtmwotlskl.html

[U68] PHP：PDO 连接
来源：http://hz.sweek.top/gtvpfvoiww.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jinqigfzy.top/gtlvkdackk.html

[U69] PHP：PDO 预处理
来源：http://hz.yj20258888.top/gthtlckopc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yuanzhike.top/gtykeksjyb.html

[U70] PHP：PDO 事务
来源：http://hz.mhx1999.top/gtzopcwhyu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.smart0.xyz/gtlguwymmq.html

[U71] PHP：抛出异常
来源：http://hz.yvedp.cn/gtqehcjqzw.html

throw new RuntimeException("失败", 500);
来源：http://hz.yj20258.top/gtxkmxpycx.html

[U72] PHP：写错误日志
来源：http://hz.iojbl.cn/gtsxgowlmg.html

error_log("失败: " . $e->getMessage());
来源：http://hz.haohaochexian.top/gtddolurjn.html

[U73] PHP：读取 ini 配置
来源：http://hz.redwolf501.top/gthmznivsr.html

parse_ini_file("config.ini", true)
来源：http://hz.dashuyun.cn/gtwtztzjkv.html

[U74] PHP：读取环境变量
来源：http://hz.shanyushiyangkeji.top/gtnkawuhbm.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jianghu66.top/gtuswezexe.html

[U75] PHP：依赖注入
来源：http://hz.yuanzhike.top/gtikmkbwel.html

composer require psr/container
来源：http://hz.cheryme.top/gttexruyfg.html

[U76] PHP：简单路由
来源：http://hz.yvedp.cn/gtcrwpieay.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jinghuilouyu.cn/gtuultcpqa.html

[U77] PHP：模板渲染
来源：http://hz.aibaodan.cn/gtkkvfksnr.html

composer require twig/twig
来源：http://hz.haohaochexian.top/gttgohmekk.html

[U78] PHP：单元测试
来源：http://hz.sysykeji.top/gtaduelwak.html

composer require --dev phpunit/phpunit
来源：http://hz.hysaishi.cn/gtvfvjtjts.html

[U79] PHP：静态分析
来源：http://hz.yvedp.cn/gtoqvrjchy.html

composer require --dev phpstan/phpstan
来源：http://hz.haohaochexian.top/gtqokkaucy.html

[U80] PHP：代码规范修复
来源：http://hz.jinghuilouyu.cn/gtxkprzvej.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhoulong.xyz/gtbricqblk.html

[U81] JS：初始化项目
来源：http://hz.jianghu66.top/gtxaszwxat.html

npm init -y;  npm i express
来源：http://hz.pengpengdd.cyou/gtxulkefwq.html

[U82] JS：package.json 脚本
来源：http://hz.feifeiyinyue.top/gttunnjeyg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.sweek.top/gtebxrooxg.html

[U83] JS：ES Module 导入导出
来源：http://hz.feifeiyinyue.top/gtomzquyzp.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zhiwuduotai.top/gtankekngr.html

[U84] JS：CommonJS 写法
来源：http://hz.cdnleiting.top/gtbvyayocy.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.sufxvd.cn/gtipcilgfr.html

[U85] JS：可选链
来源：http://hz.0kj1m.cn/gtmbbaabbf.html

a?.b?.c
来源：http://hz.zhixingplan.top/gthkdurvhv.html

[U86] JS：空值合并
来源：http://hz.hnxiangtu.top/gtyrejgogu.html

a ?? b
来源：http://hz.yongpay.top/gtiulrzotf.html

[U87] JS：解构默认值
来源：http://hz.xuetiantiany.cn/gtnvttljyv.html

const { a = 1, b = 2 } = obj;
来源：http://hz.ywan-chungtsiang.top/gtoisrdncz.html

[U88] JS：对象展开合并
来源：http://hz.gotoacloud.top/gtbkitypfn.html

{ ...a, ...b }
来源：http://hz.sufxvd.cn/gtmklkxmlm.html

[U89] JS：数组去重
来源：http://hz.9152youxi.cn/gthsyokjge.html

[...new Set(arr)]
来源：http://hz.c1oappe.top/gticvngxje.html

[U90] JS：数字数组排序
来源：http://hz.havefunace.top/gthqxqjhkf.html

[...arr].sort((a, b) => a - b)
来源：http://hz.redwolf501.top/gtsavkdqdd.html

[U91] JS：对象键值遍历
来源：http://hz.pycfn.com/gtowxsjtgi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.cheryme.top/gtvjwjtpkj.html

[U92] JS：深拷贝
来源：http://hz.sufxvd.cn/gtbvjbbkpr.html

structuredClone(obj)
来源：http://hz.chenlongwang.top/gtxolzepws.html

[U93] JS：模板字符串
来源：http://hz.hnqzz.top/gtxbbpyyex.html

`共 ${n} 条`
来源：http://hz.xylfe.cn/gtigicsqne.html

[U94] JS：箭头函数
来源：http://hz.wangdashe.top/gtyqirjtgn.html

const double = x => x * 2;
来源：http://hz.zhaomingkeji.xyz/gthbftyquz.html

[U95] JS：Promise 包装
来源：http://hz.yueranfly.top/gtpijbinsj.html

new Promise((resolve, reject) => {})
来源：http://hz.wangshuangyany.cn/gtefrgosbc.html

[U96] JS：async/await 与异常
来源：http://hz.yj20258.top/gterhitsui.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.hammf.cn/gtongnagjm.html

[U97] JS：并发请求
来源：http://hz.yongpay.top/gtiepacwbo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtbggzvlqp.html

[U98] JS：fetch 带 JSON
来源：http://hz.tianlin.xyz/gtwkaukegt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.gogol.net.cn/gtkjlguqsc.html

[U99] JS：事件监听
来源：http://hz.cucudq.cn/gtqezdirjs.html

el.addEventListener("click", e => {})
来源：http://hz.zhixingplan.top/gtfaoinwip.html

[U100] JS：DOM 查询
来源：http://hz.cqqwz.cn/gtwgefhurf.html

document.querySelector(".item")
来源：http://hz.yonumen.top/gttqszdpnx.html

[U101] JS：classList 操作
来源：http://hz.xingfuxueyuan.xyz/gtjeoxkzua.html

el.classList.toggle("active")
来源：http://hz.pengpengdd.cyou/gtaossvjof.html

[U102] JS：本地存储
来源：http://hz.zhaomingkeji.xyz/gtebycxomb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jinqigfzy.top/gtzhtebskb.html

[U103] JS：定时器
来源：http://hz.yonumen.top/gtwswtecbw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.mhx1999.top/gtubgpufed.html

[U104] JS：防抖
来源：http://hz.hfpthk.cn/gtxiiivkcu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.iojbl.cn/gttmtifiav.html

[U105] JS：节流
来源：http://hz.cqqwz.cn/gtmfmcqorc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.cdnleiting.top/gtvotwzlxo.html

[U106] JS：日期格式化
来源：http://hz.yuanzhike.top/gtlarqxvnl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ybcxt.top/gtposdnwfv.html

[U107] JS：数字千分位
来源：http://hz.svipenyu.cn/gthfpunkve.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.shanyushiyangtech.top/gtnbhhutqm.html

[U108] JS：随机整数
来源：http://hz.9152youxi.cn/gtazowbaai.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zhiwuduotai.top/gtumvaelra.html

[U109] JS：数组分组
来源：http://hz.havefunace.top/gtifmleavt.html

Object.groupBy(arr, x => x.type)
来源：http://hz.gogol.net.cn/gtuqxhupom.html

[U110] JS：数组分块
来源：http://hz.xuetiantiany.cn/gtvodpetbp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.xuanzx.com/gtawnhcewo.html

[U111] JS：对象转 Map
来源：http://hz.yueranfly.top/gtjntqmkgw.html

new Map(Object.entries(obj))
来源：http://hz.aizwys.cn/gtraxlnopo.html

[U112] JS：字符串补位
来源：http://hz.jqgufenzy.top/gtawumijcq.html

"7".padStart(3, "0")
来源：http://hz.daxiang520.top/gttihlubon.html

[U113] JS：正则替换全部
来源：http://hz.havefunace.top/gtyhhtbnwq.html

s.replaceAll("a", "b")
来源：http://hz.smart0.xyz/gttofzimbz.html

[U114] JS：JSON 深比较
来源：http://hz.gaohongyu789.top/gtbtxzldun.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gzhubu.top/gtzdvilmrb.html

[U115] JS：生成 UUID
来源：http://hz.zhengqikj.top/gtkhbyxmcv.html

crypto.randomUUID()
来源：http://hz.yj20258888.top/gtkupmnuna.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.tianlin.xyz/gtidkncuzo.html

/** @param {string} name */ function f(name) {}
来源：http://hz.hfpthk.cn/gtaybisbuo.html

[U117] JS：单元测试
来源：http://hz.haohaochexian.top/gtviigrtcr.html

npm i -D vitest;  npx vitest
来源：http://hz.yj202588.top/gtvoyssvrt.html

[U118] JS：开发服务器
来源：http://hz.hnxiangtu.top/gtcxqzmsll.html

npm i -D vite;  npx vite
来源：http://hz.jinghuilouyu.cn/gtshnpxtcs.html

[U119] JS：生产构建
来源：http://hz.xziqi.cn/gtfcltkirh.html

npx vite build
来源：http://hz.haohaochexian.top/gtcoqlvcpt.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.gzhubu.top/gtjxsztzae.html

import.meta.env.VITE_API_URL
来源：http://hz.dashuyun.cn/gtdseytzgr.html

================================================================================
来源：http://hz.yongpay.top/gtwigzxdod.html

统计汇总
来源：http://hz.cqqwz.cn/gthukgukel.html

================================================================================
来源：http://hz.smart0.xyz/gteovyejvh.html

按语言统计（条）：
来源：http://hz.316326.xyz/gtxqaqigrq.html

Python ......... 252
来源：http://hz.gogol.net.cn/gthgbhuewg.html

PHP ............ 252
来源：http://hz.zhijiandao.cn/gtlywudqzd.html

JavaScript ..... 252
来源：http://hz.jinghuilouyu.cn/gtjyfnonsw.html

TypeScript ..... 212
来源：http://hz.zhiwuduotai.top/gtcaqvfjms.html

Java ........... 212
来源：http://hz.gotoacloud.top/gtrxayecir.html

Go ............. 212
来源：http://hz.shanyushiyangkeji.top/gttpxxrevf.html

Ruby ........... 212
来源：http://hz.chenlongwang.top/gtgqeckjkw.html

C# ............. 212
来源：http://hz.ppjwa.cn/gtuyqidwey.html

C .............. 30
来源：http://hz.gotoacloud.top/gthisuiqsl.html

C++ ............ 30
来源：http://hz.nanxuanxn.top/gtrixtooot.html

SQL ............ 90
来源：http://hz.hfpthk.cn/gtqsapcvni.html

Bash ........... 80
来源：http://hz.wangshuangyany.cn/gtctbudunh.html

Kotlin ......... 15
来源：http://hz.c1oappe.top/gtxivmnocl.html

Swift .......... 15
来源：http://hz.vqdsnc.cn/gtwkbhmfvm.html

Lua ............ 10
来源：http://hz.shuidangran.top/gtzrqlownh.html

Perl ........... 10
来源：http://hz.hammf.cn/gtfeuqpypj.html

Scala .......... 10
来源：http://hz.quarkkingdee.top/gtjqlcevps.html

------------------------------------
来源：http://hz.zhongyouzk.top/gtmxiripxe.html

合计 ........... 2106 条
来源：http://hz.haohaochexian.top/gtkyixpqee.html

按章节统计：
来源：http://hz.birdmap.top/gtybbqogij.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.ybcxt.top/gtjkrudwqq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.gzhubu.top/gtqqnskdwu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.ydjk.org.cn/gtafkdejub.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.dashuyun.cn/gtdcawglav.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.aizwys.cn/gtaysuqjrf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.ydzc1.top/gtrkyvekhg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jinqigfzy.top/gtkwzrtlix.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.chenzaomai.com/gtluvstjpj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yonumen.top/gtdshroihd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yanxiufei.cn/gtnrlabqix.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.316326.xyz/gthuqxcwxk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.hysaishi.cn/gtrdicwufq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.shuidangran.top/gticoewkul.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.xinyue.icu/gtfpflcpae.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.redwolf501.top/gtxrcncwjx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.hongshengwenyu.top/gtqsitshby.html

Q SQL 专题                              90
来源：http://hz.cqqwz.cn/gtyjtimxok.html

R Bash 专题                             80
来源：http://hz.wangdashe.top/gtyskfrhai.html

S C / C++ 专题                          60
来源：http://hz.tianlin.xyz/gtwrlgbrvu.html

T 其他语言补充                          60
来源：http://hz.yueranfly.top/gtueyjfkit.html

U 高频实用片段                         120
来源：http://hz.jinyuanbaomall.cn/gthxllqazp.html

------------------------------------
来源：http://hz.jlsjyb.cn/gtzklyjzdv.html

合计                                  2106 条
来源：http://hz.fengsongda.top/gtqgwluops.html

--------------------------------------------------------------------------------
来源：http://hz.xuanzx.com/gtuifmvvrg.html

使用提醒
来源：http://hz.snrcjt.cn/gttxgaxgxt.html

--------------------------------------------------------------------------------
来源：http://hz.daxiang520.top/gtbjnagkjl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.tianlin.xyz/gtxjdbivlz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.ydjk.org.cn/gtnxzkmvde.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.sxryk.cn/gtiuxvgkex.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.ywan-chungtsiang.top/gtqbizwafu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.guowangkeji.top/gtjarkqspo.html

—— 文件结束 ——
来源：http://hz.hnqzz.top/gtqlgzvaoz.html

================================================================================
来源：http://hz.smart0.xyz/gtqerzsaoi.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.kuanghao11.cn/gtialsqvsv.html

Common Programming Examples Cheat Book
来源：http://hz.hysaishi.cn/gtwyspwozv.html

================================================================================
来源：http://hz.daxiang520.top/gtshbbcgls.html

【收录内容】
来源：http://hz.yonumen.top/gtcobxxvfy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.hnxiangtu.top/gtcfrhwtpp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jinqigfzy.top/gtogcixped.html

SQL · Bash · C · C++
来源：http://hz.zhiwuduotai.top/gtckbcojap.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.dashuyun.cn/gterytbfgh.html

【使用说明】
来源：http://hz.gotoacloud.top/gtrgbxcvlr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.shangyingyoupin.top/gtczmoqulq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zdqjudy.top/gtkwencleh.html


<!-- 参考信息 -->