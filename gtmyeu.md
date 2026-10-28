代发 wailian999

[U01] Py：创建虚拟环境
来源：http://hz.sweek.top/gtwusropva.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xinyue.icu/gtmxozrhgr.html

[U02] Py：导出 / 安装依赖
来源：http://hz.svipenyu.cn/gtqvamvrkk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zycfv.cn/gtefappdfm.html

[U03] Py：加载 .env 配置
来源：http://hz.jiagoushi.top/gtostnesmi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.meibo888.top/gteckxatyi.html

[U04] Py：变量调试打印
来源：http://hz.jinqigfzy.top/gtnxzfejlt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhiwuduotai.top/gtncnlbbuo.html

[U05] Py：列表去重且保序
来源：http://hz.yuanzhike.top/gtmiuiunjs.html

list(dict.fromkeys(arr))
来源：http://hz.kuanghao11.cn/gttfadoecc.html

[U06] Py：合并两个字典
来源：http://hz.pengpengdd.cyou/gtlzoxtetr.html

{**a, **b}
来源：http://hz.ehwqpu.com/gtjcirkosy.html

[U07] Py：反转字典键值
来源：http://hz.cheryme.top/gtxzcluilz.html

{v: k for k, v in d.items()}
来源：http://hz.sxryk.cn/gtzmwipsmt.html

[U08] Py：展平二维列表
来源：http://hz.haohaochexian.top/gtkalpzrvl.html

[y for x in nested for y in x]
来源：http://hz.dianchejie.cn/gtsuspnaoe.html

[U09] Py：字典取最大值的键
来源：http://hz.jiagoushi.top/gtsdohdncd.html

max(d, key=d.get)
来源：http://hz.guowangkeji.top/gtvephswab.html

[U10] Py：按值排序字典
来源：http://hz.yangfankeji.com/gtpcmmehxl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cdnleiting.top/gtaghewymg.html

[U11] Py：生成器表达式
来源：http://hz.shuidangran.top/gtqgmcyfxo.html

(x * 2 for x in arr)
来源：http://hz.ydzc1.top/gtkvjmgcoz.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.redwolf501.top/gtebjoztfz.html

Counter(arr).most_common(3)
来源：http://hz.yj202588.top/gtzlndpvgb.html

[U13] Py：固定长度队列
来源：http://hz.shanyushiyangkeji.top/gthuszlibz.html

deque(maxlen=10)
来源：http://hz.zhengqikj.top/gtolyaaxhi.html

[U14] Py：分组收集到列表
来源：http://hz.dianchejie.cn/gtjdxtbtnl.html

defaultdict(list)
来源：http://hz.cucudq.cn/gtofirfgae.html

[U15] Py：高精度计时
来源：http://hz.zhoulong.xyz/gtwctjocii.html

t = time.perf_counter()
来源：http://hz.yuxming.cn/gttcdonwyx.html

[U16] Py：命令行参数解析
来源：http://hz.sweek.top/gtzaokuvnv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yj20258888.top/gtjjrabnzw.html

[U17] Py：初始化日志
来源：http://hz.aibaodan.cn/gtzhbksddm.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.smart0.xyz/gtpajoyswo.html

[U18] Py：预编译正则
来源：http://hz.dianchejie.cn/gtmkyrvfjn.html

pat = re.compile(r"\d+")
来源：http://hz.ivvv.top/gthlgpdmii.html

[U19] Py：正则替换带回调
来源：http://hz.jqgfzy.top/gtdupcjteq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.c1oappe.top/gtbetelgks.html

[U20] Py：缓存函数结果
来源：http://hz.birdmap.top/gtpbkovlhl.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shuidangran.top/gtsnvksyji.html

[U21] Py：自定义上下文管理器
来源：http://hz.guowangkeji.top/gtqxcbmawh.html

@contextlib.contextmanager
来源：http://hz.bjfxy.top/gtjcwgqtli.html

[U22] Py：矩阵转置
来源：http://hz.zhaomingkeji.xyz/gtudcumxio.html

list(zip(*m))
来源：http://hz.sxryk.cn/gtzymjyvsz.html

[U23] Py：分块读取大文件
来源：http://hz.vqdsnc.cn/gtoeyrclsk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.gogol.net.cn/gtqgykbxdv.html

[U24] Py：路径操作
来源：http://hz.ivvv.top/gtglvlclar.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.feifeiyinyue.top/gtnyieymap.html

