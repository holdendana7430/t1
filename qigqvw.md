代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yj202588.top/gtsrmrehrg.html

[T59] Scala：循环
来源：http://hz.ivvv.top/gtwrwkwfuz.html

for (i <- 1 to 10) println(i)
来源：http://hz.pycfn.com/gtaqdbicvl.html

[T60] Scala：折叠
来源：http://hz.birdmap.top/gtkjdwzekv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.chenzaomai.com/gtucnxbqpi.html

================================================================================
来源：http://hz.cqqwz.cn/gtodnkposo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ydjk.org.cn/gtdlrjbjzf.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtfiavmxpi.html

[U01] Py：创建虚拟环境
来源：http://hz.yongpay.top/gtksuncaas.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.pengpengdd.cyou/gttsohhxhf.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hnxiangtu.top/gtqjklvntf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.chenzaomai.com/gthpxfanuz.html

[U03] Py：加载 .env 配置
来源：http://hz.chenzaomai.com/gthhaylzyx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yonumen.top/gtqizgxxzo.html

[U04] Py：变量调试打印
来源：http://hz.hongshengwenyu.top/gthsghzana.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.quarkkingdee.top/gtmlrwygkr.html

[U05] Py：列表去重且保序
来源：http://hz.nanxuanxn.top/gtkhwiywgk.html

list(dict.fromkeys(arr))
来源：http://hz.jinqigfzy.top/gtznoippby.html

[U06] Py：合并两个字典
来源：http://hz.xziqi.cn/gtgvcemkek.html

{**a, **b}
来源：http://hz.gotoacloud.top/gttrcczzau.html

[U07] Py：反转字典键值
来源：http://hz.xuetiantiany.cn/gtfjwfvwht.html

{v: k for k, v in d.items()}
来源：http://hz.cheryme.top/gtgjhbmsiz.html

[U08] Py：展平二维列表
来源：http://hz.jianghu66.top/gtpuxkhkvj.html

[y for x in nested for y in x]
来源：http://hz.xziqi.cn/gtoodhskvh.html

[U09] Py：字典取最大值的键
来源：http://hz.snrcjt.cn/gthwtbjden.html

max(d, key=d.get)
来源：http://hz.aizwys.cn/gtophjbbqr.html

[U10] Py：按值排序字典
来源：http://hz.yueranfly.top/gtnmtebppb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yangfankeji.com/gtblrxshbc.html

[U11] Py：生成器表达式
来源：http://hz.jianghu66.top/gtdqyzdbre.html

(x * 2 for x in arr)
来源：http://hz.birdmap.top/gtoagqntgh.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.daria6918.cn/gthighsymg.html

Counter(arr).most_common(3)
来源：http://hz.ehwqpu.com/gtmgaqqiyi.html

[U13] Py：固定长度队列
来源：http://hz.jyoumei.cn/gtsbssmzmk.html

deque(maxlen=10)
来源：http://hz.9152youxi.cn/gtezaucrsc.html

[U14] Py：分组收集到列表
来源：http://hz.shanyushiyangtech.top/gtvkbgywie.html

defaultdict(list)
来源：http://hz.316326.xyz/gtzjjovnkl.html

[U15] Py：高精度计时
来源：http://hz.yuxming.cn/gtacxlcyxd.html

t = time.perf_counter()
来源：http://hz.dashuyun.cn/gtrtdrsugx.html

[U16] Py：命令行参数解析
来源：http://hz.zhoulong.xyz/gtxprrmvjg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.nwbrower.top/gttpzsqlkv.html

[U17] Py：初始化日志
来源：http://hz.yueranfly.top/gtrbceodjd.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zdqjudy.top/gtekeyxyqv.html

[U18] Py：预编译正则
来源：http://hz.yonumen.top/gtazfhkmfl.html

pat = re.compile(r"\d+")
来源：http://hz.shanyushiyangtech.top/gtvnhfoodt.html

[U19] Py：正则替换带回调
来源：http://hz.redwolf501.top/gtlcabkggl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.cashguo.top/gtvujsoqwr.html

[U20] Py：缓存函数结果
来源：http://hz.wangshuangyany.cn/gtjhbqddru.html

@functools.lru_cache(maxsize=None)
来源：http://hz.9152youxi.cn/gtcpxtcdku.html

[U21] Py：自定义上下文管理器
来源：http://hz.xingfuxueyuan.xyz/gtbwxshmcb.html

