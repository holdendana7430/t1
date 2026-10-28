代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.chenjidiqi.icu/gtvuiwzhrs.html

================================================================================
来源：http://hz.jqgfzy.top/gtyiascsig.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.gaohongyu789.top/gtcsazrpgj.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtawvsfevg.html

[U01] Py：创建虚拟环境
来源：http://hz.bjfxy.top/gtrycdrfay.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yuanzhike.top/gtovueomag.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yj202588.top/gtzhiltbfx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.bjfxy.top/gttwwegcfs.html

[U03] Py：加载 .env 配置
来源：http://hz.yj202588.top/gtiaquhyvt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.tianlin.xyz/gttacynhaj.html

[U04] Py：变量调试打印
来源：http://hz.fengsongda.top/gtbubfhvvr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.fzhhl.top/gtjrmaepkx.html

[U05] Py：列表去重且保序
来源：http://hz.hywenlv.cn/gtgdummcwr.html

list(dict.fromkeys(arr))
来源：http://hz.iojbl.cn/gticaoyyfp.html

[U06] Py：合并两个字典
来源：http://hz.jiagoushi.top/gtdfotvzzj.html

{**a, **b}
来源：http://hz.daxiang520.top/gtoydetahn.html

[U07] Py：反转字典键值
来源：http://hz.mhx1999.top/gtbglucztm.html

{v: k for k, v in d.items()}
来源：http://hz.gaohongyu789.top/gtnsdiyzxl.html

[U08] Py：展平二维列表
来源：http://hz.pycfn.com/gtevcxibxx.html

[y for x in nested for y in x]
来源：http://hz.cqqwz.cn/gtzijrzqnr.html

[U09] Py：字典取最大值的键
来源：http://hz.gaohongyu789.top/gtzsgrgkxc.html

max(d, key=d.get)
来源：http://hz.pengpengdd.cyou/gtdelrgxli.html

[U10] Py：按值排序字典
来源：http://hz.guowangkeji.top/gtzdwnlrdk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.andypj.xyz/gtjxjhfpsr.html

[U11] Py：生成器表达式
来源：http://hz.316326.xyz/gtvxqlxeyx.html

(x * 2 for x in arr)
来源：http://hz.feifeiyinyue.top/gthzybgaot.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ehwqpu.com/gtbvcnalvc.html

Counter(arr).most_common(3)
来源：http://hz.9152youxi.cn/gtjbpgayuz.html

[U13] Py：固定长度队列
来源：http://hz.tianlin.xyz/gtdjtjjmvd.html

deque(maxlen=10)
来源：http://hz.xingfuxueyuan.xyz/gtdzcxmxes.html

[U14] Py：分组收集到列表
来源：http://hz.pycfn.com/gtcyhgwuoq.html

defaultdict(list)
来源：http://hz.quarkkingdee.top/gtwnpfyncd.html

[U15] Py：高精度计时
来源：http://hz.cqqwz.cn/gtnbruqjfr.html

t = time.perf_counter()
来源：http://hz.kuanghao11.cn/gtfzijofas.html

[U16] Py：命令行参数解析
来源：http://hz.sxryk.cn/gtirdgtclt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ybcxt.top/gtegdrzlan.html

[U17] Py：初始化日志
来源：http://hz.jinqigfzy.top/gtygqpgpri.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.52xcode.cn/gtjxfyzjuw.html

[U18] Py：预编译正则
来源：http://hz.mhx1999.top/gtnpslzjam.html

pat = re.compile(r"\d+")
来源：http://hz.ppjwa.cn/gtcwszjofy.html

[U19] Py：正则替换带回调
来源：http://hz.nwbrower.top/gtvutrazon.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yj202588.top/gttjgxzrfl.html

[U20] Py：缓存函数结果
来源：http://hz.meibo888.top/gtauajbjjd.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zycfv.cn/gtdsgzoasj.html

[U21] Py：自定义上下文管理器
来源：http://hz.sweek.top/gtmjkymwty.html

@contextlib.contextmanager
来源：http://hz.zhijiandao.cn/gtlhnhbvkw.html

[U22] Py：矩阵转置
来源：http://hz.52xcode.cn/gtocrxyxct.html

list(zip(*m))
来源：http://hz.shanyushiyangtech.top/gtffjksxht.html

[U23] Py：分块读取大文件
来源：http://hz.yanxiufei.cn/gteltqmgzx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.sysykeji.top/gtnuglynvy.html