[U25] Py：CSV 按字典读
来源：http://hz.yongpay.top/gteivpxyut.html

csv.DictReader(f)
来源：http://hz.jinqigufen.top/gtqsvhlxhc.html

[U26] Py：并发下载
来源：http://hz.tian-w.cn/gtuneanbym.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.nwbrower.top/gtotmvldvv.html

[U27] Py：异步 HTTP
来源：http://hz.sysykeji.top/gtsbqxrhau.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.tianlin.xyz/gtsesucsot.html

[U28] Py：类型别名
来源：http://hz.yueranfly.top/gtmgcxiweh.html

UserId = int
来源：http://hz.jyoumei.cn/gtiwhxgfbp.html

[U29] Py：属性校验
来源：http://hz.shanyushiyangkeji.top/gtwhytakfa.html

@property 与 @x.setter 配合
来源：http://hz.iojbl.cn/gtfvizwnip.html

[U30] Py：数据类
来源：http://hz.yvedp.cn/gthrgvnwxx.html

@dataclass(slots=True)
来源：http://hz.zhijiandao.cn/gtapevizho.html

[U31] Py：单测
来源：http://hz.hnqzz.top/gtiygwmbwq.html

python -m pytest -q
来源：http://hz.sweek.top/gtdqfhnqnn.html

[U32] Py：代码格式化
来源：http://hz.chenjidiqi.icu/gtiljdzqqh.html

ruff format . && ruff check --fix .
来源：http://hz.hnxiangtu.top/gtwhfyccjm.html

[U33] Py：打包发布
来源：http://hz.cdnleiting.top/gttsywpmmy.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yonumen.top/gtqotglbss.html

[U34] Py：判断编码
来源：http://hz.kuanghao11.cn/gtnbayavdv.html

chardet.detect(raw)
来源：http://hz.vqdsnc.cn/gtpxtaytwd.html

[U35] Py：发送邮件
来源：http://hz.xuetiantiany.cn/gtuywjheac.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.hnqzz.top/gtsbtymuwp.html

[U36] Py：定时任务
来源：http://hz.nwbrower.top/gtdrcqtbxe.html

schedule.every(10).minutes.do(job)
来源：http://hz.hywenlv.cn/gtqitsxqhv.html

[U37] Py：读写 Excel
来源：http://hz.wangshuangyany.cn/gtixauiszd.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jqgufenzy.top/gtjhaqbnma.html

[U38] Py：获取脚本所在目录
来源：http://hz.cucudq.cn/gtucvuqclt.html

Path(__file__).resolve().parent
来源：http://hz.pengpengdd.cyou/gtrbmvfely.html

[U39] Py：判断是否在交互环境
来源：http://hz.ywan-chungtsiang.top/gtpgbdhart.html

sys.stdout.isatty()
来源：http://hz.birdmap.top/gtdkdafykr.html

[U40] Py：打印到标准错误
来源：http://hz.yvedp.cn/gtbyolupua.html

print("err", file=sys.stderr)
来源：http://hz.dianchejie.cn/gttuuwdcjr.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.shanyushiyangtech.top/gtmktupeph.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhongyouzk.top/gtojaybbvh.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhijiandao.cn/gtkprydhut.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jinqigufen.top/gthlgiikxw.html

[U43] PHP：声明命名空间
来源：http://hz.zhixingplan.top/gtfeggbibg.html

namespace App\Http;
来源：http://hz.jiagoushi.top/gtqwqrcrqg.html

[U44] PHP：开启严格类型
来源：http://hz.xingfuxueyuan.xyz/gtjmvdpeih.html

declare(strict_types=1);
来源：http://hz.chenjidiqi.icu/gtxkieabia.html

[U45] PHP：类型声明与返回类型
来源：http://hz.nanxinkj.top/gtomhmycze.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhiwuduotai.top/gtqhfsnfkd.html

[U46] PHP：可空类型
来源：http://hz.hnqzz.top/gtkgehtoab.html

?string $name = null
来源：http://hz.haohaochexian.top/gtseyzcgzf.html

[U47] PHP：联合类型
来源：http://hz.wangshuangyany.cn/gtdoruyfja.html

int|string $id
来源：http://hz.ybcxt.top/gtwhustqus.html

[U48] PHP：纯枚举
来源：http://hz.xingfuxueyuan.xyz/gtgnpmettc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.feifeiyinyue.top/gtqhbhirqo.html

