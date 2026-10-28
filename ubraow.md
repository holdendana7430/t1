代发 wailian999

[U01] Py：创建虚拟环境
来源：http://hz.fengsongda.top/gtfubkcaud.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.quarkkingdee.top/gtffiucsoz.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yj202588.top/gtgoiinstj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jyoumei.cn/gtaairytap.html

[U03] Py：加载 .env 配置
来源：http://hz.kuanghao11.cn/gtiburhyhn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.haohaochexian.top/gtbzpfqybv.html

[U04] Py：变量调试打印
来源：http://hz.tian-w.cn/gtauglijjl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.tianlin.xyz/gtytcrcxao.html

[U05] Py：列表去重且保序
来源：http://hz.zhijiandao.cn/gtbawwccgk.html

list(dict.fromkeys(arr))
来源：http://hz.iojbl.cn/gtabybodpd.html

[U06] Py：合并两个字典
来源：http://hz.tanke756.top/gtjsndlbce.html

{**a, **b}
来源：http://hz.svipenyu.cn/gtpyqulodk.html

[U07] Py：反转字典键值
来源：http://hz.nanxinkj.top/gtaitkdsis.html

{v: k for k, v in d.items()}
来源：http://hz.ywan-chungtsiang.top/gtarzvblnd.html

[U08] Py：展平二维列表
来源：http://hz.jinghuilouyu.cn/gtczvsgyku.html

[y for x in nested for y in x]
来源：http://hz.bjfxy.top/gtgwfdyida.html

[U09] Py：字典取最大值的键
来源：http://hz.yanxiufei.cn/gtpuqnaxnr.html

max(d, key=d.get)
来源：http://hz.bjfxy.top/gtykmdwqwp.html

[U10] Py：按值排序字典
来源：http://hz.zhiwuduotai.top/gtidftgxpp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.9152youxi.cn/gttgynjiag.html

[U11] Py：生成器表达式
来源：http://hz.gotoacloud.top/gtjstgfgke.html

(x * 2 for x in arr)
来源：http://hz.0kj1m.cn/gthancsfho.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jinqigfzy.top/gtmeqogwwd.html

Counter(arr).most_common(3)
来源：http://hz.andypj.xyz/gtcuqwtdcd.html

[U13] Py：固定长度队列
来源：http://hz.wangshuangyany.cn/gtvatlnqvy.html

deque(maxlen=10)
来源：http://hz.yuxming.cn/gtqcvuyuff.html

[U14] Py：分组收集到列表
来源：http://hz.dianchejie.cn/gtemmahaez.html

defaultdict(list)
来源：http://hz.mhx1999.top/gttpuqpjbc.html

[U15] Py：高精度计时
来源：http://hz.redwolf501.top/gtqtdfgoro.html

t = time.perf_counter()
来源：http://hz.jlsjyb.cn/gtznlkokeg.html

[U16] Py：命令行参数解析
来源：http://hz.gotoacloud.top/gtxdcnkiju.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.shzxlz.cn/gtapmqekvn.html

[U17] Py：初始化日志
来源：http://hz.svipenyu.cn/gtmqnnjbzv.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yonumen.top/gttgtsmdvm.html

[U18] Py：预编译正则
来源：http://hz.zycfv.cn/gtvsxfgcpc.html

pat = re.compile(r"\d+")
来源：http://hz.shuidangran.top/gtjjmzagaq.html

[U19] Py：正则替换带回调
来源：http://hz.nwbrower.top/gtclnoyaty.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.andypj.xyz/gtvdukkooo.html

[U20] Py：缓存函数结果
来源：http://hz.dianchejie.cn/gtsjammgyk.html

@functools.lru_cache(maxsize=None)
来源：http://hz.wangshuangyany.cn/gtpnkqniwt.html

[U21] Py：自定义上下文管理器
来源：http://hz.guowangkeji.top/gtfttcnvkd.html

@contextlib.contextmanager
来源：http://hz.gaohongyu789.top/gtwbiaezdd.html

[U22] Py：矩阵转置
来源：http://hz.jlsjyb.cn/gticoestbw.html

list(zip(*m))
来源：http://hz.sysykeji.top/gtcggpjosx.html

[U23] Py：分块读取大文件
来源：http://hz.xylfe.cn/gtwyqxytnp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zhixingplan.top/gtuparmwan.html