@contextlib.contextmanager
来源：http://hz.jinyuanbaomall.cn/gthnohqvfm.html

[U22] Py：矩阵转置
来源：http://hz.gotoacloud.top/gtbffrnyxt.html

list(zip(*m))
来源：http://hz.xingfuxueyuan.xyz/gtasurybzq.html

[U23] Py：分块读取大文件
来源：http://hz.nwbrower.top/gtugzvjxmb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jinyuanbaomall.cn/gtxztyaevf.html

[U24] Py：路径操作
来源：http://hz.yj20258888.top/gtcnusaaxo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.daxiang520.top/gtmbkstidk.html

[U25] Py：CSV 按字典读
来源：http://hz.jianghu66.top/gttckacked.html

csv.DictReader(f)
来源：http://hz.gzhubu.top/gtlfrdgusx.html

[U26] Py：并发下载
来源：http://hz.xylfe.cn/gtqzwgwuon.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yonumen.top/gtpfmdihvr.html

[U27] Py：异步 HTTP
来源：http://hz.cqqwz.cn/gtmyqzqjmy.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zhijiandao.cn/gtlzevoluh.html

[U28] Py：类型别名
来源：http://hz.shuidangran.top/gtqxqjqztp.html

UserId = int
来源：http://hz.jinyuanbaomall.cn/gtsuxtplnk.html

[U29] Py：属性校验
来源：http://hz.ppjwa.cn/gtzwxzxbci.html

@property 与 @x.setter 配合
来源：http://hz.haohaochexian.top/gthfxivhnz.html

[U30] Py：数据类
来源：http://hz.dianchejie.cn/gthkumdbte.html

@dataclass(slots=True)
来源：http://hz.jyoumei.cn/gtrupwbbmz.html

[U31] Py：单测
来源：http://hz.tian-w.cn/gtefzztksb.html

python -m pytest -q
来源：http://hz.tianlin.xyz/gtwjfjlzol.html

[U32] Py：代码格式化
来源：http://hz.ehwqpu.com/gtmfejdbxt.html

ruff format . && ruff check --fix .
来源：http://hz.ehwqpu.com/gtfxiswfhc.html

[U33] Py：打包发布
来源：http://hz.shanyushiyangtech.top/gtkzpmdmuj.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.0kj1m.cn/gtajyeavzj.html

[U34] Py：判断编码
来源：http://hz.cucudq.cn/gtdseaxsnz.html

chardet.detect(raw)
来源：http://hz.xylfe.cn/gtyidgnkls.html

[U35] Py：发送邮件
来源：http://hz.smart0.xyz/gtqhimxzmx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.tianlin.xyz/gtchelrdzp.html

[U36] Py：定时任务
来源：http://hz.bjfxy.top/gtaaqldohq.html

schedule.every(10).minutes.do(job)
来源：http://hz.kuanghao11.cn/gtfrrcygzi.html

[U37] Py：读写 Excel
来源：http://hz.xingfuxueyuan.xyz/gtrvzznvsh.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yj20258888.top/gtdixawihv.html

[U38] Py：获取脚本所在目录
来源：http://hz.sweek.top/gtwzqvmmfu.html

Path(__file__).resolve().parent
来源：http://hz.zdqjudy.top/gtqhufyuor.html

[U39] Py：判断是否在交互环境
来源：http://hz.guannengcc.top/gtczlqhtgt.html

sys.stdout.isatty()
来源：http://hz.yuxming.cn/gtfwfehley.html

[U40] Py：打印到标准错误
来源：http://hz.cqqwz.cn/gtbwqcfapw.html

print("err", file=sys.stderr)
来源：http://hz.316326.xyz/gtkaoucjoo.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jyoumei.cn/gtmlaamqfz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.sxryk.cn/gtpxwyqpzz.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.chenjidiqi.icu/gthifxvdqg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.daxiang520.top/gtrvsbsrdk.html

[U43] PHP：声明命名空间
来源：http://hz.sufxvd.cn/gtaaxfktub.html

namespace App\Http;
来源：http://hz.wangdashe.top/gtmtjkeenu.html

[U44] PHP：开启严格类型
来源：http://hz.52xcode.cn/gtmexwmpen.html

declare(strict_types=1);
来源：http://hz.jinqigufen.top/gtbtbsqwgo.html

[U45] PHP：类型声明与返回类型
来源：http://hz.bjfxy.top/gtofqehfso.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jlsjyb.cn/gtclesgytw.html