[U49] PHP：只读属性
来源：http://hz.zhoulong.xyz/gtaochavto.html

public readonly string $name
来源：http://hz.9152youxi.cn/gtmqkgmrsa.html

[U50] PHP：构造器属性提升
来源：http://hz.jinqigufen.top/gtciztofqb.html

public function __construct(private int $id) {}
来源：http://hz.ivvv.top/gtvxdfjyzk.html

[U51] PHP：数组解构
来源：http://hz.cashguo.top/gtyltsiqzb.html

[$a, $b] = $arr;
来源：http://hz.shangyingyoupin.top/gtemzhxyaj.html

[U52] PHP：箭头函数
来源：http://hz.chenjidiqi.icu/gtbsknvjsb.html

$double = fn($x) => $x * 2;
来源：http://hz.jiagoushi.top/gtpolpsbwy.html

[U53] PHP：空合并运算符
来源：http://hz.birdmap.top/gthxkarhaq.html

$v = $a ?? $b ?? "default";
来源：http://hz.xuetiantiany.cn/gttqybctrw.html

[U54] PHP：空安全调用
来源：http://hz.vqdsnc.cn/gtypjaoige.html

$obj?->method()
来源：http://hz.ydjk.org.cn/gtioissuxy.html

[U55] PHP：match 表达式
来源：http://hz.zhaomingkeji.xyz/gtvtyuflkj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.xinyue.icu/gtujrurhgb.html

[U56] PHP：命名参数
来源：http://hz.jqgufenzy.top/gtqkfmdavh.html

f(a: 1, b: 2)
来源：http://hz.dashuyun.cn/gtnbhqotdt.html

[U57] PHP：字符串插值
来源：http://hz.svipenyu.cn/gtkygdozrf.html

"值: {$a}"
来源：http://hz.zhaomingkeji.xyz/gtnnojburk.html

[U58] PHP：数组三件套
来源：http://hz.tanke756.top/gtmecrkjai.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hongshengwenyu.top/gtgacutuxc.html

[U59] PHP：自定义排序
来源：http://hz.9152youxi.cn/gtckqszkov.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.wangdashe.top/gtwbyfruah.html

[U60] PHP：JSON 编解码
来源：http://hz.zhiwuduotai.top/gtcddickep.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.guowangkeji.top/gtbxvkitrv.html

[U61] PHP：正则
来源：http://hz.chenlongwang.top/gtxnzliijh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jyoumei.cn/gtsgewhmmp.html

[U62] PHP：日期对象
来源：http://hz.chenlongwang.top/gtmceyjygo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.pengpengdd.cyou/gthosmfbzy.html

[U63] PHP：文件读写
来源：http://hz.hnxiangtu.top/gtigvkuqqw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.c1oappe.top/gtoopzrbsz.html

[U64] PHP：目录遍历
来源：http://hz.daxiang520.top/gtuehwejfb.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hammf.cn/gtjebytsya.html

[U65] PHP：会话
来源：http://hz.jlsjyb.cn/gtnbqfhlzd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.smart0.xyz/gtbmvuratb.html

[U66] PHP：设置 Cookie
来源：http://hz.9152youxi.cn/gtqtqgpjxs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.52xcode.cn/gtselydktk.html

[U67] PHP：处理文件上传
来源：http://hz.xingfuxueyuan.xyz/gtqulgjlzq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.gogol.net.cn/gtnmpmserw.html

[U68] PHP：PDO 连接
来源：http://hz.xinyue.icu/gtugriitxw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xziqi.cn/gthlzvpmua.html

[U69] PHP：PDO 预处理
来源：http://hz.pengpengdd.cyou/gtfeslbqhf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hammf.cn/gtikzagbws.html

[U70] PHP：PDO 事务
来源：http://hz.xuetiantiany.cn/gtvkikntld.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jqgfzy.top/gtsokanwhx.html

[U71] PHP：抛出异常
来源：http://hz.guowangkeji.top/gtmcplgvjk.html

throw new RuntimeException("失败", 500);
来源：http://hz.0kj1m.cn/gtduzkzrea.html

[U72] PHP：写错误日志
来源：http://hz.yonumen.top/gtkidiefge.html

error_log("失败: " . $e->getMessage());
来源：http://hz.316326.xyz/gttmgaegel.html

[U73] PHP：读取 ini 配置
来源：http://hz.redwolf501.top/gtnqyrlbuq.html