[U24] Py：路径操作
来源：http://hz.svipenyu.cn/gtkteqptjc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.cheryme.top/gtkecgxeik.html

[U25] Py：CSV 按字典读
来源：http://hz.ybcxt.top/gtysqurlkk.html

csv.DictReader(f)
来源：http://hz.havefunace.top/gtakgwnkgj.html

[U26] Py：并发下载
来源：http://hz.yvedp.cn/gtwubqizoc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yuanzhike.top/gtjmpwgmfp.html

[U27] Py：异步 HTTP
来源：http://hz.birdmap.top/gtkxxixysg.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.c1oappe.top/gtcqmagltb.html

[U28] Py：类型别名
来源：http://hz.yangfankeji.com/gtvwsykjyt.html

UserId = int
来源：http://hz.hysaishi.cn/gtwwbyvvxb.html

[U29] Py：属性校验
来源：http://hz.ydzc1.top/gtisjsapad.html

@property 与 @x.setter 配合
来源：http://hz.chenjidiqi.icu/gticqcogzo.html

[U30] Py：数据类
来源：http://hz.hywenlv.cn/gtormuyqlp.html

@dataclass(slots=True)
来源：http://hz.redwolf501.top/gtnztunwqs.html

[U31] Py：单测
来源：http://hz.jianghu66.top/gtshrdosma.html

python -m pytest -q
来源：http://hz.ydzc1.top/gttkfflmtg.html

[U32] Py：代码格式化
来源：http://hz.cdnleiting.top/gthreupakw.html

ruff format . && ruff check --fix .
来源：http://hz.jqgufenzy.top/gtutfsvqzv.html

[U33] Py：打包发布
来源：http://hz.tianlin.xyz/gtgogzxcez.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.sufxvd.cn/gtvozuatwl.html

[U34] Py：判断编码
来源：http://hz.zhiwuduotai.top/gttnnqxmmx.html

chardet.detect(raw)
来源：http://hz.sxryk.cn/gtsfugisbs.html

[U35] Py：发送邮件
来源：http://hz.haohaochexian.top/gtdgjsiean.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cdnleiting.top/gtvwmvkcui.html

[U36] Py：定时任务
来源：http://hz.iojbl.cn/gtczqhjtqq.html

schedule.every(10).minutes.do(job)
来源：http://hz.xylfe.cn/gtnxjvrlkp.html

[U37] Py：读写 Excel
来源：http://hz.sufxvd.cn/gtxvmzcprq.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yangfankeji.com/gtoaemiicl.html

[U38] Py：获取脚本所在目录
来源：http://hz.hfpthk.cn/gtpazwrwfd.html

Path(__file__).resolve().parent
来源：http://hz.wangdashe.top/gtutldbnym.html

[U39] Py：判断是否在交互环境
来源：http://hz.fengsongda.top/gtfvwzfwvu.html

sys.stdout.isatty()
来源：http://hz.redwolf501.top/gtolesjxcf.html

[U40] Py：打印到标准错误
来源：http://hz.yj20258.top/gtroiskrmj.html

print("err", file=sys.stderr)
来源：http://hz.xuanzx.com/gtabejetbu.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.snrcjt.cn/gtmldenbpm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ybcxt.top/gttdpgjmdj.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xuetiantiany.cn/gtzgtmlzsx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.kuanghao11.cn/gtgmpxbqcs.html

[U43] PHP：声明命名空间
来源：http://hz.yueranfly.top/gtgtkriirr.html

namespace App\Http;
来源：http://hz.guowangkeji.top/gtaksbanlp.html

[U44] PHP：开启严格类型
来源：http://hz.wangdashe.top/gtdhznkkpe.html

declare(strict_types=1);
来源：http://hz.nanxuanxn.top/gtrnfxavtv.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hammf.cn/gtjqzzuhxf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.c1oappe.top/gteszfhfyq.html

[U46] PHP：可空类型
来源：http://hz.yj202588.top/gttprafwea.html

?string $name = null
来源：http://hz.smart0.xyz/gtiwihwinu.html

[U47] PHP：联合类型
来源：http://hz.nanxuanxn.top/gtqfudlckr.html

int|string $id
来源：http://hz.feifeiyinyue.top/gtpptylwig.html

[U48] PHP：纯枚举
来源：http://hz.hammf.cn/gtapyyviym.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.redwolf501.top/gtrcdiwicb.html

