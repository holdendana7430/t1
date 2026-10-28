代发 wailian999

val a = 1;  var b = 2
来源：http://hz.hfpthk.cn/gtjlxhqunp.html

[T53] Scala：字符串插值
来源：http://hz.tian-w.cn/gtpqejcmvx.html

s"值: $b"
来源：http://hz.cqqwz.cn/gtchndszuu.html

[T54] Scala：集合映射
来源：http://hz.yanxiufei.cn/gtmqklcqvx.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.cashguo.top/gtmqdcmdar.html

[T55] Scala：集合过滤
来源：http://hz.meibo888.top/gtujoqnuwk.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.pengpengdd.cyou/gtbtwupzkn.html

[T56] Scala：样例类
来源：http://hz.shanyushiyangkeji.top/gtmimgeunc.html

case class User(name: String, age: Int)
来源：http://hz.ppjwa.cn/gtdccokbtw.html

[T57] Scala：模式匹配
来源：http://hz.9152youxi.cn/gtjsanfygy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yangfankeji.com/gtpazfeeaf.html

[T58] Scala：函数定义
来源：http://hz.quarkkingdee.top/gtjgydafzb.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.chenjidiqi.icu/gtbtiterlk.html

[T59] Scala：循环
来源：http://hz.yuanzhike.top/gtecbzvuvc.html

for (i <- 1 to 10) println(i)
来源：http://hz.ydjk.org.cn/gtlxdheyzc.html

[T60] Scala：折叠
来源：http://hz.wangshuangyany.cn/gtljzcdcwn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hongshengwenyu.top/gtxoeqguuq.html

================================================================================
来源：http://hz.xylfe.cn/gtswiuhuoi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.havefunace.top/gtxnauwvvg.html

================================================================================
来源：http://hz.cucudq.cn/gtybrkkqbn.html

[U01] Py：创建虚拟环境
来源：http://hz.haohaochexian.top/gtklwzsgph.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xinyue.icu/gtbmbrzwne.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yangfankeji.com/gtdgblsqok.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.snrcjt.cn/gtsppltsvb.html

[U03] Py：加载 .env 配置
来源：http://hz.xuanzx.com/gtwdyimois.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.nanxinkj.top/gtumovblxl.html

[U04] Py：变量调试打印
来源：http://hz.gaohongyu789.top/gtibrwclvl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.ywan-chungtsiang.top/gtwzggdgce.html

[U05] Py：列表去重且保序
来源：http://hz.yongpay.top/gtfzhchadg.html

list(dict.fromkeys(arr))
来源：http://hz.sysykeji.top/gtfgxyuyxc.html

[U06] Py：合并两个字典
来源：http://hz.gogol.net.cn/gtghhqaegc.html

{**a, **b}
来源：http://hz.hammf.cn/gtseuhvjqa.html

[U07] Py：反转字典键值
来源：http://hz.yj20258.top/gtrssfknht.html

{v: k for k, v in d.items()}
来源：http://hz.zhengqikj.top/gtxzdqhuuk.html

[U08] Py：展平二维列表
来源：http://hz.gaohongyu789.top/gtieepitej.html

[y for x in nested for y in x]
来源：http://hz.cheryme.top/gtmvqjxyds.html

[U09] Py：字典取最大值的键
来源：http://hz.andypj.xyz/gtbrnoeckt.html

max(d, key=d.get)
来源：http://hz.daxiang520.top/gtexgabyoe.html

[U10] Py：按值排序字典
来源：http://hz.meibo888.top/gtwljdmsfb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hongshengwenyu.top/gtubpyvxlm.html

[U11] Py：生成器表达式
来源：http://hz.zdqjudy.top/gtjnzjwhid.html

(x * 2 for x in arr)
来源：http://hz.chenjidiqi.icu/gtqttylixg.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.cdnleiting.top/gtuwmbcnzw.html

Counter(arr).most_common(3)
来源：http://hz.bjfxy.top/gtxvtvljrj.html

[U13] Py：固定长度队列
来源：http://hz.yj202588.top/gtlrzetqfc.html

deque(maxlen=10)
来源：http://hz.sufxvd.cn/gtkrltmjnp.html

[U14] Py：分组收集到列表
来源：http://hz.c1oappe.top/gtxdpgabzb.html

defaultdict(list)
来源：http://hz.ydzc1.top/gtxowlfnwr.html

[U15] Py：高精度计时
来源：http://hz.ydjk.org.cn/gtxdzrjsnm.html