[U24] Py：路径操作
来源：http://hz.ivvv.top/gtenokwmtx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.shangyingyoupin.top/gtomozbhlw.html

[U25] Py：CSV 按字典读
来源：http://hz.jinqigfzy.top/gtpdakzzjx.html

csv.DictReader(f)
来源：http://hz.hammf.cn/gtntvxgpzp.html

[U26] Py：并发下载
来源：http://hz.chenjidiqi.icu/gtlzjbykwx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hysaishi.cn/gtevftjzti.html

[U27] Py：异步 HTTP
来源：http://hz.zhiwuduotai.top/gtgfwrkzqh.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.wangdashe.top/gtrortjfuj.html

[U28] Py：类型别名
来源：http://hz.nanxuanxn.top/gtdfddrnle.html

UserId = int
来源：http://hz.316326.xyz/gtaadwdtlr.html

[U29] Py：属性校验
来源：http://hz.dashuyun.cn/gtujuphtdg.html

@property 与 @x.setter 配合
来源：http://hz.haohaochexian.top/gtbreabopv.html

[U30] Py：数据类
来源：http://hz.tanke756.top/gtsppvhoyl.html

@dataclass(slots=True)
来源：http://hz.haohaochexian.top/gtqhspbsml.html

[U31] Py：单测
来源：http://hz.gaohongyu789.top/gthkeamlee.html

python -m pytest -q
来源：http://hz.chenjidiqi.icu/gtyiqbgewk.html

[U32] Py：代码格式化
来源：http://hz.havefunace.top/gtmreyexap.html

ruff format . && ruff check --fix .
来源：http://hz.snrcjt.cn/gtvuxyofak.html

[U33] Py：打包发布
来源：http://hz.ivvv.top/gtaxybqdfb.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hywenlv.cn/gtehpgjzvi.html

[U34] Py：判断编码
来源：http://hz.aizwys.cn/gtaxeznqyy.html

chardet.detect(raw)
来源：http://hz.jinqigfzy.top/gtcyzpvdse.html

[U35] Py：发送邮件
来源：http://hz.sysykeji.top/gtkgfufcmg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.sysykeji.top/gtvoblcxyz.html

[U36] Py：定时任务
来源：http://hz.tian-w.cn/gtmzdnrbvm.html

schedule.every(10).minutes.do(job)
来源：http://hz.gogol.net.cn/gtufqxnhpp.html

[U37] Py：读写 Excel
来源：http://hz.shangyingyoupin.top/gttwjtpvve.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ywan-chungtsiang.top/gtumyagbwm.html

[U38] Py：获取脚本所在目录
来源：http://hz.quarkkingdee.top/gtmxapvddo.html

Path(__file__).resolve().parent
来源：http://hz.chenlongwang.top/gttnmjxczc.html

[U39] Py：判断是否在交互环境
来源：http://hz.ppjwa.cn/gttnmnvbhl.html

sys.stdout.isatty()
来源：http://hz.iojbl.cn/gtcbeepkns.html

[U40] Py：打印到标准错误
来源：http://hz.ybcxt.top/gtciuhnprv.html

print("err", file=sys.stderr)
来源：http://hz.xinyue.icu/gtreiklfhr.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.hnqzz.top/gtucmrwpzo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhoulong.xyz/gtnvszycps.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.gaohongyu789.top/gtcyvxratf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ppjwa.cn/gtxrifibuc.html

[U43] PHP：声明命名空间
来源：http://hz.hysaishi.cn/gtuixdktnp.html

namespace App\Http;
来源：http://hz.svipenyu.cn/gtvmxewuox.html

[U44] PHP：开启严格类型
来源：http://hz.cucudq.cn/gtnrsimynl.html

declare(strict_types=1);
来源：http://hz.vqdsnc.cn/gtnqsepajq.html

[U45] PHP：类型声明与返回类型
来源：http://hz.dashuyun.cn/gtdlfpbwjz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pycfn.com/gtdnpbtngr.html

[U46] PHP：可空类型
来源：http://hz.zdqjudy.top/gtijawnhyx.html

?string $name = null
来源：http://hz.cucudq.cn/gtfzgbmmww.html

[U47] PHP：联合类型
来源：http://hz.shzxlz.cn/gtjzdfocno.html

int|string $id
来源：http://hz.sweek.top/gtynzntdou.html

[U48] PHP：纯枚举
来源：http://hz.snrcjt.cn/gtgbkujqkv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.daxiang520.top/gtzzqoatsb.html