[U46] PHP：可空类型
来源：http://hz.bjfxy.top/gtshsgieik.html

?string $name = null
来源：http://hz.0kj1m.cn/gtprvhgkgi.html

[U47] PHP：联合类型
来源：http://hz.dashuyun.cn/gtsxewferz.html

int|string $id
来源：http://hz.yongpay.top/gtfxhoyvjp.html

[U48] PHP：纯枚举
来源：http://hz.sufxvd.cn/gttvwhlbdo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhengqikj.top/gtkreopqho.html

[U49] PHP：只读属性
来源：http://hz.hongshengwenyu.top/gtngdlkwkv.html

public readonly string $name
来源：http://hz.ywan-chungtsiang.top/gttbxbghir.html

[U50] PHP：构造器属性提升
来源：http://hz.kuanghao11.cn/gtrdzlvyvw.html

public function __construct(private int $id) {}
来源：http://hz.andypj.xyz/gthrsqybhn.html

[U51] PHP：数组解构
来源：http://hz.hammf.cn/gtnxcenyas.html

[$a, $b] = $arr;
来源：http://hz.kuanghao11.cn/gtwsxoimtt.html

[U52] PHP：箭头函数
来源：http://hz.vqdsnc.cn/gtufcucaac.html

$double = fn($x) => $x * 2;
来源：http://hz.shuidangran.top/gtioxzdufm.html

[U53] PHP：空合并运算符
来源：http://hz.jiagoushi.top/gtfnbqiaga.html

$v = $a ?? $b ?? "default";
来源：http://hz.52xcode.cn/gtnheabmey.html

[U54] PHP：空安全调用
来源：http://hz.gaohongyu789.top/gtnkoxaobn.html

$obj?->method()
来源：http://hz.jiagoushi.top/gttnhzfgqu.html

[U55] PHP：match 表达式
来源：http://hz.ydzc1.top/gtfgqhktfn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.gogol.net.cn/gtnjeritgy.html

[U56] PHP：命名参数
来源：http://hz.xuanzx.com/gthhglninj.html

f(a: 1, b: 2)
来源：http://hz.jinyuanbaomall.cn/gtijcfdkpi.html

[U57] PHP：字符串插值
来源：http://hz.tanke756.top/gtidnvahbz.html

"值: {$a}"
来源：http://hz.jinyuanbaomall.cn/gtzinhexsg.html

[U58] PHP：数组三件套
来源：http://hz.0kj1m.cn/gtsjcghucr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.haohaochexian.top/gtwtinndhu.html

[U59] PHP：自定义排序
来源：http://hz.cashguo.top/gtjdtyubze.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daxiang520.top/gtwuwjqqah.html

[U60] PHP：JSON 编解码
来源：http://hz.jiagoushi.top/gtvwzpchvj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.hammf.cn/gtaghtpayf.html

[U61] PHP：正则
来源：http://hz.yj20258888.top/gtnsskgnyv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.fengsongda.top/gtxyytsdhq.html

[U62] PHP：日期对象
来源：http://hz.hnqzz.top/gtkysirtor.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jianghu66.top/gtzoyzhbgx.html

[U63] PHP：文件读写
来源：http://hz.zhixingplan.top/gtatirevwk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yuxming.cn/gtjnxbmwjt.html

[U64] PHP：目录遍历
来源：http://hz.ybcxt.top/gtvsxaheym.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.52xcode.cn/gtbmlmfdrm.html

[U65] PHP：会话
来源：http://hz.dashuyun.cn/gtqvedscfu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.sysykeji.top/gtnhxcsajo.html

[U66] PHP：设置 Cookie
来源：http://hz.chenzaomai.com/gtvbfxaqyl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.xuanzx.com/gtqifmehea.html

[U67] PHP：处理文件上传
来源：http://hz.ivvv.top/gtyhvoimbg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yvedp.cn/gtxfmrwrxx.html

[U68] PHP：PDO 连接
来源：http://hz.tianlin.xyz/gtiwwshcwj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.kuanghao11.cn/gtxgrjefoe.html

[U69] PHP：PDO 预处理
来源：http://hz.yongpay.top/gtbwnlgpyl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zdqjudy.top/gtvktsfjvt.html

[U70] PHP：PDO 事务
来源：http://hz.ehwqpu.com/gtqxmulquh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yonumen.top/gtkyagokkt.html

[U71] PHP：抛出异常
来源：http://hz.sxryk.cn/gtjjkxnzll.html