t = time.perf_counter()
来源：http://hz.jqgfzy.top/gterpdkiqz.html

[U16] Py：命令行参数解析
来源：http://hz.hongshengwenyu.top/gtyyxbojzm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.shanyushiyangtech.top/gtwgyikzis.html

[U17] Py：初始化日志
来源：http://hz.zdqjudy.top/gtckzprrbm.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.chenzaomai.com/gthtlnjjri.html

[U18] Py：预编译正则
来源：http://hz.zhixingplan.top/gtdnbgrhef.html

pat = re.compile(r"\d+")
来源：http://hz.tian-w.cn/gtawxofdul.html

[U19] Py：正则替换带回调
来源：http://hz.tian-w.cn/gthbqjrvqm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zycfv.cn/gtitdnreko.html

[U20] Py：缓存函数结果
来源：http://hz.bjfxy.top/gtrdvtznsx.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yj20258.top/gtjvvkpkrh.html

[U21] Py：自定义上下文管理器
来源：http://hz.aizwys.cn/gtuatqdjzy.html

@contextlib.contextmanager
来源：http://hz.jlsjyb.cn/gtbrfdyhpg.html

[U22] Py：矩阵转置
来源：http://hz.jinqigfzy.top/gtbtlkyxde.html

list(zip(*m))
来源：http://hz.zhijiandao.cn/gtmeiyzpzx.html

[U23] Py：分块读取大文件
来源：http://hz.ybcxt.top/gtrzsjazab.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cqqwz.cn/gtoouhzdna.html

[U24] Py：路径操作
来源：http://hz.zhixingplan.top/gtiffzbapx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.xinyue.icu/gthgcicyne.html

[U25] Py：CSV 按字典读
来源：http://hz.zhixingplan.top/gtkoyjkpnp.html

csv.DictReader(f)
来源：http://hz.feifeiyinyue.top/gtvqnlnyuk.html

[U26] Py：并发下载
来源：http://hz.cdnleiting.top/gtahknyrcu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.sxryk.cn/gtkorvliqn.html

[U27] Py：异步 HTTP
来源：http://hz.chenzaomai.com/gtucwdkruz.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.hnqzz.top/gtovfvkape.html

[U28] Py：类型别名
来源：http://hz.0kj1m.cn/gtivxwnyel.html

UserId = int
来源：http://hz.chenzaomai.com/gtptzdovym.html

[U29] Py：属性校验
来源：http://hz.gaohongyu789.top/gtquktfqdz.html

@property 与 @x.setter 配合
来源：http://hz.yj202588.top/gtuxxoihrq.html

[U30] Py：数据类
来源：http://hz.zhixingplan.top/gtbddkbeju.html

@dataclass(slots=True)
来源：http://hz.fengsongda.top/gtlafjrwpv.html

[U31] Py：单测
来源：http://hz.zdqjudy.top/gtyzblqona.html

python -m pytest -q
来源：http://hz.shzxlz.cn/gtjnokdhea.html

[U32] Py：代码格式化
来源：http://hz.aibaodan.cn/gtzrvdpkzt.html

ruff format . && ruff check --fix .
来源：http://hz.cqqwz.cn/gtikvcgdit.html

[U33] Py：打包发布
来源：http://hz.cucudq.cn/gtstgqnpkm.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.cdnleiting.top/gtkegevcpu.html

[U34] Py：判断编码
来源：http://hz.birdmap.top/gtbmfiqskf.html

chardet.detect(raw)
来源：http://hz.chenlongwang.top/gtcnnmyjmp.html

[U35] Py：发送邮件
来源：http://hz.cucudq.cn/gtylfaqouo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.snrcjt.cn/gtosvvbaer.html

[U36] Py：定时任务
来源：http://hz.0kj1m.cn/gtgpsekeis.html

schedule.every(10).minutes.do(job)
来源：http://hz.jqgufenzy.top/gtbhxjcuft.html

[U37] Py：读写 Excel
来源：http://hz.yueranfly.top/gtzmijnuyl.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ivvv.top/gtnbehvyhc.html

[U38] Py：获取脚本所在目录
来源：http://hz.iojbl.cn/gtfgkdhvym.html

Path(__file__).resolve().parent
来源：http://hz.andypj.xyz/gtbxgelygz.html

[U39] Py：判断是否在交互环境
来源：http://hz.ivvv.top/gtbjwyfnrc.html

