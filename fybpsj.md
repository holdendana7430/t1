代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://hz.jianghu66.top/gtvwzgyeqi.html

[T51] Scala：Hello World
来源：http://hz.9152youxi.cn/gtfhrfnfjf.html

println("Hello")
来源：http://hz.zhoulong.xyz/gtqemucyvs.html

[T52] Scala：变量
来源：http://hz.yuanzhike.top/gtgfrxmhhd.html

val a = 1;  var b = 2
来源：http://hz.aizwys.cn/gtudnufcpu.html

[T53] Scala：字符串插值
来源：http://hz.chenzaomai.com/gtbnfrdops.html

s"值: $b"
来源：http://hz.jiagoushi.top/gtkyledlst.html

[T54] Scala：集合映射
来源：http://hz.ppjwa.cn/gtvrhhuwto.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hammf.cn/gtsstwzlgt.html

[T55] Scala：集合过滤
来源：http://hz.jiagoushi.top/gtcohxeuhv.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jqgufenzy.top/gtbavlezzy.html

[T56] Scala：样例类
来源：http://hz.yj20258888.top/gtaxmyzitx.html

case class User(name: String, age: Int)
来源：http://hz.yongpay.top/gtlodkbawo.html

[T57] Scala：模式匹配
来源：http://hz.tanke756.top/gtrpjfiwjl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.meibo888.top/gtdxhurcuo.html

[T58] Scala：函数定义
来源：http://hz.meibo888.top/gtywnzwnoe.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.hywenlv.cn/gtezodllnn.html

[T59] Scala：循环
来源：http://hz.cheryme.top/gtlubezvnh.html

for (i <- 1 to 10) println(i)
来源：http://hz.tanke756.top/gtmeyxysvc.html

[T60] Scala：折叠
来源：http://hz.tian-w.cn/gtvueyacka.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ybcxt.top/gtylmytftb.html

================================================================================
来源：http://hz.yangfankeji.com/gtdznygwqc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shzxlz.cn/gtbiceezxk.html

================================================================================
来源：http://hz.wangdashe.top/gtdwfabeug.html

[U01] Py：创建虚拟环境
来源：http://hz.haohaochexian.top/gtczhrwput.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xylfe.cn/gtazpucysz.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yueranfly.top/gtggfdjrrj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yangfankeji.com/gtscmpzxci.html

[U03] Py：加载 .env 配置
来源：http://hz.aibaodan.cn/gtsxbldihp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.bjfxy.top/gtmhyixgoc.html

[U04] Py：变量调试打印
来源：http://hz.yangfankeji.com/gtksyjrqry.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhengqikj.top/gttvrjmxbc.html

[U05] Py：列表去重且保序
来源：http://hz.fzhhl.top/gtnekaxjod.html

list(dict.fromkeys(arr))
来源：http://hz.nanxuanxn.top/gttplxmqzo.html

[U06] Py：合并两个字典
来源：http://hz.hywenlv.cn/gtnntavtdv.html

{**a, **b}
来源：http://hz.yuanzhike.top/gtmsgqphxb.html

[U07] Py：反转字典键值
来源：http://hz.shzxlz.cn/gtxxtnywrw.html

{v: k for k, v in d.items()}
来源：http://hz.haohaochexian.top/gtfewcqdtl.html

[U08] Py：展平二维列表
来源：http://hz.yj20258888.top/gtmtspypne.html

[y for x in nested for y in x]
来源：http://hz.xuetiantiany.cn/gtnvxtdeoc.html

[U09] Py：字典取最大值的键
来源：http://hz.cucudq.cn/gtrndgwkwg.html

max(d, key=d.get)
来源：http://hz.xylfe.cn/gtrsgxkrqq.html

[U10] Py：按值排序字典
来源：http://hz.jianghu66.top/gtytdniuav.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.smart0.xyz/gtgzlcgahi.html

[U11] Py：生成器表达式
来源：http://hz.tianlin.xyz/gtpgjhnwys.html

(x * 2 for x in arr)
来源：http://hz.ppjwa.cn/gtjprfmzlm.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.tanke756.top/gtptmrzncs.html

Counter(arr).most_common(3)
来源：http://hz.gaohongyu789.top/gthuguhwdl.html

[U13] Py：固定长度队列
来源：http://hz.jinqigfzy.top/gtcxrwgnsa.html

deque(maxlen=10)
来源：http://hz.nanxuanxn.top/gtrzagycgv.html