[U49] PHP：只读属性
来源：http://hz.316326.xyz/gtspxgyyak.html

public readonly string $name
来源：http://hz.jqgfzy.top/gtlfzgiwzl.html

[U50] PHP：构造器属性提升
来源：http://hz.andypj.xyz/gtymoamwsw.html

public function __construct(private int $id) {}
来源：http://hz.vqdsnc.cn/gtgwpagzkr.html

[U51] PHP：数组解构
来源：http://hz.birdmap.top/gtiritariv.html

[$a, $b] = $arr;
来源：http://hz.ivvv.top/gtasazlllp.html

[U52] PHP：箭头函数
来源：http://hz.shanyushiyangkeji.top/gtcdlvghyj.html

$double = fn($x) => $x * 2;
来源：http://hz.52xcode.cn/gtjbcsoqpg.html

[U53] PHP：空合并运算符
来源：http://hz.xylfe.cn/gtigdpndem.html

$v = $a ?? $b ?? "default";
来源：http://hz.316326.xyz/gtyfexysau.html

[U54] PHP：空安全调用
来源：http://hz.c1oappe.top/gthnskrgta.html

$obj?->method()
来源：http://hz.xuetiantiany.cn/gtpzsbbtmy.html

[U55] PHP：match 表达式
来源：http://hz.jinqigfzy.top/gtnqaxmpom.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.hammf.cn/gtwhkwaekv.html

[U56] PHP：命名参数
来源：http://hz.yj202588.top/gtgynuroso.html

f(a: 1, b: 2)
来源：http://hz.aizwys.cn/gtqpxkiqxo.html

[U57] PHP：字符串插值
来源：http://hz.bjfxy.top/gtjdiwqvlv.html

"值: {$a}"
来源：http://hz.yonumen.top/gtomjjsdhg.html

[U58] PHP：数组三件套
来源：http://hz.zhongyouzk.top/gtrqzeglxq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.xziqi.cn/gtgorvdftr.html

[U59] PHP：自定义排序
来源：http://hz.hongshengwenyu.top/gtxvyjnmpo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jlsjyb.cn/gtxcbetneb.html

[U60] PHP：JSON 编解码
来源：http://hz.shangyingyoupin.top/gtsoteblhg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.shangyingyoupin.top/gtjytzssbb.html

[U61] PHP：正则
来源：http://hz.kuanghao11.cn/gtiotegglc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj202588.top/gtjjioudyy.html

[U62] PHP：日期对象
来源：http://hz.cdnleiting.top/gtmmqybqcn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.aibaodan.cn/gtqcwasfqa.html

[U63] PHP：文件读写
来源：http://hz.shanyushiyangkeji.top/gtpcvdiuml.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.ydzc1.top/gtvqcvldcl.html

[U64] PHP：目录遍历
来源：http://hz.yanxiufei.cn/gtviclvapn.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.chenzaomai.com/gtahpdtstk.html

[U65] PHP：会话
来源：http://hz.nanxuanxn.top/gtcnhvmpsi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.xuetiantiany.cn/gtvahpbmxe.html

[U66] PHP：设置 Cookie
来源：http://hz.jinyuanbaomall.cn/gtefsdpmuc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhengqikj.top/gtllbtvmby.html

[U67] PHP：处理文件上传
来源：http://hz.52xcode.cn/gteypifwfj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.mhx1999.top/gtdrizpbco.html

[U68] PHP：PDO 连接
来源：http://hz.snrcjt.cn/gtzionggna.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.fengsongda.top/gtmmucdoez.html

[U69] PHP：PDO 预处理
来源：http://hz.yueranfly.top/gtzhweubpp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jianghu66.top/gtlzunletp.html

[U70] PHP：PDO 事务
来源：http://hz.jinqigufen.top/gtgktlcoxk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.cashguo.top/gtvixailjw.html

[U71] PHP：抛出异常
来源：http://hz.andypj.xyz/gtkgamqbsx.html

throw new RuntimeException("失败", 500);
来源：http://hz.yanxiufei.cn/gtrrbdycnx.html

[U72] PHP：写错误日志
来源：http://hz.hfpthk.cn/gtplxtpurl.html

error_log("失败: " . $e->getMessage());
来源：http://hz.shanyushiyangtech.top/gtmhwefrvg.html

[U73] PHP：读取 ini 配置
来源：http://hz.xylfe.cn/gtrzzvnbvf.html