sys.stdout.isatty()
来源：http://hz.c1oappe.top/gtmcgrpesk.html

[U40] Py：打印到标准错误
来源：http://hz.sufxvd.cn/gtqdnhknvb.html

print("err", file=sys.stderr)
来源：http://hz.zycfv.cn/gteoaqftsa.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.havefunace.top/gtwfdqwueu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hnxiangtu.top/gtueataizb.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.shanyushiyangkeji.top/gtgtobwdei.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yj20258888.top/gtwstddpiv.html

[U43] PHP：声明命名空间
来源：http://hz.shzxlz.cn/gtlkxpncoc.html

namespace App\Http;
来源：http://hz.xziqi.cn/gtwoocqopv.html

[U44] PHP：开启严格类型
来源：http://hz.guowangkeji.top/gtfglxqskx.html

declare(strict_types=1);
来源：http://hz.mhx1999.top/gtkdkmdbrd.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yuxming.cn/gtkrzwlyar.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.smart0.xyz/gtzeyvklbp.html

[U46] PHP：可空类型
来源：http://hz.hnqzz.top/gtaqkunnmj.html

?string $name = null
来源：http://hz.andypj.xyz/gtqxnazldr.html

[U47] PHP：联合类型
来源：http://hz.zdqjudy.top/gtzrlfxktn.html

int|string $id
来源：http://hz.zhiwuduotai.top/gtplkvqgbe.html

[U48] PHP：纯枚举
来源：http://hz.meibo888.top/gtvcwombac.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yongpay.top/gtccfniazl.html

[U49] PHP：只读属性
来源：http://hz.svipenyu.cn/gtlzitrunw.html

public readonly string $name
来源：http://hz.hammf.cn/gtwwckfuvp.html

[U50] PHP：构造器属性提升
来源：http://hz.mhx1999.top/gtnkccjhbw.html

public function __construct(private int $id) {}
来源：http://hz.hnxiangtu.top/gtbnhetqfj.html

[U51] PHP：数组解构
来源：http://hz.fengsongda.top/gtcrdqrqhz.html

[$a, $b] = $arr;
来源：http://hz.wangshuangyany.cn/gtnjzesocv.html

[U52] PHP：箭头函数
来源：http://hz.jqgufenzy.top/gtcoccctdu.html

$double = fn($x) => $x * 2;
来源：http://hz.yj20258.top/gtikylnitl.html

[U53] PHP：空合并运算符
来源：http://hz.tanke756.top/gtiguhvgkc.html

$v = $a ?? $b ?? "default";
来源：http://hz.hongshengwenyu.top/gttkfajqgf.html

[U54] PHP：空安全调用
来源：http://hz.hongshengwenyu.top/gtnlbsmexu.html

$obj?->method()
来源：http://hz.guannengcc.top/gtggroyjui.html

[U55] PHP：match 表达式
来源：http://hz.cdnleiting.top/gtrlgokrjj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.bjfxy.top/gtgvxlrlpw.html

[U56] PHP：命名参数
来源：http://hz.yj20258.top/gtizrwijqw.html

f(a: 1, b: 2)
来源：http://hz.andypj.xyz/gtehcrcoxl.html

[U57] PHP：字符串插值
来源：http://hz.xziqi.cn/gtpwrnahrw.html

"值: {$a}"
来源：http://hz.yj202588.top/gtqlnelgad.html

[U58] PHP：数组三件套
来源：http://hz.xuetiantiany.cn/gtfefwxnmv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.sysykeji.top/gtysyadaoy.html

[U59] PHP：自定义排序
来源：http://hz.birdmap.top/gtaglydvhh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hongshengwenyu.top/gtxnjqddqu.html

[U60] PHP：JSON 编解码
来源：http://hz.cucudq.cn/gtmvfeuxqm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ywan-chungtsiang.top/gtlcjkzzax.html

[U61] PHP：正则
来源：http://hz.kuanghao11.cn/gtqiheelin.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.gogol.net.cn/gtudzcckcd.html

[U62] PHP：日期对象
来源：http://hz.jinqigufen.top/gtpfgvsygq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.andypj.xyz/gtvxqabliy.html

[U63] PHP：文件读写
来源：http://hz.yanxiufei.cn/gtioimexfv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yj20258888.top/gtatuvgzsj.html

[U64] PHP：目录遍历
来源：http://hz.jianghu66.top/gtehrvhrfn.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.sweek.top/gtvqaepsiw.html