[U14] Py：分组收集到列表
来源：http://hz.yanxiufei.cn/gtfiowzvrt.html

defaultdict(list)
来源：http://hz.cqqwz.cn/gtwpaghkdq.html

[U15] Py：高精度计时
来源：http://hz.cdnleiting.top/gtwbyaypdd.html

t = time.perf_counter()
来源：http://hz.bjfxy.top/gtwbkxcirf.html

[U16] Py：命令行参数解析
来源：http://hz.zdqjudy.top/gtwcsbbhqe.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jinyuanbaomall.cn/gtvhojxowt.html

[U17] Py：初始化日志
来源：http://hz.hfpthk.cn/gtaghbejjn.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.haohaochexian.top/gtayhspcvm.html

[U18] Py：预编译正则
来源：http://hz.tanke756.top/gtcrwmvdwf.html

pat = re.compile(r"\d+")
来源：http://hz.hnqzz.top/gtwgwghocy.html

[U19] Py：正则替换带回调
来源：http://hz.jiagoushi.top/gtospjzwso.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.quarkkingdee.top/gtsdbgrsdz.html

[U20] Py：缓存函数结果
来源：http://hz.yj20258.top/gtmsrnsvgm.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yueranfly.top/gtjgjfucmx.html

[U21] Py：自定义上下文管理器
来源：http://hz.hysaishi.cn/gtoyqmyynv.html

@contextlib.contextmanager
来源：http://hz.cucudq.cn/gtnamocgxf.html

[U22] Py：矩阵转置
来源：http://hz.feifeiyinyue.top/gtqpdhstwt.html

list(zip(*m))
来源：http://hz.hnxiangtu.top/gtapolejsw.html

[U23] Py：分块读取大文件
来源：http://hz.yvedp.cn/gtfujuwlfv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ydzc1.top/gtsndfkvdx.html

[U24] Py：路径操作
来源：http://hz.bjfxy.top/gtjtajdozp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yvedp.cn/gtzfpjwswf.html

[U25] Py：CSV 按字典读
来源：http://hz.mhx1999.top/gtyosgurvj.html

csv.DictReader(f)
来源：http://hz.jqgufenzy.top/gtiuwobgyh.html

[U26] Py：并发下载
来源：http://hz.haohaochexian.top/gtmwokhual.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhoulong.xyz/gtgejfqmbw.html

[U27] Py：异步 HTTP
来源：http://hz.gotoacloud.top/gtoopvxbkz.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.0kj1m.cn/gtuhvsfwzf.html

[U28] Py：类型别名
来源：http://hz.bjfxy.top/gtgcjxkecn.html

UserId = int
来源：http://hz.zhiwuduotai.top/gtrvzxpams.html

[U29] Py：属性校验
来源：http://hz.zhongyouzk.top/gtabixaxus.html

@property 与 @x.setter 配合
来源：http://hz.svipenyu.cn/gthbzxjfcv.html

[U30] Py：数据类
来源：http://hz.aibaodan.cn/gtujseyxti.html

@dataclass(slots=True)
来源：http://hz.yj202588.top/gtjycihcrj.html

[U31] Py：单测
来源：http://hz.wangdashe.top/gtxwujkavk.html

python -m pytest -q
来源：http://hz.quarkkingdee.top/gtokdapzxc.html

[U32] Py：代码格式化
来源：http://hz.ppjwa.cn/gtlnvhezwa.html

ruff format . && ruff check --fix .
来源：http://hz.tian-w.cn/gtpfatkzqd.html

[U33] Py：打包发布
来源：http://hz.zhiwuduotai.top/gtfxcsxroc.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.cheryme.top/gtdvjwkwgj.html

[U34] Py：判断编码
来源：http://hz.zdqjudy.top/gtboxhokld.html

chardet.detect(raw)
来源：http://hz.wangshuangyany.cn/gtwtyaenue.html

[U35] Py：发送邮件
来源：http://hz.yongpay.top/gttdrgdced.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cdnleiting.top/gtgvstzubd.html

[U36] Py：定时任务
来源：http://hz.tanke756.top/gtlluegstt.html

schedule.every(10).minutes.do(job)
来源：http://hz.redwolf501.top/gtpixdhtkg.html

[U37] Py：读写 Excel
来源：http://hz.zdqjudy.top/gtabiakvcv.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.sysykeji.top/gtcnnwgqfg.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhoulong.xyz/gtybmiapef.html