parse_ini_file("config.ini", true)
来源：http://hz.ivvv.top/gtmtumcbiv.html

[U74] PHP：读取环境变量
来源：http://hz.hammf.cn/gtipmfvitw.html

getenv("APP_ENV") ?: "production"
来源：http://hz.svipenyu.cn/gtjxlngdcn.html

[U75] PHP：依赖注入
来源：http://hz.hywenlv.cn/gtzvylzrny.html

composer require psr/container
来源：http://hz.pycfn.com/gtciwrnlgy.html

[U76] PHP：简单路由
来源：http://hz.yuxming.cn/gtrogmoauh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hongshengwenyu.top/gtzrwyhyja.html

[U77] PHP：模板渲染
来源：http://hz.dashuyun.cn/gtkmxjpffx.html

composer require twig/twig
来源：http://hz.birdmap.top/gttqqugbch.html

[U78] PHP：单元测试
来源：http://hz.pengpengdd.cyou/gtwtakqgdk.html

composer require --dev phpunit/phpunit
来源：http://hz.xuanzx.com/gtiubbswkb.html

[U79] PHP：静态分析
来源：http://hz.guowangkeji.top/gtubzhrfys.html

composer require --dev phpstan/phpstan
来源：http://hz.hnqzz.top/gtomxjartu.html

[U80] PHP：代码规范修复
来源：http://hz.xinyue.icu/gtfolfphls.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.ydjk.org.cn/gtmlacopxj.html

[U81] JS：初始化项目
来源：http://hz.xingfuxueyuan.xyz/gtpmrkmozp.html

npm init -y;  npm i express
来源：http://hz.meibo888.top/gtaqaimcpw.html

[U82] JS：package.json 脚本
来源：http://hz.gaohongyu789.top/gtbfthyswu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.chenlongwang.top/gtevidmpdb.html

[U83] JS：ES Module 导入导出
来源：http://hz.jianghu66.top/gtgnbvkldk.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.ywan-chungtsiang.top/gtrarzfnvq.html

[U84] JS：CommonJS 写法
来源：http://hz.sweek.top/gtnluwfkad.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.hysaishi.cn/gtxhmehzot.html

[U85] JS：可选链
来源：http://hz.jianghu66.top/gtbcgcvday.html

a?.b?.c
来源：http://hz.cashguo.top/gtzvuisohb.html

[U86] JS：空值合并
来源：http://hz.nanxinkj.top/gtwuqhmugx.html

a ?? b
来源：http://hz.shuidangran.top/gtzffholzu.html

[U87] JS：解构默认值
来源：http://hz.xziqi.cn/gtdfewkchb.html

const { a = 1, b = 2 } = obj;
来源：http://hz.wangdashe.top/gtwffgtvnu.html

[U88] JS：对象展开合并
来源：http://hz.hongshengwenyu.top/gtjrzifpbh.html

{ ...a, ...b }
来源：http://hz.quarkkingdee.top/gtuhaypgpp.html

[U89] JS：数组去重
来源：http://hz.meibo888.top/gtmeeyrfhi.html

[...new Set(arr)]
来源：http://hz.fengsongda.top/gtmopstuzs.html

[U90] JS：数字数组排序
来源：http://hz.yongpay.top/gtzoczfrxx.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hywenlv.cn/gtobjjhhhq.html

[U91] JS：对象键值遍历
来源：http://hz.fzhhl.top/gttktyxfrk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jyoumei.cn/gtznwzdbqn.html

[U92] JS：深拷贝
来源：http://hz.hnqzz.top/gtwlliyyqa.html

structuredClone(obj)
来源：http://hz.hongshengwenyu.top/gtqtakgdiu.html

[U93] JS：模板字符串
来源：http://hz.c1oappe.top/gthprmtfvi.html

`共 ${n} 条`
来源：http://hz.jinqigufen.top/gtomlcukqn.html

[U94] JS：箭头函数
来源：http://hz.gzhubu.top/gtagtzwoii.html

const double = x => x * 2;
来源：http://hz.xylfe.cn/gtjxnpzqwc.html

[U95] JS：Promise 包装
来源：http://hz.jqgufenzy.top/gtcgupsfbr.html

new Promise((resolve, reject) => {})
来源：http://hz.feifeiyinyue.top/gtcyvjqlcq.html

[U96] JS：async/await 与异常
来源：http://hz.aizwys.cn/gtqapkqdhd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.redwolf501.top/gtegzqngcr.html