parse_ini_file("config.ini", true)
来源：http://hz.daxiang520.top/gtlotmfqgz.html

[U74] PHP：读取环境变量
来源：http://hz.yj202588.top/gtpgoewqhr.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jinghuilouyu.cn/gtnrnupcvs.html

[U75] PHP：依赖注入
来源：http://hz.jianghu66.top/gtyamjkxgj.html

composer require psr/container
来源：http://hz.daxiang520.top/gtvlgwqfoq.html

[U76] PHP：简单路由
来源：http://hz.yj20258888.top/gtgvgzbpib.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.tianlin.xyz/gtpjipupkj.html

[U77] PHP：模板渲染
来源：http://hz.xuetiantiany.cn/gtkvezplnb.html

composer require twig/twig
来源：http://hz.wangshuangyany.cn/gtrczoqhgb.html

[U78] PHP：单元测试
来源：http://hz.guowangkeji.top/gtafiprucj.html

composer require --dev phpunit/phpunit
来源：http://hz.wangdashe.top/gtcdebsnac.html

[U79] PHP：静态分析
来源：http://hz.hywenlv.cn/gtmnnqabiz.html

composer require --dev phpstan/phpstan
来源：http://hz.xingfuxueyuan.xyz/gtyfalpzev.html

[U80] PHP：代码规范修复
来源：http://hz.shangyingyoupin.top/gtudajbgez.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.gogol.net.cn/gtgobwxnem.html

[U81] JS：初始化项目
来源：http://hz.smart0.xyz/gthggkrapb.html

npm init -y;  npm i express
来源：http://hz.0kj1m.cn/gtboxvcinf.html

[U82] JS：package.json 脚本
来源：http://hz.zdqjudy.top/gtxervilzh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.gaohongyu789.top/gtfgwscqyo.html

[U83] JS：ES Module 导入导出
来源：http://hz.cqqwz.cn/gtjcrzqgdt.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.chenjidiqi.icu/gtgdzfrixn.html

[U84] JS：CommonJS 写法
来源：http://hz.yuxming.cn/gtjyqgsobe.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zhengqikj.top/gtvshmymnx.html

[U85] JS：可选链
来源：http://hz.ehwqpu.com/gtpoqjzpdw.html

a?.b?.c
来源：http://hz.zhengqikj.top/gttmauhmje.html

[U86] JS：空值合并
来源：http://hz.hongshengwenyu.top/gtrttoufma.html

a ?? b
来源：http://hz.shangyingyoupin.top/gthbgcxsdf.html

[U87] JS：解构默认值
来源：http://hz.ppjwa.cn/gtpatlezup.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yonumen.top/gtscdmfkrq.html

[U88] JS：对象展开合并
来源：http://hz.jinghuilouyu.cn/gtayywojds.html

{ ...a, ...b }
来源：http://hz.hfpthk.cn/gtardqfpnz.html

[U89] JS：数组去重
来源：http://hz.jlsjyb.cn/gtzgvxisfy.html

[...new Set(arr)]
来源：http://hz.zdqjudy.top/gtwjabdsqn.html

[U90] JS：数字数组排序
来源：http://hz.quarkkingdee.top/gtuoblddhk.html