Path(__file__).resolve().parent
来源：http://hz.ybcxt.top/gtyjltnvxe.html

[U39] Py：判断是否在交互环境
来源：http://hz.sxryk.cn/gtjkqdmbph.html

sys.stdout.isatty()
来源：http://hz.jinyuanbaomall.cn/gtbrfdexie.html

[U40] Py：打印到标准错误
来源：http://hz.nanxuanxn.top/gtsupobzns.html

print("err", file=sys.stderr)
来源：http://hz.xuetiantiany.cn/gtgsjrpswv.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.xingfuxueyuan.xyz/gtsolshwxz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.cucudq.cn/gtwivzxgvu.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.haohaochexian.top/gtkxnwqtdx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.cucudq.cn/gtqsjobqle.html

[U43] PHP：声明命名空间
来源：http://hz.c1oappe.top/gtmqmycvpw.html

namespace App\Http;
来源：http://hz.ivvv.top/gtecppetkg.html

[U44] PHP：开启严格类型
来源：http://hz.haohaochexian.top/gtzjuametj.html

declare(strict_types=1);
来源：http://hz.sufxvd.cn/gtnwtzqedx.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hongshengwenyu.top/gtzxjsaofj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zdqjudy.top/gtuzvefxcq.html

[U46] PHP：可空类型
来源：http://hz.mhx1999.top/gtbpihhhdd.html

?string $name = null
来源：http://hz.guowangkeji.top/gtxyhmfats.html

[U47] PHP：联合类型
来源：http://hz.nanxinkj.top/gtzgzmkazo.html

int|string $id
来源：http://hz.zhiwuduotai.top/gtpnlctjpg.html

[U48] PHP：纯枚举
来源：http://hz.ybcxt.top/gtlgfjnykx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.c1oappe.top/gtainizwpw.html

[U49] PHP：只读属性
来源：http://hz.guowangkeji.top/gtwaidbewz.html

public readonly string $name
来源：http://hz.xylfe.cn/gtxavgeqiw.html

[U50] PHP：构造器属性提升
来源：http://hz.hysaishi.cn/gtabfbuusg.html

public function __construct(private int $id) {}
来源：http://hz.9152youxi.cn/gtyfnynuvf.html

[U51] PHP：数组解构
来源：http://hz.nwbrower.top/gtzloorqok.html

[$a, $b] = $arr;
来源：http://hz.redwolf501.top/gticzmchoy.html

[U52] PHP：箭头函数
来源：http://hz.zhongyouzk.top/gtnjtlekek.html

$double = fn($x) => $x * 2;
来源：http://hz.hnqzz.top/gttqzxvmqc.html

[U53] PHP：空合并运算符
来源：http://hz.gogol.net.cn/gtsqccdokn.html

$v = $a ?? $b ?? "default";
来源：http://hz.jlsjyb.cn/gtiymbxlzq.html

[U54] PHP：空安全调用
来源：http://hz.ybcxt.top/gthfludfkj.html

$obj?->method()
来源：http://hz.tanke756.top/gtsdspduea.html

[U55] PHP：match 表达式
来源：http://hz.pengpengdd.cyou/gtwmqicpkv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.andypj.xyz/gtbdctmfiw.html

[U56] PHP：命名参数
来源：http://hz.sysykeji.top/gtbwwtoxfs.html

f(a: 1, b: 2)
来源：http://hz.sweek.top/gtiicydzzk.html

[U57] PHP：字符串插值
来源：http://hz.yj202588.top/gtejshaega.html

"值: {$a}"
来源：http://hz.hywenlv.cn/gtoqedspgf.html

[U58] PHP：数组三件套
来源：http://hz.ydjk.org.cn/gtcbekgjnt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.kuanghao11.cn/gtxacpwfpx.html

[U59] PHP：自定义排序
来源：http://hz.zhiwuduotai.top/gtlyysuhht.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.aizwys.cn/gtubueauav.html

[U60] PHP：JSON 编解码
来源：http://hz.ivvv.top/gtnidrhtfh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jqgfzy.top/gtxtoysnvf.html

[U61] PHP：正则
来源：http://hz.yj20258.top/gtfexywdyq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.xziqi.cn/gtxockfdyc.html

[U62] PHP：日期对象
来源：http://hz.xuanzx.com/gtfouzotei.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yongpay.top/gtnpxbbncp.html