[U65] PHP：会话
来源：http://hz.ydzc1.top/gtzzsxjjet.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.svipenyu.cn/gtrghknyob.html

[U66] PHP：设置 Cookie
来源：http://hz.hammf.cn/gtzowgsybj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.smart0.xyz/gtiwactbxu.html

[U67] PHP：处理文件上传
来源：http://hz.wangshuangyany.cn/gtxalohiri.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.shanyushiyangtech.top/gtpcpjkahn.html

[U68] PHP：PDO 连接
来源：http://hz.shanyushiyangkeji.top/gtrtedmrnf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yj20258888.top/gtlfojntpp.html

[U69] PHP：PDO 预处理
来源：http://hz.yongpay.top/gtojzylxyx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.feifeiyinyue.top/gtqycfnblg.html

[U70] PHP：PDO 事务
来源：http://hz.jqgufenzy.top/gtjuflkbrz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zhongyouzk.top/gtmprzocsa.html

[U71] PHP：抛出异常
来源：http://hz.chenjidiqi.icu/gtmxfozaqe.html

throw new RuntimeException("失败", 500);
来源：http://hz.ppjwa.cn/gtrkzaeery.html

[U72] PHP：写错误日志
来源：http://hz.jyoumei.cn/gtigprqqhx.html

error_log("失败: " . $e->getMessage());
来源：http://hz.shanyushiyangkeji.top/gtehfkhxgd.html

[U73] PHP：读取 ini 配置
来源：http://hz.jiagoushi.top/gttiqvkdqh.html

parse_ini_file("config.ini", true)
来源：http://hz.0kj1m.cn/gtzpuousdi.html

[U74] PHP：读取环境变量
来源：http://hz.sysykeji.top/gtxoynjqhf.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yongpay.top/gtlhdrsfau.html

[U75] PHP：依赖注入
来源：http://hz.zhongyouzk.top/gtcikqxflv.html

composer require psr/container
来源：http://hz.gogol.net.cn/gtngamdeer.html

[U76] PHP：简单路由
来源：http://hz.wangshuangyany.cn/gtmxkljeqa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yj20258.top/gtvcfndtbk.html

[U77] PHP：模板渲染
来源：http://hz.zhongyouzk.top/gtoupayslz.html

composer require twig/twig
来源：http://hz.sxryk.cn/gtlfyknihh.html

[U78] PHP：单元测试
来源：http://hz.zhongyouzk.top/gtmsntcrxk.html

composer require --dev phpunit/phpunit
来源：http://hz.tianlin.xyz/gtqxlmhxih.html

[U79] PHP：静态分析
来源：http://hz.ydjk.org.cn/gtclftpyek.html

composer require --dev phpstan/phpstan
来源：http://hz.guannengcc.top/gtkoboeoqa.html

[U80] PHP：代码规范修复
来源：http://hz.zycfv.cn/gthrvgafmu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.52xcode.cn/gtuwjryoui.html

[U81] JS：初始化项目
来源：http://hz.iojbl.cn/gtscykwxcx.html

npm init -y;  npm i express
来源：http://hz.pycfn.com/gthbdbexuk.html

[U82] JS：package.json 脚本
来源：http://hz.gaohongyu789.top/gtmyjtilqs.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.sysykeji.top/gtanrdhpqa.html

[U83] JS：ES Module 导入导出
来源：http://hz.nanxinkj.top/gtwvzaifbb.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yj20258.top/gtvpbwlghf.html

[U84] JS：CommonJS 写法
来源：http://hz.bjfxy.top/gtqtgvecyw.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.hnxiangtu.top/gtwbfdfgxm.html

[U85] JS：可选链
来源：http://hz.hfpthk.cn/gtcruulyug.html

a?.b?.c
来源：http://hz.ppjwa.cn/gtxlwtdhbq.html

[U86] JS：空值合并
来源：http://hz.sxryk.cn/gtigclwapd.html

a ?? b
来源：http://hz.yanxiufei.cn/gtbxmwsknj.html

[U87] JS：解构默认值
来源：http://hz.bjfxy.top/gtrubvkkds.html

const { a = 1, b = 2 } = obj;
来源：http://hz.cashguo.top/gtfrhwdmbj.html

[U88] JS：对象展开合并
来源：http://hz.zycfv.cn/gtpwxtgilz.html

{ ...a, ...b }
来源：http://hz.jinyuanbaomall.cn/gtbyuqtowu.html