[...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gtazagwqgg.html

[U91] JS：对象键值遍历
来源：http://hz.daxiang520.top/gtccyurdyn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.9152youxi.cn/gtafyesqvk.html

[U92] JS：深拷贝
来源：http://hz.snrcjt.cn/gtsvqaogem.html

structuredClone(obj)
来源：http://hz.aibaodan.cn/gtnzmipadf.html

[U93] JS：模板字符串
来源：http://hz.hysaishi.cn/gtjwzhgvve.html

`共 ${n} 条`
来源：http://hz.tanke756.top/gtzqrvsfyx.html

[U94] JS：箭头函数
来源：http://hz.andypj.xyz/gtqcoqmjvr.html

const double = x => x * 2;
来源：http://hz.yanxiufei.cn/gtwqlsqgun.html

[U95] JS：Promise 包装
来源：http://hz.zhijiandao.cn/gtcwsiqljq.html

new Promise((resolve, reject) => {})
来源：http://hz.zhongyouzk.top/gtxhqgirnj.html

[U96] JS：async/await 与异常
来源：http://hz.kuanghao11.cn/gtglzyurhl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.hnqzz.top/gtxeaoayvq.html

[U97] JS：并发请求
来源：http://hz.tanke756.top/gtexksuxrn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gtackvemqx.html

[U98] JS：fetch 带 JSON
来源：http://hz.haohaochexian.top/gtwausxbzc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.andypj.xyz/gtqoqneitz.html

[U99] JS：事件监听
来源：http://hz.yangfankeji.com/gtmmksxzhr.html

el.addEventListener("click", e => {})
来源：http://hz.zhijiandao.cn/gtgrwaqehz.html

[U100] JS：DOM 查询
来源：http://hz.zdqjudy.top/gtrgrwsnqn.html

document.querySelector(".item")
来源：http://hz.pycfn.com/gtggmanzms.html

[U101] JS：classList 操作
来源：http://hz.smart0.xyz/gtnnfcdqmg.html

el.classList.toggle("active")
来源：http://hz.zhoulong.xyz/gttaalbzwf.html

[U102] JS：本地存储
来源：http://hz.yanxiufei.cn/gtapglonej.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yuanzhike.top/gtlkbfpupv.html

[U103] JS：定时器
来源：http://hz.ehwqpu.com/gttoalqjhh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hnxiangtu.top/gtzrbdarzb.html

[U104] JS：防抖
来源：http://hz.sweek.top/gtagiakfvb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.316326.xyz/gthaswzbot.html

[U105] JS：节流
来源：http://hz.smart0.xyz/gthlcvcepa.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.fzhhl.top/gtlwynlbbr.html

[U106] JS：日期格式化
来源：http://hz.yj20258.top/gtulvxygca.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yanxiufei.cn/gttmosizfs.html

[U107] JS：数字千分位
来源：http://hz.jlsjyb.cn/gtqdnagmlo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.shzxlz.cn/gtgiwhqurn.html

[U108] JS：随机整数
来源：http://hz.guannengcc.top/gtqchfwabb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.nanxinkj.top/gtcxxpuyvn.html

[U109] JS：数组分组
来源：http://hz.zhongyouzk.top/gtgmwaakfe.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yonumen.top/gtmgwzinji.html

[U110] JS：数组分块
来源：http://hz.zhixingplan.top/gtifzhoqje.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.chenlongwang.top/gtgdsktmgj.html

[U111] JS：对象转 Map
来源：http://hz.jlsjyb.cn/gtyuzgmdgi.html

new Map(Object.entries(obj))
来源：http://hz.chenlongwang.top/gtxjxsvrdw.html

[U112] JS：字符串补位
来源：http://hz.xuetiantiany.cn/gtbjfgemyu.html

"7".padStart(3, "0")
来源：http://hz.shanyushiyangkeji.top/gtjxmprdgo.html

[U113] JS：正则替换全部
来源：http://hz.sweek.top/gtnwcgeigu.html

s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtyxxwgflb.html

[U114] JS：JSON 深比较
来源：http://hz.snrcjt.cn/gtstdihahh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zdqjudy.top/gtnkhdysee.html

[U115] JS：生成 UUID
来源：http://hz.mhx1999.top/gthbvsbgbe.html

crypto.randomUUID()
来源：http://hz.zhijiandao.cn/gtgfixlpxx.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.wangdashe.top/gtgbimqzgc.html

/** @param {string} name */ function f(name) {}
来源：http://hz.52xcode.cn/gtankyisyn.html

[U117] JS：单元测试
来源：http://hz.sufxvd.cn/gtzhoidxdy.html

npm i -D vitest;  npx vitest
来源：http://hz.chenjidiqi.icu/gttjnvkcfm.html

[U118] JS：开发服务器
来源：http://hz.guannengcc.top/gtdvwztesw.html

npm i -D vite;  npx vite
来源：http://hz.zhijiandao.cn/gteqpsbery.html

[U119] JS：生产构建
来源：http://hz.chenjidiqi.icu/gtysxzgkyh.html

npx vite build
来源：http://hz.yueranfly.top/gtxkozbuxm.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.chenjidiqi.icu/gtfrvhvwkd.html

import.meta.env.VITE_API_URL
来源：http://hz.aibaodan.cn/gtemgvfuxq.html

================================================================================
来源：http://hz.haohaochexian.top/gtndgbnrqv.html

统计汇总
来源：http://hz.hammf.cn/gthslfwuzn.html

================================================================================
来源：http://hz.ppjwa.cn/gtklmoqaqg.html

按语言统计（条）：
来源：http://hz.zhongyouzk.top/gtvjhvnddq.html

Python ......... 252
来源：http://hz.hnqzz.top/gtutmzoifv.html

PHP ............ 252
来源：http://hz.aibaodan.cn/gtiiifqfmm.html

JavaScript ..... 252
来源：http://hz.shangyingyoupin.top/gtrbygsfhc.html

TypeScript ..... 212
来源：http://hz.zhengqikj.top/gtkehfjidy.html

Java ........... 212
来源：http://hz.zhijiandao.cn/gtrnnjolzw.html

Go ............. 212
来源：http://hz.tian-w.cn/gtysbudvkl.html

Ruby ........... 212
来源：http://hz.feifeiyinyue.top/gtttywuzhn.html

C# ............. 212
来源：http://hz.zhengqikj.top/gtugxroahw.html

C .............. 30
来源：http://hz.iojbl.cn/gtingdjaoj.html

C++ ............ 30
来源：http://hz.zhengqikj.top/gtkgafsdij.html

SQL ............ 90
来源：http://hz.yj202588.top/gthmwvbwrg.html

Bash ........... 80
来源：http://hz.daria6918.cn/gtuozfztmw.html

Kotlin ......... 15
来源：http://hz.redwolf501.top/gtfoxfjqay.html

Swift .......... 15
来源：http://hz.jqgfzy.top/gtnmmymbdb.html

Lua ............ 10
来源：http://hz.jlsjyb.cn/gtnyritcae.html

Perl ........... 10
来源：http://hz.dashuyun.cn/gtjssbywyv.html

Scala .......... 10
来源：http://hz.kuanghao11.cn/gtkrhhgpnb.html

------------------------------------
来源：http://hz.aibaodan.cn/gtccefzbqe.html

合计 ........... 2106 条
来源：http://hz.zhijiandao.cn/gtmlszagen.html

按章节统计：
来源：http://hz.c1oappe.top/gtajjxpjhr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.iojbl.cn/gttxvlqqrz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.chenlongwang.top/gtgvksliag.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.wangdashe.top/gtqevevjry.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.andypj.xyz/gtlrtvbqcx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.snrcjt.cn/gtdcakopan.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.guannengcc.top/gtwwwnofof.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.smart0.xyz/gtwzsdyuaj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.wangdashe.top/gtavgwboyx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.ywan-chungtsiang.top/gtdknalzxx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yj202588.top/gtdmsbnyun.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.chenjidiqi.icu/gtppxjluka.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.cdnleiting.top/gtggbzzexb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.feifeiyinyue.top/gtlxzekkwo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jinqigufen.top/gtvhirlyce.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jlsjyb.cn/gtafmtpkuq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yueranfly.top/gtsbiszadc.html

Q SQL 专题                              90
来源：http://hz.havefunace.top/gtdiyggysj.html

R Bash 专题                             80
来源：http://hz.tian-w.cn/gtdqmsezce.html

S C / C++ 专题                          60
来源：http://hz.tian-w.cn/gtvmgysajc.html

T 其他语言补充                          60
来源：http://hz.jqgufenzy.top/gtivmogvhj.html

U 高频实用片段                         120
来源：http://hz.yuxming.cn/gtyfugzpum.html

------------------------------------
来源：http://hz.mhx1999.top/gtqnblegrb.html

合计                                  2106 条
来源：http://hz.ybcxt.top/gtuqwqnwpp.html

--------------------------------------------------------------------------------
来源：http://hz.zhixingplan.top/gtncmfqofw.html

使用提醒
来源：http://hz.havefunace.top/gtoieshbgv.html

--------------------------------------------------------------------------------
来源：http://hz.jyoumei.cn/gtkoqlockb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.sysykeji.top/gtmxhqtmar.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.dianchejie.cn/gtbzcakfgq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zhongyouzk.top/gtlwyhminq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.cqqwz.cn/gtxaiezlzc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.hongshengwenyu.top/gtptxhbcuj.html

—— 文件结束 ——
来源：http://hz.gotoacloud.top/gtipgbzwjw.html

================================================================================
来源：http://hz.gzhubu.top/gtinkjkvnz.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yangfankeji.com/gtsersjmpo.html

Common Programming Examples Cheat Book
来源：http://hz.gogol.net.cn/gtnzplyrci.html

================================================================================
来源：http://hz.gogol.net.cn/gtxuyzdvkl.html


<!-- 参考信息 -->