[U63] PHP：文件读写
来源：http://hz.quarkkingdee.top/gtfzheuvpv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yuxming.cn/gtrygprzmj.html

[U64] PHP：目录遍历
来源：http://hz.dashuyun.cn/gtayxcjfcb.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.mhx1999.top/gtfecsojij.html

[U65] PHP：会话
来源：http://hz.shzxlz.cn/gtbllrebwa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zhixingplan.top/gtbfdsixeo.html

[U66] PHP：设置 Cookie
来源：http://hz.ywan-chungtsiang.top/gtngksnpaq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yongpay.top/gtmkbioixl.html

[U67] PHP：处理文件上传
来源：http://hz.xuanzx.com/gtgtybwwrp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.pycfn.com/gtdgqcymcd.html

[U68] PHP：PDO 连接
来源：http://hz.hysaishi.cn/gtejlgdbjh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.ydjk.org.cn/gtwemzckzu.html

[U69] PHP：PDO 预处理
来源：http://hz.cdnleiting.top/gtnkwedmud.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.ybcxt.top/gtxwqditvf.html

[U70] PHP：PDO 事务
来源：http://hz.jinqigufen.top/gtpqxcdrvu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.ivvv.top/gtnwbutlde.html

[U71] PHP：抛出异常
来源：http://hz.dianchejie.cn/gtiwxyesmw.html

throw new RuntimeException("失败", 500);
来源：http://hz.daxiang520.top/gtgfemidox.html

[U72] PHP：写错误日志
来源：http://hz.gotoacloud.top/gtnceiiffl.html

error_log("失败: " . $e->getMessage());
来源：http://hz.jinqigfzy.top/gtfeztjaux.html

[U73] PHP：读取 ini 配置
来源：http://hz.chenjidiqi.icu/gtrynmgzux.html

parse_ini_file("config.ini", true)
来源：http://hz.jinqigfzy.top/gtdznkneef.html

[U74] PHP：读取环境变量
来源：http://hz.xingfuxueyuan.xyz/gtaeigpvob.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yj20258888.top/gtbwahvyxe.html

[U75] PHP：依赖注入
来源：http://hz.redwolf501.top/gtvqywmdwy.html

composer require psr/container
来源：http://hz.zhixingplan.top/gtzmmkopir.html

[U76] PHP：简单路由
来源：http://hz.jinghuilouyu.cn/gtacocdnic.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yvedp.cn/gtlevzxvng.html

[U77] PHP：模板渲染
来源：http://hz.dashuyun.cn/gtjwlxedez.html

composer require twig/twig
来源：http://hz.haohaochexian.top/gtbbdslaws.html

[U78] PHP：单元测试
来源：http://hz.birdmap.top/gtgsvwplhy.html

composer require --dev phpunit/phpunit
来源：http://hz.jianghu66.top/gtiuavziuf.html

[U79] PHP：静态分析
来源：http://hz.ehwqpu.com/gtlcitukts.html

composer require --dev phpstan/phpstan
来源：http://hz.316326.xyz/gtlvyypylb.html

[U80] PHP：代码规范修复
来源：http://hz.xinyue.icu/gtpwqapnue.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.havefunace.top/gtdokllgiz.html

[U81] JS：初始化项目
来源：http://hz.nanxuanxn.top/gtrlmmfbzx.html

npm init -y;  npm i express
来源：http://hz.daria6918.cn/gtcvpdbddq.html

[U82] JS：package.json 脚本
来源：http://hz.chenlongwang.top/gtdnnoumbt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.nanxinkj.top/gtivxjmwvk.html

[U83] JS：ES Module 导入导出
来源：http://hz.nwbrower.top/gtltvtplxz.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.jqgfzy.top/gtxinhyaid.html

[U84] JS：CommonJS 写法
来源：http://hz.jiagoushi.top/gtuiombtkf.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.shanyushiyangkeji.top/gtzltlakel.html

[U85] JS：可选链
来源：http://hz.cdnleiting.top/gtphaxojle.html

a?.b?.c
来源：http://hz.cashguo.top/gtmogxbvte.html

[U86] JS：空值合并
来源：http://hz.fzhhl.top/gtfisyouqr.html

a ?? b
来源：http://hz.zycfv.cn/gtzwariomt.html

[U87] JS：解构默认值
来源：http://hz.ydzc1.top/gtgbykrpbz.html

const { a = 1, b = 2 } = obj;
来源：http://hz.shanyushiyangtech.top/gthzsbdsvg.html