throw new RuntimeException("失败", 500);
来源：http://hz.jinqigufen.top/gtvcvuityx.html

[U72] PHP：写错误日志
来源：http://hz.gotoacloud.top/gtxzudpfuf.html

error_log("失败: " . $e->getMessage());
来源：http://hz.52xcode.cn/gtuhhrkehd.html

[U73] PHP：读取 ini 配置
来源：http://hz.sufxvd.cn/gtvgurdlkv.html

parse_ini_file("config.ini", true)
来源：http://hz.cheryme.top/gtaepysfku.html

[U74] PHP：读取环境变量
来源：http://hz.hysaishi.cn/gtqiyrnpmp.html

getenv("APP_ENV") ?: "production"
来源：http://hz.c1oappe.top/gtentaqmof.html

[U75] PHP：依赖注入
来源：http://hz.yonumen.top/gttovqrrxl.html

composer require psr/container
来源：http://hz.shanyushiyangtech.top/gtohujxixo.html

[U76] PHP：简单路由
来源：http://hz.chenlongwang.top/gtmnowurvq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jlsjyb.cn/gtqydupezr.html

[U77] PHP：模板渲染
来源：http://hz.ppjwa.cn/gtrccetnpr.html

composer require twig/twig
来源：http://hz.zdqjudy.top/gtdfjgaptv.html

[U78] PHP：单元测试
来源：http://hz.nwbrower.top/gtsypignmt.html

composer require --dev phpunit/phpunit
来源：http://hz.316326.xyz/gtulnmfsxu.html

[U79] PHP：静态分析
来源：http://hz.yvedp.cn/gtdqcwslih.html

composer require --dev phpstan/phpstan
来源：http://hz.ivvv.top/gtvsolpsaf.html

[U80] PHP：代码规范修复
来源：http://hz.daria6918.cn/gtaulrrzet.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yanxiufei.cn/gtifurshal.html

[U81] JS：初始化项目
来源：http://hz.hysaishi.cn/gtveaoctbu.html

npm init -y;  npm i express
来源：http://hz.ydjk.org.cn/gttswwudpb.html

[U82] JS：package.json 脚本
来源：http://hz.bjfxy.top/gtvsgbzzej.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.tianlin.xyz/gtaafugmyi.html

[U83] JS：ES Module 导入导出
来源：http://hz.zdqjudy.top/gtijmxmger.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zhiwuduotai.top/gtcqliiqiz.html

[U84] JS：CommonJS 写法
来源：http://hz.ppjwa.cn/gtsbwtopcv.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.iojbl.cn/gtsjgsuvux.html

[U85] JS：可选链
来源：http://hz.hfpthk.cn/gttuqbsxto.html

a?.b?.c
来源：http://hz.andypj.xyz/gtwzdsqmkz.html

[U86] JS：空值合并
来源：http://hz.svipenyu.cn/gtxekahghe.html

a ?? b
来源：http://hz.chenlongwang.top/gtucjdjkab.html

[U87] JS：解构默认值
来源：http://hz.pycfn.com/gttfjgegdy.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jinqigufen.top/gtrqnsgokj.html

[U88] JS：对象展开合并
来源：http://hz.cucudq.cn/gteqrphvde.html

{ ...a, ...b }
来源：http://hz.nanxinkj.top/gtcrgvdalp.html

[U89] JS：数组去重
来源：http://hz.pycfn.com/gthznkanzj.html

[...new Set(arr)]
来源：http://hz.shanyushiyangtech.top/gtjoypztci.html

[U90] JS：数字数组排序
来源：http://hz.jinghuilouyu.cn/gtnhessqgl.html