[U49] PHP：只读属性
来源：http://hz.bjfxy.top/gtrndmxujn.html

public readonly string $name
来源：http://hz.9152youxi.cn/gtzyelzbsx.html

[U50] PHP：构造器属性提升
来源：http://hz.gaohongyu789.top/gtoimhqhwp.html

public function __construct(private int $id) {}
来源：http://hz.jinqigufen.top/gtcjwunejl.html

[U51] PHP：数组解构
来源：http://hz.yuanzhike.top/gtfdfnrdvz.html

[$a, $b] = $arr;
来源：http://hz.tianlin.xyz/gteeweworj.html

[U52] PHP：箭头函数
来源：http://hz.wangshuangyany.cn/gtbynneliz.html

$double = fn($x) => $x * 2;
来源：http://hz.zhixingplan.top/gtbbejaeoh.html

[U53] PHP：空合并运算符
来源：http://hz.yj20258.top/gttczjxrqy.html

$v = $a ?? $b ?? "default";
来源：http://hz.kuanghao11.cn/gtosyifegg.html

[U54] PHP：空安全调用
来源：http://hz.cucudq.cn/gtqxiqvuhe.html

$obj?->method()
来源：http://hz.fzhhl.top/gtdloyfsch.html

[U55] PHP：match 表达式
来源：http://hz.shangyingyoupin.top/gtthqpujrx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ppjwa.cn/gtrsyrnatv.html

[U56] PHP：命名参数
来源：http://hz.c1oappe.top/gtgkcsidvw.html

f(a: 1, b: 2)
来源：http://hz.bjfxy.top/gtzgyidxru.html

[U57] PHP：字符串插值
来源：http://hz.yvedp.cn/gtgrpcddsy.html

"值: {$a}"
来源：http://hz.dashuyun.cn/gteyhyoopf.html

[U58] PHP：数组三件套
来源：http://hz.aizwys.cn/gtkfumovyx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.guowangkeji.top/gtnuchgysf.html

[U59] PHP：自定义排序
来源：http://hz.gzhubu.top/gtwcnmmhuh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yvedp.cn/gtrjztcroq.html

[U60] PHP：JSON 编解码
来源：http://hz.hywenlv.cn/gtuqdhkbhc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jiagoushi.top/gtrkavxbzo.html

[U61] PHP：正则
来源：http://hz.vqdsnc.cn/gtikbqghrq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.iojbl.cn/gtakyeqfwb.html

[U62] PHP：日期对象
来源：http://hz.fzhhl.top/gtquuuwhci.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.gaohongyu789.top/gtssmkqoin.html

[U63] PHP：文件读写
来源：http://hz.cashguo.top/gtoyxbarjo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.c1oappe.top/gtqqmcvdvj.html

[U64] PHP：目录遍历
来源：http://hz.kuanghao11.cn/gtufffdbno.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.fzhhl.top/gtldddnxag.html

[U65] PHP：会话
来源：http://hz.svipenyu.cn/gtiplcwycc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.gogol.net.cn/gthqiqbpng.html

[U66] PHP：设置 Cookie
来源：http://hz.mhx1999.top/gtcenvdfoo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.cucudq.cn/gtadeowlxx.html

[U67] PHP：处理文件上传
来源：http://hz.dashuyun.cn/gtylfiphnk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.chenjidiqi.icu/gtsogjmowv.html

[U68] PHP：PDO 连接
来源：http://hz.fengsongda.top/gtsvethpuf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.sufxvd.cn/gtmeiffgzn.html

[U69] PHP：PDO 预处理
来源：http://hz.nanxinkj.top/gtyiuockxk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jianghu66.top/gthsndiwfj.html

[U70] PHP：PDO 事务
来源：http://hz.tian-w.cn/gtwuibvmkw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.daxiang520.top/gtsfwjxdul.html

[U71] PHP：抛出异常
来源：http://hz.316326.xyz/gtryxnywyr.html

throw new RuntimeException("失败", 500);
来源：http://hz.jqgfzy.top/gtlcyryprp.html

[U72] PHP：写错误日志
来源：http://hz.wangdashe.top/gtacbjdugj.html

error_log("失败: " . $e->getMessage());
来源：http://hz.chenlongwang.top/gtekminmil.html

[U73] PHP：读取 ini 配置
来源：http://hz.kuanghao11.cn/gtvpvlhgpu.html