[U97] JS：并发请求
来源：http://hz.ydzc1.top/gtnjjshkqc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinghuilouyu.cn/gtpgdbhatu.html

[U98] JS：fetch 带 JSON
来源：http://hz.aibaodan.cn/gtfbkcssrs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.9152youxi.cn/gtkfqiamls.html

[U99] JS：事件监听
来源：http://hz.birdmap.top/gtvjylmgvm.html

el.addEventListener("click", e => {})
来源：http://hz.xuanzx.com/gtmonvnhpy.html

[U100] JS：DOM 查询
来源：http://hz.iojbl.cn/gtnbwpsawq.html

document.querySelector(".item")
来源：http://hz.zdqjudy.top/gtiqwwgfhv.html

[U101] JS：classList 操作
来源：http://hz.smart0.xyz/gtomuzhjil.html

el.classList.toggle("active")
来源：http://hz.0kj1m.cn/gtyngobehc.html

[U102] JS：本地存储
来源：http://hz.yvedp.cn/gtmbyhmpej.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zhixingplan.top/gtjculjetl.html

[U103] JS：定时器
来源：http://hz.nanxuanxn.top/gtifnzjgeg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.dianchejie.cn/gtnlfbotsl.html

[U104] JS：防抖
来源：http://hz.yj20258888.top/gtzqsipizi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuanzhike.top/gtujnytvhr.html

[U105] JS：节流
来源：http://hz.shuidangran.top/gtkupvakpz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hysaishi.cn/gtdtzoncwk.html

[U106] JS：日期格式化
来源：http://hz.cdnleiting.top/gtfrcajmkp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ydjk.org.cn/gtrekeytom.html

[U107] JS：数字千分位
来源：http://hz.zhengqikj.top/gtdyucilbl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.fengsongda.top/gtidgvssqx.html

[U108] JS：随机整数
来源：http://hz.gogol.net.cn/gtlohrwjwj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ybcxt.top/gtpkrqqgfz.html

[U109] JS：数组分组
来源：http://hz.316326.xyz/gtlxluuaqw.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yangfankeji.com/gtazyxyjkm.html

[U110] JS：数组分块
来源：http://hz.yanxiufei.cn/gtyfcszeus.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jinghuilouyu.cn/gtsqmilwhu.html

[U111] JS：对象转 Map
来源：http://hz.cdnleiting.top/gtjexarkto.html

new Map(Object.entries(obj))
来源：http://hz.yangfankeji.com/gtccasurdu.html

[U112] JS：字符串补位
来源：http://hz.zhoulong.xyz/gtoqgbkiyl.html

"7".padStart(3, "0")
来源：http://hz.sufxvd.cn/gtyyvioqoj.html

[U113] JS：正则替换全部
来源：http://hz.cqqwz.cn/gtijddukpl.html

s.replaceAll("a", "b")
来源：http://hz.yvedp.cn/gteduweaej.html

[U114] JS：JSON 深比较
来源：http://hz.gotoacloud.top/gtodvujbgf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shanyushiyangkeji.top/gtmlyykjrm.html

[U115] JS：生成 UUID
来源：http://hz.hnqzz.top/gtexoogotd.html

crypto.randomUUID()
来源：http://hz.jlsjyb.cn/gtquwqjobu.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.pycfn.com/gtnyldlziw.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yuxming.cn/gtetvaijqw.html

[U117] JS：单元测试
来源：http://hz.aibaodan.cn/gtsmpwkflk.html

npm i -D vitest;  npx vitest
来源：http://hz.fzhhl.top/gtgtspfcjx.html

[U118] JS：开发服务器
来源：http://hz.shanyushiyangkeji.top/gtcxujeoik.html

npm i -D vite;  npx vite
来源：http://hz.hnxiangtu.top/gtipwrlcrj.html

[U119] JS：生产构建
来源：http://hz.mhx1999.top/gtpwewohck.html

npx vite build
来源：http://hz.jinyuanbaomall.cn/gtwlhcbnoc.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jqgfzy.top/gttlrdpiuv.html

import.meta.env.VITE_API_URL
来源：http://hz.yueranfly.top/gtjwqpmocl.html

================================================================================
来源：http://hz.yanxiufei.cn/gtcqcsumpn.html

统计汇总
来源：http://hz.xingfuxueyuan.xyz/gtdalttkgz.html