[U88] JS：对象展开合并
来源：http://hz.snrcjt.cn/gtfiidaskc.html

{ ...a, ...b }
来源：http://hz.xinyue.icu/gtzfcefbpx.html

[U89] JS：数组去重
来源：http://hz.jiagoushi.top/gtzqipjnyi.html

[...new Set(arr)]
来源：http://hz.jinghuilouyu.cn/gturolcyju.html

[U90] JS：数字数组排序
来源：http://hz.daria6918.cn/gtklukqncb.html

[...arr].sort((a, b) => a - b)
来源：http://hz.chenzaomai.com/gtfvmsztma.html

[U91] JS：对象键值遍历
来源：http://hz.pycfn.com/gtagxdiari.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yangfankeji.com/gtmczssret.html

[U92] JS：深拷贝
来源：http://hz.jinqigfzy.top/gtmoqjdvad.html

structuredClone(obj)
来源：http://hz.cucudq.cn/gtcbsdmyjj.html

[U93] JS：模板字符串
来源：http://hz.hysaishi.cn/gtijgrvwno.html

`共 ${n} 条`
来源：http://hz.yj20258888.top/gtmdcnilms.html

[U94] JS：箭头函数
来源：http://hz.wangdashe.top/gthbmizsmy.html

const double = x => x * 2;
来源：http://hz.wangshuangyany.cn/gtsddagcpw.html

[U95] JS：Promise 包装
来源：http://hz.sufxvd.cn/gtbwfahtkz.html

new Promise((resolve, reject) => {})
来源：http://hz.shanyushiyangtech.top/gtppiqyutd.html

[U96] JS：async/await 与异常
来源：http://hz.yonumen.top/gtiptrqtut.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yuxming.cn/gtwpfpujtv.html

[U97] JS：并发请求
来源：http://hz.0kj1m.cn/gtfswueirt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shuidangran.top/gttxpfmmeq.html

[U98] JS：fetch 带 JSON
来源：http://hz.tanke756.top/gtfafzcxux.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.iojbl.cn/gtuuxweoji.html

[U99] JS：事件监听
来源：http://hz.iojbl.cn/gtelzhrfzl.html

el.addEventListener("click", e => {})
来源：http://hz.sufxvd.cn/gtbanecjqa.html

[U100] JS：DOM 查询
来源：http://hz.zhongyouzk.top/gtdvxzbzjg.html

document.querySelector(".item")
来源：http://hz.yueranfly.top/gttnddbguq.html

[U101] JS：classList 操作
来源：http://hz.zhoulong.xyz/gthwpqqksn.html

el.classList.toggle("active")
来源：http://hz.cdnleiting.top/gtzzcburos.html

[U102] JS：本地存储
来源：http://hz.fzhhl.top/gtguvdlduz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ivvv.top/gtutthkdkc.html

[U103] JS：定时器
来源：http://hz.jianghu66.top/gtyarcvxpr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.havefunace.top/gtozcfidnu.html

[U104] JS：防抖
来源：http://hz.yj202588.top/gtvfdnbrah.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.haohaochexian.top/gtdhyprzqv.html

[U105] JS：节流
来源：http://hz.chenjidiqi.icu/gtzueetnup.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.daria6918.cn/gtogwbzpjt.html

[U106] JS：日期格式化
来源：http://hz.pycfn.com/gtrjkgidvj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.gotoacloud.top/gtpvgczjrj.html

[U107] JS：数字千分位
来源：http://hz.jianghu66.top/gtpcheoruw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.birdmap.top/gtsuurqwnq.html

[U108] JS：随机整数
来源：http://hz.birdmap.top/gtackbyvco.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.fengsongda.top/gtyjvbtuya.html

[U109] JS：数组分组
来源：http://hz.ydjk.org.cn/gtumziimbz.html

Object.groupBy(arr, x => x.type)
来源：http://hz.hongshengwenyu.top/gtqaiqteqk.html

[U110] JS：数组分块
来源：http://hz.iojbl.cn/gtrurgmcep.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yj202588.top/gtxtrrwzoh.html

[U111] JS：对象转 Map
来源：http://hz.jinghuilouyu.cn/gtorgksyvo.html

new Map(Object.entries(obj))
来源：http://hz.yuxming.cn/gtwooddrlr.html

[U112] JS：字符串补位
来源：http://hz.bjfxy.top/gtacymnfiv.html