[U89] JS：数组去重
来源：http://hz.yanxiufei.cn/gtuxdjczol.html

[...new Set(arr)]
来源：http://hz.wangdashe.top/gtmuxkofmj.html

[U90] JS：数字数组排序
来源：http://hz.shzxlz.cn/gtzzlrxgqx.html

[...arr].sort((a, b) => a - b)
来源：http://hz.iojbl.cn/gtcbvpqprp.html

[U91] JS：对象键值遍历
来源：http://hz.gaohongyu789.top/gtesavbsvo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.kuanghao11.cn/gtsoavumhx.html

[U92] JS：深拷贝
来源：http://hz.nanxuanxn.top/gtpnlfeove.html

structuredClone(obj)
来源：http://hz.xuanzx.com/gtnakimyot.html

[U93] JS：模板字符串
来源：http://hz.sysykeji.top/gtjhdkkwut.html

`共 ${n} 条`
来源：http://hz.iojbl.cn/gtkgmyuavb.html

[U94] JS：箭头函数
来源：http://hz.tanke756.top/gtiwqmpbyf.html

const double = x => x * 2;
来源：http://hz.snrcjt.cn/gtzghmsqmx.html

[U95] JS：Promise 包装
来源：http://hz.meibo888.top/gtcmrctfsl.html

new Promise((resolve, reject) => {})
来源：http://hz.tianlin.xyz/gteymdxjlb.html

[U96] JS：async/await 与异常
来源：http://hz.tian-w.cn/gteucvwzqs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yongpay.top/gtggdakgtt.html

[U97] JS：并发请求
来源：http://hz.jqgfzy.top/gtdbnohrik.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hongshengwenyu.top/gtsudpjoff.html

[U98] JS：fetch 带 JSON
来源：http://hz.chenjidiqi.icu/gtjukvpttv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.c1oappe.top/gtapklsmqj.html

[U99] JS：事件监听
来源：http://hz.jinqigufen.top/gtvvfgxvzh.html

el.addEventListener("click", e => {})
来源：http://hz.havefunace.top/gtkugbuoaa.html

[U100] JS：DOM 查询
来源：http://hz.sufxvd.cn/gtqjfiasjp.html

document.querySelector(".item")
来源：http://hz.shuidangran.top/gttlpnjjsu.html

[U101] JS：classList 操作
来源：http://hz.hnxiangtu.top/gtqtdahuqe.html

el.classList.toggle("active")
来源：http://hz.yvedp.cn/gtisdlhiek.html

[U102] JS：本地存储
来源：http://hz.pengpengdd.cyou/gtirrxcnkr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.nanxinkj.top/gtczyteluo.html

[U103] JS：定时器
来源：http://hz.zhengqikj.top/gtwojesdxs.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.daxiang520.top/gtnvpwhytz.html

[U104] JS：防抖
来源：http://hz.guowangkeji.top/gtviyjmgtm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cheryme.top/gtgwiwuoph.html

[U105] JS：节流
来源：http://hz.jqgufenzy.top/gtzbgxbpcg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jqgfzy.top/gtxxihcaxm.html

[U106] JS：日期格式化
来源：http://hz.daxiang520.top/gtqrqjcfok.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yongpay.top/gtodjhaasy.html

[U107] JS：数字千分位
来源：http://hz.zhongyouzk.top/gtgjugbzxd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.nanxinkj.top/gtplnaqxvt.html

[U108] JS：随机整数
来源：http://hz.c1oappe.top/gtajmaqgot.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.tanke756.top/gtubhafzwz.html

[U109] JS：数组分组
来源：http://hz.mhx1999.top/gtajzvetab.html

Object.groupBy(arr, x => x.type)
来源：http://hz.52xcode.cn/gtbsrnkxus.html

[U110] JS：数组分块
来源：http://hz.shanyushiyangkeji.top/gtcyhtkkcp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.cdnleiting.top/gtzmogaegc.html

[U111] JS：对象转 Map
来源：http://hz.52xcode.cn/gtvynzvyim.html

new Map(Object.entries(obj))
来源：http://hz.0kj1m.cn/gtaftwsssm.html

[U112] JS：字符串补位
来源：http://hz.cashguo.top/gtbgsrxiox.html

"7".padStart(3, "0")
来源：http://hz.ydzc1.top/gtpcbtxzot.html

[U113] JS：正则替换全部
来源：http://hz.sweek.top/gtxyiybgig.html