[...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtmpklbulk.html

[U91] JS：对象键值遍历
来源：http://hz.jinqigfzy.top/gtycdbyage.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.hysaishi.cn/gtvdyacbbf.html

[U92] JS：深拷贝
来源：http://hz.zhijiandao.cn/gtmfpnlgim.html

structuredClone(obj)
来源：http://hz.jinqigufen.top/gtpluxxhlp.html

[U93] JS：模板字符串
来源：http://hz.yj20258.top/gtxhdnrwzf.html

`共 ${n} 条`
来源：http://hz.hammf.cn/gtcpqilhsu.html

[U94] JS：箭头函数
来源：http://hz.zhixingplan.top/gtmjiyeqsc.html

const double = x => x * 2;
来源：http://hz.cheryme.top/gturaymgqx.html

[U95] JS：Promise 包装
来源：http://hz.fzhhl.top/gthwiixixr.html

new Promise((resolve, reject) => {})
来源：http://hz.shanyushiyangkeji.top/gtlnyruxpa.html

[U96] JS：async/await 与异常
来源：http://hz.wangshuangyany.cn/gtywnvdcgj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.wangdashe.top/gtortqrwdu.html

[U97] JS：并发请求
来源：http://hz.meibo888.top/gtgfmryaxw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtkjlpsucc.html

[U98] JS：fetch 带 JSON
来源：http://hz.quarkkingdee.top/gtybciqchb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.guowangkeji.top/gtnolxovtx.html

[U99] JS：事件监听
来源：http://hz.dianchejie.cn/gtnbqimzrg.html

el.addEventListener("click", e => {})
来源：http://hz.dianchejie.cn/gtifomlgaz.html

[U100] JS：DOM 查询
来源：http://hz.guannengcc.top/gteatcxsyd.html

document.querySelector(".item")
来源：http://hz.ivvv.top/gtsxrovicm.html

[U101] JS：classList 操作
来源：http://hz.jlsjyb.cn/gtdzmwexst.html

el.classList.toggle("active")
来源：http://hz.guannengcc.top/gtankmutpv.html

[U102] JS：本地存储
来源：http://hz.zhijiandao.cn/gtkoqfpawm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yangfankeji.com/gtutrztleg.html

[U103] JS：定时器
来源：http://hz.yueranfly.top/gtxtfcvvjx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xziqi.cn/gtftlymaxu.html

[U104] JS：防抖
来源：http://hz.shuidangran.top/gtpbzjeuji.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.feifeiyinyue.top/gtogdnhdaq.html

[U105] JS：节流
来源：http://hz.sxryk.cn/gtzqdwwcwf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.meibo888.top/gtfsyxkguy.html

[U106] JS：日期格式化
来源：http://hz.yangfankeji.com/gtzxfpzrep.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jinyuanbaomall.cn/gtiokuaudk.html

[U107] JS：数字千分位
来源：http://hz.ydzc1.top/gtxoyzijut.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.feifeiyinyue.top/gtelwnwpbt.html

[U108] JS：随机整数
来源：http://hz.chenjidiqi.icu/gtgnvjazwp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hnqzz.top/gtugvzzbdu.html

[U109] JS：数组分组
来源：http://hz.zhaomingkeji.xyz/gtmsxgjgoc.html

Object.groupBy(arr, x => x.type)
来源：http://hz.shangyingyoupin.top/gtiuvjurou.html

[U110] JS：数组分块
来源：http://hz.zhoulong.xyz/gtxmpnmfgu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.chenlongwang.top/gtgtzxvpxh.html

[U111] JS：对象转 Map
来源：http://hz.jinqigfzy.top/gtnxamdqgt.html

new Map(Object.entries(obj))
来源：http://hz.wangshuangyany.cn/gtyjixdlhq.html

[U112] JS：字符串补位
来源：http://hz.mhx1999.top/gtqartmfoa.html

"7".padStart(3, "0")
来源：http://hz.sysykeji.top/gtqlatdyfw.html

[U113] JS：正则替换全部
来源：http://hz.shangyingyoupin.top/gtnclfnisq.html

s.replaceAll("a", "b")
来源：http://hz.andypj.xyz/gtobvcgrqw.html

[U114] JS：JSON 深比较
来源：http://hz.haohaochexian.top/gtodiurbgb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ehwqpu.com/gtbmsnfwuy.html

[U115] JS：生成 UUID
来源：http://hz.zhixingplan.top/gthkupkvot.html

crypto.randomUUID()
来源：http://hz.hammf.cn/gtarsvngym.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.chenzaomai.com/gtfiuesyah.html

/** @param {string} name */ function f(name) {}
来源：http://hz.ppjwa.cn/gtgmynqxaq.html

[U117] JS：单元测试
来源：http://hz.yj20258.top/gtfedeqdic.html

npm i -D vitest;  npx vitest
来源：http://hz.jlsjyb.cn/gtgiuxlksk.html

[U118] JS：开发服务器
来源：http://hz.zhengqikj.top/gtparqmurv.html

npm i -D vite;  npx vite
来源：http://hz.andypj.xyz/gtnnrqakfe.html

[U119] JS：生产构建
来源：http://hz.cqqwz.cn/gtqqjhqtgb.html

npx vite build
来源：http://hz.bjfxy.top/gtjtedmbed.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.gogol.net.cn/gtgrgwyjxf.html

import.meta.env.VITE_API_URL
来源：http://hz.zhijiandao.cn/gtwiybzfzm.html

================================================================================
来源：http://hz.xziqi.cn/gtkktkdysf.html

统计汇总
来源：http://hz.havefunace.top/gtmydmzuvn.html

================================================================================
来源：http://hz.9152youxi.cn/gtvyhqxcdy.html

按语言统计（条）：
来源：http://hz.zycfv.cn/gtzojbdiwl.html

Python ......... 252
来源：http://hz.hnqzz.top/gtxuldftdo.html

PHP ............ 252
来源：http://hz.daria6918.cn/gtnxjfjdeo.html

JavaScript ..... 252
来源：http://hz.ywan-chungtsiang.top/gtcbsxzfjz.html

TypeScript ..... 212
来源：http://hz.yj20258.top/gtkaosoolq.html

Java ........... 212
来源：http://hz.cucudq.cn/gtdihobraz.html

Go ............. 212
来源：http://hz.zhaomingkeji.xyz/gtazakuasl.html

Ruby ........... 212
来源：http://hz.gogol.net.cn/gtkkqikrvu.html

C# ............. 212
来源：http://hz.tanke756.top/gtvoessrbp.html

C .............. 30
来源：http://hz.vqdsnc.cn/gthenaskoq.html

C++ ............ 30
来源：http://hz.gaohongyu789.top/gturvkwsif.html

SQL ............ 90
来源：http://hz.nanxuanxn.top/gtvxirtaoc.html

Bash ........... 80
来源：http://hz.gotoacloud.top/gtzwlcwkfb.html

Kotlin ......... 15
来源：http://hz.sufxvd.cn/gtrkhwtfkm.html

Swift .......... 15
来源：http://hz.nanxinkj.top/gtvzrxlkou.html

Lua ............ 10
来源：http://hz.yongpay.top/gtftyhmrwh.html

Perl ........... 10
来源：http://hz.yvedp.cn/gtnijopnvt.html

Scala .......... 10
来源：http://hz.gaohongyu789.top/gtqlzobaki.html

------------------------------------
来源：http://hz.yuxming.cn/gtygnonpws.html

合计 ........... 2106 条
来源：http://hz.aizwys.cn/gtznttouba.html

按章节统计：
来源：http://hz.yanxiufei.cn/gtfgfkffui.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhengqikj.top/gtkffwipbm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hysaishi.cn/gtkxxfdzpn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.c1oappe.top/gtuqkmvcih.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ywan-chungtsiang.top/gtgzoevyih.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.nanxuanxn.top/gtbdwhzcmb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.gotoacloud.top/gtgfofltir.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jinghuilouyu.cn/gthulputaa.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.jiagoushi.top/gtadpbqheo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.gzhubu.top/gtxqrvwwto.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yvedp.cn/gtcrtxitqt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.guannengcc.top/gtfanftdqm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.shuidangran.top/gtnhozkutt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.52xcode.cn/gthbqrppmt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.shanyushiyangtech.top/gtjtbqfbkc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yvedp.cn/gtqikmhoek.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.mhx1999.top/gtaxvfwbyk.html

Q SQL 专题                              90
来源：http://hz.dashuyun.cn/gtxfzgoaqu.html

R Bash 专题                             80
来源：http://hz.mhx1999.top/gtwbumkggh.html

S C / C++ 专题                          60
来源：http://hz.xingfuxueyuan.xyz/gtrvoffzoz.html

T 其他语言补充                          60
来源：http://hz.hongshengwenyu.top/gtdiruqygy.html

U 高频实用片段                         120
来源：http://hz.jlsjyb.cn/gtmlgtmgrw.html

------------------------------------
来源：http://hz.sysykeji.top/gtlokuxzxa.html

合计                                  2106 条
来源：http://hz.yanxiufei.cn/gtzkazircl.html

--------------------------------------------------------------------------------
来源：http://hz.jianghu66.top/gtipftigca.html

使用提醒
来源：http://hz.mhx1999.top/gtynwiuvai.html

--------------------------------------------------------------------------------
来源：http://hz.snrcjt.cn/gtyjecoevq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.hysaishi.cn/gtkezcmvzq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.daxiang520.top/gtnhyqilvl.html


<!-- 参考信息 -->