parse_ini_file("config.ini", true)
来源：http://hz.birdmap.top/gtscrxbewn.html

[U74] PHP：读取环境变量
来源：http://hz.wangshuangyany.cn/gtwaaobxrl.html

getenv("APP_ENV") ?: "production"
来源：http://hz.gzhubu.top/gtlavwpvgu.html

[U75] PHP：依赖注入
来源：http://hz.aibaodan.cn/gtdzwydwxv.html

composer require psr/container
来源：http://hz.andypj.xyz/gtrhgqlmxd.html

[U76] PHP：简单路由
来源：http://hz.9152youxi.cn/gtxnatpbfb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.sxryk.cn/gtpqxogenu.html

[U77] PHP：模板渲染
来源：http://hz.ybcxt.top/gtybesxkjh.html

composer require twig/twig
来源：http://hz.pengpengdd.cyou/gthmgabkpz.html

[U78] PHP：单元测试
来源：http://hz.jinqigufen.top/gtqbbocuqq.html

composer require --dev phpunit/phpunit
来源：http://hz.shangyingyoupin.top/gtmzymjhjz.html

[U79] PHP：静态分析
来源：http://hz.dianchejie.cn/gtdgvbuoar.html

composer require --dev phpstan/phpstan
来源：http://hz.shanyushiyangtech.top/gttevazguh.html

[U80] PHP：代码规范修复
来源：http://hz.vqdsnc.cn/gtqsmgxheq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hnxiangtu.top/gtoofjrihz.html

[U81] JS：初始化项目
来源：http://hz.316326.xyz/gtqxkakxri.html

npm init -y;  npm i express
来源：http://hz.jyoumei.cn/gtwbqdwnpn.html

[U82] JS：package.json 脚本
来源：http://hz.havefunace.top/gtkhbomszd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.kuanghao11.cn/gtgvxriadi.html

[U83] JS：ES Module 导入导出
来源：http://hz.52xcode.cn/gtizipgsqr.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.fengsongda.top/gtfxmqdanx.html

[U84] JS：CommonJS 写法
来源：http://hz.dianchejie.cn/gtrnfmsruh.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.ydjk.org.cn/gtucfodkhj.html

[U85] JS：可选链
来源：http://hz.nwbrower.top/gtiiqgxrye.html

a?.b?.c
来源：http://hz.wangshuangyany.cn/gttnlghdpl.html

[U86] JS：空值合并
来源：http://hz.svipenyu.cn/gtmohwfffa.html

a ?? b
来源：http://hz.jinqigufen.top/gtlrzcgigs.html

[U87] JS：解构默认值
来源：http://hz.yuxming.cn/gtsgolekaz.html

const { a = 1, b = 2 } = obj;
来源：http://hz.birdmap.top/gtqevwnuim.html

[U88] JS：对象展开合并
来源：http://hz.hnqzz.top/gtnbwuhyly.html

{ ...a, ...b }
来源：http://hz.aibaodan.cn/gtfjlcadbc.html

[U89] JS：数组去重
来源：http://hz.daxiang520.top/gtslcjebmz.html

[...new Set(arr)]
来源：http://hz.sweek.top/gtzmxtqhcq.html

[U90] JS：数字数组排序
来源：http://hz.zhiwuduotai.top/gtrtxquxjp.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yangfankeji.com/gtwwznyibe.html

[U91] JS：对象键值遍历
来源：http://hz.hongshengwenyu.top/gtdajrmwdz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.guannengcc.top/gtpvdcnmwa.html

[U92] JS：深拷贝
来源：http://hz.jyoumei.cn/gttaygaozc.html

structuredClone(obj)
来源：http://hz.ivvv.top/gtjslpwxep.html

[U93] JS：模板字符串
来源：http://hz.ydzc1.top/gtcrpgrptw.html

`共 ${n} 条`
来源：http://hz.sweek.top/gtfudpzbfz.html

[U94] JS：箭头函数
来源：http://hz.snrcjt.cn/gtqrkpqstp.html

const double = x => x * 2;
来源：http://hz.yueranfly.top/gtdsayyvex.html

[U95] JS：Promise 包装
来源：http://hz.zhoulong.xyz/gttcqtrbqr.html

new Promise((resolve, reject) => {})
来源：http://hz.cqqwz.cn/gtunomblmj.html