s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gtkpuvhmiz.html

[U114] JS：JSON 深比较
来源：http://hz.zhaomingkeji.xyz/gtgjzjbpqz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj20258888.top/gtvxakcooi.html

[U115] JS：生成 UUID
来源：http://hz.quarkkingdee.top/gtubodjrcl.html

crypto.randomUUID()
来源：http://hz.316326.xyz/gtzdygdgdm.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jlsjyb.cn/gtnxjhyzho.html

/** @param {string} name */ function f(name) {}
来源：http://hz.guannengcc.top/gtlqcwrsdt.html

[U117] JS：单元测试
来源：http://hz.ivvv.top/gtlzlolvrq.html

npm i -D vitest;  npx vitest
来源：http://hz.wangshuangyany.cn/gtwioepuln.html

[U118] JS：开发服务器
来源：http://hz.mhx1999.top/gtqjyybcnx.html

npm i -D vite;  npx vite
来源：http://hz.hongshengwenyu.top/gtbrnzhigq.html

[U119] JS：生产构建
来源：http://hz.zhengqikj.top/gtffiqladk.html

npx vite build
来源：http://hz.cdnleiting.top/gtzkqtvnsu.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.smart0.xyz/gtvdgumwza.html

import.meta.env.VITE_API_URL
来源：http://hz.aizwys.cn/gtyguoqisi.html

================================================================================
来源：http://hz.guannengcc.top/gtgwampcup.html

统计汇总
来源：http://hz.yvedp.cn/gtewtqhsil.html

================================================================================
来源：http://hz.zycfv.cn/gtrnzkwcsb.html

按语言统计（条）：
来源：http://hz.c1oappe.top/gtbuewbqfq.html

Python ......... 252
来源：http://hz.ydzc1.top/gtwxjoqgmc.html

PHP ............ 252
来源：http://hz.zhijiandao.cn/gtidnvdbjv.html

JavaScript ..... 252
来源：http://hz.c1oappe.top/gtzgbkgfew.html

TypeScript ..... 212
来源：http://hz.quarkkingdee.top/gtcpgsoixq.html

Java ........... 212
来源：http://hz.jinqigufen.top/gtrpefxmqi.html

Go ............. 212
来源：http://hz.xinyue.icu/gtnnrdeubh.html

Ruby ........... 212
来源：http://hz.dianchejie.cn/gtqzofrlyy.html

C# ............. 212
来源：http://hz.zhongyouzk.top/gtqsjtxvva.html

C .............. 30
来源：http://hz.zhixingplan.top/gtrgqlhyed.html

C++ ............ 30
来源：http://hz.bjfxy.top/gteapfoynm.html

SQL ............ 90
来源：http://hz.yueranfly.top/gthusjmtbc.html

Bash ........... 80
来源：http://hz.hnqzz.top/gtgsqjgrrv.html

Kotlin ......... 15
来源：http://hz.zdqjudy.top/gtnzyaqcig.html

Swift .......... 15
来源：http://hz.wangshuangyany.cn/gtgvnwruhn.html

Lua ............ 10
来源：http://hz.yj202588.top/gtoticqnhw.html

Perl ........... 10
来源：http://hz.dashuyun.cn/gtfydvwtgd.html

Scala .......... 10
来源：http://hz.hysaishi.cn/gtmtgzzqgv.html

------------------------------------
来源：http://hz.cheryme.top/gtwjetktyn.html

合计 ........... 2106 条
来源：http://hz.tanke756.top/gtkxkfiwcz.html

按章节统计：
来源：http://hz.zdqjudy.top/gtfnsyhgww.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.havefunace.top/gtluifacsc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.nanxuanxn.top/gtociiphcv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.dianchejie.cn/gtaudrhlug.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.bjfxy.top/gtrqqwilso.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.xingfuxueyuan.xyz/gtergwcyfd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jyoumei.cn/gthqgtwhyk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.ivvv.top/gtfcnhwcgr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.havefunace.top/gtetkupqss.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.xinyue.icu/gtsihhowgw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.kuanghao11.cn/gtgewnfsrj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhixingplan.top/gthtjspqaf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.pycfn.com/gtukdowgwn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.aizwys.cn/gtlblrvrit.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.aizwys.cn/gtcgmayspe.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.ivvv.top/gtyabjnass.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jinqigfzy.top/gtojwkapbf.html


<!-- 参考信息 -->