================================================================================
来源：http://hz.kuanghao11.cn/gtvcmqztej.html

按语言统计（条）：
来源：http://hz.gotoacloud.top/gttngtvphh.html

Python ......... 252
来源：http://hz.zhoulong.xyz/gtzmiahagp.html

PHP ............ 252
来源：http://hz.jinghuilouyu.cn/gtwwhhllhe.html

JavaScript ..... 252
来源：http://hz.yonumen.top/gtexhcuxll.html

TypeScript ..... 212
来源：http://hz.yj202588.top/gtmdlyqczh.html

Java ........... 212
来源：http://hz.jinyuanbaomall.cn/gtdvofnjzu.html

Go ............. 212
来源：http://hz.guannengcc.top/gtydyylfog.html

Ruby ........... 212
来源：http://hz.kuanghao11.cn/gtsuwtyirt.html

C# ............. 212
来源：http://hz.shzxlz.cn/gtxdyepask.html

C .............. 30
来源：http://hz.jlsjyb.cn/gtbyllzipt.html

C++ ............ 30
来源：http://hz.guannengcc.top/gtrjmvqgkl.html

SQL ............ 90
来源：http://hz.tian-w.cn/gthrzgkwbq.html

Bash ........... 80
来源：http://hz.zhengqikj.top/gtnsfivclz.html

Kotlin ......... 15
来源：http://hz.mhx1999.top/gtlluztijd.html

Swift .......... 15
来源：http://hz.zhiwuduotai.top/gteaqnbrfx.html

Lua ............ 10
来源：http://hz.yonumen.top/gthuruoawm.html

Perl ........... 10
来源：http://hz.xuanzx.com/gtradrlfzo.html

Scala .......... 10
来源：http://hz.chenjidiqi.icu/gtwkjpjdsl.html

------------------------------------
来源：http://hz.ehwqpu.com/gtnxwulpmf.html

合计 ........... 2106 条
来源：http://hz.jlsjyb.cn/gtamdobdbh.html

按章节统计：
来源：http://hz.tianlin.xyz/gtizuusqba.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.havefunace.top/gtwkjzfxcl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.xziqi.cn/gtrhhmhbrs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.hongshengwenyu.top/gtdpiwcckd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.nanxuanxn.top/gtfdspxhga.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jiagoushi.top/gtmhhbgcul.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yuxming.cn/gtkyzrvicz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.gogol.net.cn/gtedlrydup.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.jinqigfzy.top/gtumzbdwbx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.0kj1m.cn/gtntklpopk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.aibaodan.cn/gtnvzphpvx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.wangdashe.top/gtkvpwojba.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jinghuilouyu.cn/gthijhtbru.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.hnxiangtu.top/gtkroqdmzi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yj202588.top/gthsjekiqn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.daxiang520.top/gtacegqlga.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yj20258.top/gtlkwwqwng.html

Q SQL 专题                              90
来源：http://hz.quarkkingdee.top/gtylnjrymu.html

R Bash 专题                             80
来源：http://hz.xziqi.cn/gtvmmtvehl.html

S C / C++ 专题                          60
来源：http://hz.wangdashe.top/gtvalwkltx.html

T 其他语言补充                          60
来源：http://hz.yj20258888.top/gtepxkyhlx.html

U 高频实用片段                         120
来源：http://hz.pycfn.com/gtbbaepmht.html

------------------------------------
来源：http://hz.ehwqpu.com/gtkvjfoain.html

合计                                  2106 条
来源：http://hz.xziqi.cn/gtyxrxpugc.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258.top/gtoqztycfe.html

使用提醒
来源：http://hz.hnqzz.top/gtqedbxydc.html

--------------------------------------------------------------------------------
来源：http://hz.yj202588.top/gtodfnkodz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zhaomingkeji.xyz/gtbmsvnngp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.316326.xyz/gtvyfalvue.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.aizwys.cn/gtohpismdr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.quarkkingdee.top/gtagtlshzs.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.xziqi.cn/gtcyiinixf.html

—— 文件结束 ——
来源：http://hz.havefunace.top/gtikoiebqw.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtkzrldtax.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.aizwys.cn/gtxhmpkkhb.html

Common Programming Examples Cheat Book
来源：http://hz.nanxuanxn.top/gtzppgcidb.html

================================================================================
来源：http://hz.zhoulong.xyz/gtmjszvyuw.html


<!-- 参考信息 -->