"7".padStart(3, "0")
来源：http://hz.xinyue.icu/gtlmbivmsn.html

[U113] JS：正则替换全部
来源：http://hz.ivvv.top/gtlogxzkwu.html

s.replaceAll("a", "b")
来源：http://hz.ybcxt.top/gtkumomrya.html

[U114] JS：JSON 深比较
来源：http://hz.316326.xyz/gtufeccebz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhijiandao.cn/gtblcinkfy.html

[U115] JS：生成 UUID
来源：http://hz.zhaomingkeji.xyz/gtfsmjsxzb.html

crypto.randomUUID()
来源：http://hz.cashguo.top/gtsokqtekf.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.sysykeji.top/gtvqwszlli.html

/** @param {string} name */ function f(name) {}
来源：http://hz.andypj.xyz/gtddliprql.html

[U117] JS：单元测试
来源：http://hz.jianghu66.top/gthrqpqfbp.html

npm i -D vitest;  npx vitest
来源：http://hz.zycfv.cn/gteundfskl.html

[U118] JS：开发服务器
来源：http://hz.cashguo.top/gthyfprsaw.html

npm i -D vite;  npx vite
来源：http://hz.yongpay.top/gtepmweoee.html

[U119] JS：生产构建
来源：http://hz.cashguo.top/gtbagvehfw.html

npx vite build
来源：http://hz.daxiang520.top/gtebdtcern.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.dashuyun.cn/gtupxrbjas.html

import.meta.env.VITE_API_URL
来源：http://hz.zhixingplan.top/gtmzzagixv.html

================================================================================
来源：http://hz.kuanghao11.cn/gtqxkesmxl.html

统计汇总
来源：http://hz.meibo888.top/gtzwqynfys.html

================================================================================
来源：http://hz.wangdashe.top/gtonmkrewm.html

按语言统计（条）：
来源：http://hz.jinqigfzy.top/gtagsspkym.html

Python ......... 252
来源：http://hz.yongpay.top/gtdktscpmu.html

PHP ............ 252
来源：http://hz.shzxlz.cn/gtsytidahd.html

JavaScript ..... 252
来源：http://hz.daria6918.cn/gtkacmxnpi.html

TypeScript ..... 212
来源：http://hz.shanyushiyangkeji.top/gtpsttirwr.html

Java ........... 212
来源：http://hz.chenlongwang.top/gtyifhkwxr.html

Go ............. 212
来源：http://hz.ehwqpu.com/gtwxzvfllo.html

Ruby ........... 212
来源：http://hz.cdnleiting.top/gtpmreozrv.html

C# ............. 212
来源：http://hz.snrcjt.cn/gtnidgwtso.html

C .............. 30
来源：http://hz.guannengcc.top/gtqfperncx.html

C++ ............ 30
来源：http://hz.guowangkeji.top/gtyztdgsgs.html

SQL ............ 90
来源：http://hz.xuanzx.com/gthuzdufub.html

Bash ........... 80
来源：http://hz.c1oappe.top/gtwnjefrkt.html

Kotlin ......... 15
来源：http://hz.guannengcc.top/gtcympigai.html

Swift .......... 15
来源：http://hz.shuidangran.top/gtyacpzili.html

Lua ............ 10
来源：http://hz.nwbrower.top/gtuqbinryl.html

Perl ........... 10
来源：http://hz.shzxlz.cn/gtyaxrraso.html

Scala .......... 10
来源：http://hz.xylfe.cn/gtdogqxofa.html

------------------------------------
来源：http://hz.chenlongwang.top/gtgvjdsgdc.html

合计 ........... 2106 条
来源：http://hz.gzhubu.top/gtpwnxndam.html

按章节统计：
来源：http://hz.jqgfzy.top/gtxajwrjtk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.ivvv.top/gtacpvcayz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.sxryk.cn/gtsllnqkii.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.chenzaomai.com/gtblfqzphw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.xingfuxueyuan.xyz/gtbjzjewey.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.aibaodan.cn/gtqrvcqtrt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.cashguo.top/gtjbipgqnz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yj20258888.top/gtirstwyii.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.hfpthk.cn/gtmhqddcdz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.kuanghao11.cn/gtkrgnucmo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.andypj.xyz/gtozqwoelu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.wangshuangyany.cn/gtsaylutop.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.shzxlz.cn/gtmigltylk.html


<!-- 参考信息 -->