[U96] JS：async/await 与异常
来源：http://hz.ehwqpu.com/gtnicrhqdp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.guannengcc.top/gtujrtcjfl.html

[U97] JS：并发请求
来源：http://hz.pengpengdd.cyou/gtwrufjjdn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jyoumei.cn/gtbuafxyqd.html

[U98] JS：fetch 带 JSON
来源：http://hz.hywenlv.cn/gtwhrrnajo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.dianchejie.cn/gtobjfiydo.html

[U99] JS：事件监听
来源：http://hz.hongshengwenyu.top/gtxlstutsj.html

el.addEventListener("click", e => {})
来源：http://hz.xylfe.cn/gtpfucqptu.html

[U100] JS：DOM 查询
来源：http://hz.xingfuxueyuan.xyz/gtlrccknsh.html

document.querySelector(".item")
来源：http://hz.haohaochexian.top/gtownzboua.html

[U101] JS：classList 操作
来源：http://hz.hongshengwenyu.top/gtxycwdbgi.html

el.classList.toggle("active")
来源：http://hz.ywan-chungtsiang.top/gttnfxanhg.html

[U102] JS：本地存储
来源：http://hz.wangshuangyany.cn/gtvwycagzz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.sweek.top/gtezynakdr.html

[U103] JS：定时器
来源：http://hz.sysykeji.top/gtvfibqipr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xziqi.cn/gtauonroek.html

[U104] JS：防抖
来源：http://hz.yj20258.top/gtrzjwsdrd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.iojbl.cn/gtrspdnxpg.html

[U105] JS：节流
来源：http://hz.yuxming.cn/gtliwzxteh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jqgufenzy.top/gtuijvurwj.html

[U106] JS：日期格式化
来源：http://hz.vqdsnc.cn/gtmhmlwrkd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.xuanzx.com/gtjfncuall.html

[U107] JS：数字千分位
来源：http://hz.jqgufenzy.top/gtactptgeu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ydjk.org.cn/gteeggsymn.html

[U108] JS：随机整数
来源：http://hz.jinqigfzy.top/gtsukdhity.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jinqigfzy.top/gtcvzufmaq.html

[U109] JS：数组分组
来源：http://hz.ywan-chungtsiang.top/gtwelgbtgi.html

Object.groupBy(arr, x => x.type)
来源：http://hz.ivvv.top/gtwvbqjsxs.html

[U110] JS：数组分块
来源：http://hz.ivvv.top/gtjasfvxzk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zhoulong.xyz/gtkzxmlcjn.html

[U111] JS：对象转 Map
来源：http://hz.yj20258888.top/gtgxqbaass.html

new Map(Object.entries(obj))
来源：http://hz.daria6918.cn/gtikpatjpf.html

[U112] JS：字符串补位
来源：http://hz.daria6918.cn/gtfxzuzwrp.html

"7".padStart(3, "0")
来源：http://hz.tian-w.cn/gtbqnzydsl.html

[U113] JS：正则替换全部
来源：http://hz.9152youxi.cn/gtggxwdpss.html

s.replaceAll("a", "b")
来源：http://hz.aizwys.cn/gtnsrnooyl.html

[U114] JS：JSON 深比较
来源：http://hz.snrcjt.cn/gtejlkyced.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.smart0.xyz/gtcuclqwlv.html

[U115] JS：生成 UUID
来源：http://hz.svipenyu.cn/gtzxwmoecb.html

crypto.randomUUID()
来源：http://hz.fzhhl.top/gtuxfzuxsy.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.shangyingyoupin.top/gtizeseipw.html

/** @param {string} name */ function f(name) {}
来源：http://hz.gogol.net.cn/gtqywzwtwn.html

[U117] JS：单元测试
来源：http://hz.ppjwa.cn/gtlzedpghj.html

npm i -D vitest;  npx vitest
来源：http://hz.9152youxi.cn/gtsuoftevi.html

[U118] JS：开发服务器
来源：http://hz.316326.xyz/gtcwfrqhpf.html

npm i -D vite;  npx vite
来源：http://hz.iojbl.cn/gtzzswjcbh.html

[U119] JS：生产构建
来源：http://hz.dashuyun.cn/gtakkthzdk.html

npx vite build
来源：http://hz.yangfankeji.com/gttxaqdaba.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jinyuanbaomall.cn/gtuyihhwju.html

import.meta.env.VITE_API_URL
来源：http://hz.cdnleiting.top/gtbzxgwats.html

================================================================================
来源：http://hz.kuanghao11.cn/gtsmpyazed.html

统计汇总
来源：http://hz.mhx1999.top/gtbvddpima.html

================================================================================
来源：http://hz.cqqwz.cn/gtygtpxgsk.html

按语言统计（条）：
来源：http://hz.ppjwa.cn/gtiesvooia.html

Python ......... 252
来源：http://hz.xuanzx.com/gtbpbwravi.html

PHP ............ 252
来源：http://hz.zhengqikj.top/gtxmwewxzm.html

JavaScript ..... 252
来源：http://hz.yongpay.top/gtjnygzojh.html

TypeScript ..... 212
来源：http://hz.hammf.cn/gtegxxedrc.html

Java ........... 212
来源：http://hz.zycfv.cn/gtvmwpctrt.html

Go ............. 212
来源：http://hz.vqdsnc.cn/gtwhmafouk.html

Ruby ........... 212
来源：http://hz.chenjidiqi.icu/gttbqordug.html

C# ............. 212
来源：http://hz.zhixingplan.top/gtdtlndicj.html

C .............. 30
来源：http://hz.yueranfly.top/gtbgqdziqm.html

C++ ............ 30
来源：http://hz.ppjwa.cn/gtndxjwlqr.html

SQL ............ 90
来源：http://hz.xuanzx.com/gtyicrdgjl.html

Bash ........... 80
来源：http://hz.nanxinkj.top/gtbzmrjesk.html

Kotlin ......... 15
来源：http://hz.zhaomingkeji.xyz/gtrmqhifrw.html

Swift .......... 15
来源：http://hz.zhengqikj.top/gtvwbcuubl.html

Lua ............ 10
来源：http://hz.tanke756.top/gtlnlqchku.html

Perl ........... 10
来源：http://hz.shanyushiyangtech.top/gtupjlrpqf.html

Scala .......... 10
来源：http://hz.yangfankeji.com/gtbkyocxye.html

------------------------------------
来源：http://hz.nwbrower.top/gtnvnlqspi.html

合计 ........... 2106 条
来源：http://hz.zdqjudy.top/gtcqvjwssw.html

按章节统计：
来源：http://hz.dashuyun.cn/gtldtssyvw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yuxming.cn/gtzvffpfkt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zdqjudy.top/gtnynwglim.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.svipenyu.cn/gtdvqhaxcn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jyoumei.cn/gtvmaqziyi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.ydzc1.top/gtjgchqmmb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.nwbrower.top/gtheinbjfw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.mhx1999.top/gtglzlsqzl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.xuanzx.com/gtmxyxdimq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jinqigfzy.top/gtoxpqgcji.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.meibo888.top/gtxpjyjmyr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.shzxlz.cn/gtakulrntb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.shuidangran.top/gtacypcfnt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.gaohongyu789.top/gtmifilgfp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.ehwqpu.com/gthcgiyxxq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.tanke756.top/gtdahoubkd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jiagoushi.top/gtjvyzlird.html

Q SQL 专题                              90
来源：http://hz.zhijiandao.cn/gtqyxemwbf.html

R Bash 专题                             80
来源：http://hz.quarkkingdee.top/gtihnyoigu.html

S C / C++ 专题                          60
来源：http://hz.bjfxy.top/gtqzckfinu.html

T 其他语言补充                          60
来源：http://hz.sweek.top/gtmxrzccga.html

U 高频实用片段                         120
来源：http://hz.smart0.xyz/gtzixhegyu.html

------------------------------------
来源：http://hz.tian-w.cn/gttavknuuw.html

合计                                  2106 条
来源：http://hz.ehwqpu.com/gtmzuqiwkm.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigfzy.top/gtojxtatqu.html

使用提醒
来源：http://hz.zycfv.cn/gtehexzaem.html

--------------------------------------------------------------------------------
来源：http://hz.smart0.xyz/gtzwrqwgmx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.nwbrower.top/gtnuffjrrh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.mhx1999.top/gtglymfxrc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.feifeiyinyue.top/gtdrhyoksh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.chenjidiqi.icu/gtuncerwwy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.feifeiyinyue.top/gttwxqcycy.html

—— 文件结束 ——
来源：http://hz.pengpengdd.cyou/gtchjkxakx.html


<!-- 参考信息 -->