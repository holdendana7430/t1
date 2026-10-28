代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://hz.dianchejie.cn/gtofhemafq.html

[T55] Scala：集合过滤
来源：http://hz.jlsjyb.cn/gttqccjccl.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hfpthk.cn/gtrkruzuwz.html

[T56] Scala：样例类
来源：http://hz.gzhubu.top/gthxovzcbm.html

case class User(name: String, age: Int)
来源：http://hz.snrcjt.cn/gtxfzsvbeb.html

[T57] Scala：模式匹配
来源：http://hz.zhixingplan.top/gtqlwpdvln.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.dianchejie.cn/gtsjwnymab.html

[T58] Scala：函数定义
来源：http://hz.chenzaomai.com/gtswzutwrm.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhongyouzk.top/gtnsxiwcep.html

[T59] Scala：循环
来源：http://hz.yonumen.top/gtnzkbocme.html

for (i <- 1 to 10) println(i)
来源：http://hz.jinqigufen.top/gtqlyisakt.html

[T60] Scala：折叠
来源：http://hz.hywenlv.cn/gteztduucw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xingfuxueyuan.xyz/gtytwphlit.html

================================================================================
来源：http://hz.9152youxi.cn/gtutgazhzq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yvedp.cn/gtwcrcvyif.html

================================================================================
来源：http://hz.hnxiangtu.top/gtuluuygub.html

[U01] Py：创建虚拟环境
来源：http://hz.gaohongyu789.top/gtzefcrlob.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xingfuxueyuan.xyz/gtztnlovmh.html

[U02] Py：导出 / 安装依赖
来源：http://hz.sxryk.cn/gtldlbufov.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.nanxuanxn.top/gtkazonxow.html

[U03] Py：加载 .env 配置
来源：http://hz.tanke756.top/gtyypaeriv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.haohaochexian.top/gtxitfbxsf.html

[U04] Py：变量调试打印
来源：http://hz.ehwqpu.com/gtygjnxqrn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.gzhubu.top/gtepcyqcmt.html

[U05] Py：列表去重且保序
来源：http://hz.nanxinkj.top/gtjdstiazc.html

list(dict.fromkeys(arr))
来源：http://hz.vqdsnc.cn/gtlltfzzih.html

[U06] Py：合并两个字典
来源：http://hz.0kj1m.cn/gttbpfchbu.html

{**a, **b}
来源：http://hz.yuanzhike.top/gtoumpjfqp.html

[U07] Py：反转字典键值
来源：http://hz.jqgfzy.top/gtoogbnjje.html

{v: k for k, v in d.items()}
来源：http://hz.zhixingplan.top/gtenpsusyn.html

[U08] Py：展平二维列表
来源：http://hz.yongpay.top/gtzozdtjqo.html

[y for x in nested for y in x]
来源：http://hz.yueranfly.top/gtgjbkdbek.html

[U09] Py：字典取最大值的键
来源：http://hz.yvedp.cn/gtxwmfxlvl.html

max(d, key=d.get)
来源：http://hz.52xcode.cn/gtbnehkjqt.html

[U10] Py：按值排序字典
来源：http://hz.haohaochexian.top/gtvjfiniga.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.sufxvd.cn/gtlzcazhsc.html

[U11] Py：生成器表达式
来源：http://hz.0kj1m.cn/gtjayzewfo.html

(x * 2 for x in arr)
来源：http://hz.guowangkeji.top/gtbzmvtddo.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.shuidangran.top/gtcqvwdyux.html

Counter(arr).most_common(3)
来源：http://hz.0kj1m.cn/gtsfkcyjja.html

[U13] Py：固定长度队列
来源：http://hz.gzhubu.top/gtkdyleudj.html

deque(maxlen=10)
来源：http://hz.yuanzhike.top/gtjcrffkhn.html

[U14] Py：分组收集到列表
来源：http://hz.ivvv.top/gthtqpdwas.html

defaultdict(list)
来源：http://hz.jinyuanbaomall.cn/gtsxaeequm.html

[U15] Py：高精度计时
来源：http://hz.andypj.xyz/gtkhilznxl.html

t = time.perf_counter()
来源：http://hz.ydjk.org.cn/gttdgwvnjk.html

[U16] Py：命令行参数解析
来源：http://hz.hongshengwenyu.top/gtruxfrzlz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.haohaochexian.top/gtyzvwijhd.html

[U17] Py：初始化日志
来源：http://hz.cucudq.cn/gtxuhrcsrn.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yj202588.top/gtfahfdvac.html

[U18] Py：预编译正则
来源：http://hz.hnxiangtu.top/gtkpvxmxhn.html

pat = re.compile(r"\d+")
来源：http://hz.nwbrower.top/gtohwyjulz.html

[U19] Py：正则替换带回调
来源：http://hz.xziqi.cn/gttrcdoble.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.kuanghao11.cn/gtkdffjxfw.html

[U20] Py：缓存函数结果
来源：http://hz.cashguo.top/gtmrvduwfh.html

@functools.lru_cache(maxsize=None)
来源：http://hz.gotoacloud.top/gtcosljuso.html

[U21] Py：自定义上下文管理器
来源：http://hz.daxiang520.top/gtzdrbcjry.html

@contextlib.contextmanager
来源：http://hz.hywenlv.cn/gteotwhvwr.html

[U22] Py：矩阵转置
来源：http://hz.yongpay.top/gtasdvwfvo.html

list(zip(*m))
来源：http://hz.cucudq.cn/gtreowerpb.html

[U23] Py：分块读取大文件
来源：http://hz.hnxiangtu.top/gtdivxcmvm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ppjwa.cn/gtbmsbjokr.html

[U24] Py：路径操作
来源：http://hz.cqqwz.cn/gteyjhyfqi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.0kj1m.cn/gtdkkgniyu.html

[U25] Py：CSV 按字典读
来源：http://hz.fengsongda.top/gtrbtqhvvn.html

csv.DictReader(f)
来源：http://hz.shzxlz.cn/gtlrdbwhcu.html

[U26] Py：并发下载
来源：http://hz.ywan-chungtsiang.top/gtygpwjiwh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.shuidangran.top/gttlcfrzfl.html

[U27] Py：异步 HTTP
来源：http://hz.zhongyouzk.top/gtplsihmfr.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.shzxlz.cn/gtulschhva.html

[U28] Py：类型别名
来源：http://hz.shangyingyoupin.top/gtkisxyuam.html

UserId = int
来源：http://hz.zhixingplan.top/gtxlazfjvr.html

[U29] Py：属性校验
来源：http://hz.dianchejie.cn/gtrcqjqcvv.html

@property 与 @x.setter 配合
来源：http://hz.guannengcc.top/gtzcopmfga.html

[U30] Py：数据类
来源：http://hz.ppjwa.cn/gtwzvpvukh.html

@dataclass(slots=True)
来源：http://hz.vqdsnc.cn/gtcwqgtjxi.html

[U31] Py：单测
来源：http://hz.shuidangran.top/gtoupypbac.html

python -m pytest -q
来源：http://hz.kuanghao11.cn/gttnuuvelp.html

[U32] Py：代码格式化
来源：http://hz.nanxinkj.top/gtofptpyal.html

ruff format . && ruff check --fix .
来源：http://hz.hysaishi.cn/gtmjylqktb.html

[U33] Py：打包发布
来源：http://hz.yueranfly.top/gtrxozhnys.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.svipenyu.cn/gticgpigkj.html

[U34] Py：判断编码
来源：http://hz.kuanghao11.cn/gtzergxpeo.html

chardet.detect(raw)
来源：http://hz.ydzc1.top/gtnbebmsaq.html

[U35] Py：发送邮件
来源：http://hz.redwolf501.top/gtmlggnkea.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.nwbrower.top/gtvhgokwpn.html

[U36] Py：定时任务
来源：http://hz.hywenlv.cn/gtelnymbfb.html

schedule.every(10).minutes.do(job)
来源：http://hz.sufxvd.cn/gtusrtdyxu.html

[U37] Py：读写 Excel
来源：http://hz.pycfn.com/gtcbhqcmzv.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.bjfxy.top/gtlcxchrjl.html

[U38] Py：获取脚本所在目录
来源：http://hz.ywan-chungtsiang.top/gtnmzccerd.html

Path(__file__).resolve().parent
来源：http://hz.birdmap.top/gtiobfcojw.html

[U39] Py：判断是否在交互环境
来源：http://hz.hywenlv.cn/gtczftqyip.html

sys.stdout.isatty()
来源：http://hz.hywenlv.cn/gtisxtmhql.html

[U40] Py：打印到标准错误
来源：http://hz.sweek.top/gtkuduubal.html

print("err", file=sys.stderr)
来源：http://hz.svipenyu.cn/gtjoeclghk.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.wangshuangyany.cn/gtlkzhdtgo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jyoumei.cn/gtvsqytnuo.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.dianchejie.cn/gtetzmlkij.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yj20258.top/gtncotmcwg.html

[U43] PHP：声明命名空间
来源：http://hz.sweek.top/gtgrslfqzc.html

namespace App\Http;
来源：http://hz.bjfxy.top/gtdoxtours.html

[U44] PHP：开启严格类型
来源：http://hz.tianlin.xyz/gtwwxzmwgo.html

declare(strict_types=1);
来源：http://hz.zhiwuduotai.top/gtjbdyokiu.html

[U45] PHP：类型声明与返回类型
来源：http://hz.316326.xyz/gtrwwouomg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj202588.top/gtmmcjrkmv.html

[U46] PHP：可空类型
来源：http://hz.redwolf501.top/gtehxqbpdu.html

?string $name = null
来源：http://hz.zhaomingkeji.xyz/gtdaxwtxzo.html

[U47] PHP：联合类型
来源：http://hz.c1oappe.top/gtrojqguel.html

int|string $id
来源：http://hz.c1oappe.top/gtmenywylh.html

[U48] PHP：纯枚举
来源：http://hz.gogol.net.cn/gtrsvicxtx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.gotoacloud.top/gtqrbeqmzo.html

[U49] PHP：只读属性
来源：http://hz.zhengqikj.top/gtjcdskblq.html

public readonly string $name
来源：http://hz.yj20258.top/gtjyxiqvri.html

[U50] PHP：构造器属性提升
来源：http://hz.daxiang520.top/gtsbitaqjm.html

public function __construct(private int $id) {}
来源：http://hz.sxryk.cn/gtqgbptdcr.html

[U51] PHP：数组解构
来源：http://hz.hysaishi.cn/gtjattokds.html

[$a, $b] = $arr;
来源：http://hz.redwolf501.top/gtntzthqaj.html

[U52] PHP：箭头函数
来源：http://hz.snrcjt.cn/gtqrjotcmy.html

$double = fn($x) => $x * 2;
来源：http://hz.zhengqikj.top/gtnfrywuqw.html

[U53] PHP：空合并运算符
来源：http://hz.chenlongwang.top/gttejxiknr.html

$v = $a ?? $b ?? "default";
来源：http://hz.yongpay.top/gtfbwlbgmq.html

[U54] PHP：空安全调用
来源：http://hz.zycfv.cn/gtctffjmrw.html

$obj?->method()
来源：http://hz.yueranfly.top/gtmuqnfypi.html

[U55] PHP：match 表达式
来源：http://hz.0kj1m.cn/gthqcbwgfp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.daxiang520.top/gtoskiocnu.html

[U56] PHP：命名参数
来源：http://hz.zhoulong.xyz/gtefxeatga.html

f(a: 1, b: 2)
来源：http://hz.yanxiufei.cn/gtrjnwfdqz.html

[U57] PHP：字符串插值
来源：http://hz.gaohongyu789.top/gtpwouurvd.html

"值: {$a}"
来源：http://hz.ivvv.top/gthnulysxm.html

[U58] PHP：数组三件套
来源：http://hz.yanxiufei.cn/gtbojmgvnu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.shanyushiyangtech.top/gtwisisppy.html

[U59] PHP：自定义排序
来源：http://hz.xingfuxueyuan.xyz/gtakdhmorn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jyoumei.cn/gtkdlavyrr.html

[U60] PHP：JSON 编解码
来源：http://hz.snrcjt.cn/gtqyzywyee.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.xuanzx.com/gtzxgfszat.html

[U61] PHP：正则
来源：http://hz.52xcode.cn/gtadzaciyx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.tanke756.top/gtmjgkdauc.html

[U62] PHP：日期对象
来源：http://hz.tian-w.cn/gtugflxgsc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zhiwuduotai.top/gtmyrykyuv.html

[U63] PHP：文件读写
来源：http://hz.mhx1999.top/gtilkbwynm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.cucudq.cn/gtuandzrqy.html

[U64] PHP：目录遍历
来源：http://hz.shangyingyoupin.top/gtwetrykob.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.shanyushiyangtech.top/gtsehhhiqj.html

[U65] PHP：会话
来源：http://hz.yvedp.cn/gtdcgnkzat.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.nanxinkj.top/gtxxvspmpl.html

[U66] PHP：设置 Cookie
来源：http://hz.iojbl.cn/gtefhowwjl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yuxming.cn/gtqlxucnga.html

[U67] PHP：处理文件上传
来源：http://hz.chenjidiqi.icu/gtuhzriedn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jinyuanbaomall.cn/gtsezukgiu.html

[U68] PHP：PDO 连接
来源：http://hz.jlsjyb.cn/gtrogbmxpn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xingfuxueyuan.xyz/gtlkkareef.html

[U69] PHP：PDO 预处理
来源：http://hz.ywan-chungtsiang.top/gtkeoycjne.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.mhx1999.top/gtjyysdevq.html

[U70] PHP：PDO 事务
来源：http://hz.yangfankeji.com/gtxacgbsuw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yueranfly.top/gtormcoizq.html

[U71] PHP：抛出异常
来源：http://hz.chenjidiqi.icu/gtxcinpqpz.html

throw new RuntimeException("失败", 500);
来源：http://hz.redwolf501.top/gtoicfxhkm.html

[U72] PHP：写错误日志
来源：http://hz.yj20258888.top/gtvzquvfvc.html

error_log("失败: " . $e->getMessage());
来源：http://hz.haohaochexian.top/gtmnfvnwmk.html

[U73] PHP：读取 ini 配置
来源：http://hz.vqdsnc.cn/gtteoiqdxk.html

parse_ini_file("config.ini", true)
来源：http://hz.daxiang520.top/gtlnbiikkt.html

[U74] PHP：读取环境变量
来源：http://hz.shanyushiyangtech.top/gtfmuhkrsd.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hammf.cn/gtyhjdqsai.html

[U75] PHP：依赖注入
来源：http://hz.yonumen.top/gtewziwrym.html

composer require psr/container
来源：http://hz.jinghuilouyu.cn/gtzxlamzji.html

[U76] PHP：简单路由
来源：http://hz.guannengcc.top/gtmxzaigon.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.ybcxt.top/gtgsqrjxhd.html

[U77] PHP：模板渲染
来源：http://hz.smart0.xyz/gtqdkcegmt.html

composer require twig/twig
来源：http://hz.chenlongwang.top/gtcjnorbio.html

[U78] PHP：单元测试
来源：http://hz.hywenlv.cn/gtjydxqpqn.html

composer require --dev phpunit/phpunit
来源：http://hz.dianchejie.cn/gtwpvwoqih.html

[U79] PHP：静态分析
来源：http://hz.fzhhl.top/gtgitdqtpj.html

composer require --dev phpstan/phpstan
来源：http://hz.daxiang520.top/gtrawdcwqc.html

[U80] PHP：代码规范修复
来源：http://hz.52xcode.cn/gttbaqgywy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.ydzc1.top/gtmfrjihhg.html

[U81] JS：初始化项目
来源：http://hz.zhengqikj.top/gtawjhggyh.html

npm init -y;  npm i express
来源：http://hz.xylfe.cn/gtlxjweykg.html

[U82] JS：package.json 脚本
来源：http://hz.zhengqikj.top/gtkqzipulq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yuxming.cn/gtzqjzdiyz.html

[U83] JS：ES Module 导入导出
来源：http://hz.ehwqpu.com/gtlgpouyvu.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.shanyushiyangkeji.top/gtyxlvmowj.html

[U84] JS：CommonJS 写法
来源：http://hz.gzhubu.top/gtwnmfzjod.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.52xcode.cn/gttxshtqwd.html

[U85] JS：可选链
来源：http://hz.shanyushiyangkeji.top/gtouyargtx.html

a?.b?.c
来源：http://hz.iojbl.cn/gtexggihan.html

[U86] JS：空值合并
来源：http://hz.chenlongwang.top/gtsjvzcsho.html

a ?? b
来源：http://hz.cdnleiting.top/gtrboesdjr.html

[U87] JS：解构默认值
来源：http://hz.hongshengwenyu.top/gtgjjcpzxo.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jyoumei.cn/gtylfrgrfo.html

[U88] JS：对象展开合并
来源：http://hz.hywenlv.cn/gtaiecexyu.html

{ ...a, ...b }
来源：http://hz.jlsjyb.cn/gtrvpcpfyi.html

[U89] JS：数组去重
来源：http://hz.yonumen.top/gtmcjdhqrr.html

[...new Set(arr)]
来源：http://hz.yj20258.top/gtarakosiw.html

[U90] JS：数字数组排序
来源：http://hz.xziqi.cn/gtzerkjhpb.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yuxming.cn/gtsnadzhwb.html

[U91] JS：对象键值遍历
来源：http://hz.zdqjudy.top/gtzxxhfnoc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.52xcode.cn/gtxzdqiabu.html

[U92] JS：深拷贝
来源：http://hz.jyoumei.cn/gtjxbvqdrk.html

structuredClone(obj)
来源：http://hz.nanxuanxn.top/gtktcpzavl.html

[U93] JS：模板字符串
来源：http://hz.jinghuilouyu.cn/gtdbjexwwc.html

`共 ${n} 条`
来源：http://hz.aizwys.cn/gtkjmcrxkh.html

[U94] JS：箭头函数
来源：http://hz.yueranfly.top/gtsutglayn.html

const double = x => x * 2;
来源：http://hz.vqdsnc.cn/gthvlomwaw.html

[U95] JS：Promise 包装
来源：http://hz.iojbl.cn/gtzgtzxpir.html

new Promise((resolve, reject) => {})
来源：http://hz.sxryk.cn/gtzvuztowe.html

[U96] JS：async/await 与异常
来源：http://hz.gogol.net.cn/gtskpjewxi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.gotoacloud.top/gtfgowrgsj.html

[U97] JS：并发请求
来源：http://hz.gotoacloud.top/gtgcpqhhfr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtyxdnkjlw.html

[U98] JS：fetch 带 JSON
来源：http://hz.gotoacloud.top/gttgcgzysh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hywenlv.cn/gtuhnfnwyp.html

[U99] JS：事件监听
来源：http://hz.zhengqikj.top/gtnqysrqxc.html

el.addEventListener("click", e => {})
来源：http://hz.jyoumei.cn/gtubemxrnd.html

[U100] JS：DOM 查询
来源：http://hz.daria6918.cn/gtmdrhzbjl.html

document.querySelector(".item")
来源：http://hz.aizwys.cn/gtvakvfesv.html

[U101] JS：classList 操作
来源：http://hz.sweek.top/gtydtlebaw.html

el.classList.toggle("active")
来源：http://hz.cheryme.top/gtpuehwpge.html

[U102] JS：本地存储
来源：http://hz.gzhubu.top/gtsdovqjwh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ehwqpu.com/gtryfxnoqb.html

[U103] JS：定时器
来源：http://hz.zhixingplan.top/gtjdpqtvrf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.c1oappe.top/gtmplqlrwx.html

[U104] JS：防抖
来源：http://hz.yuxming.cn/gtmerrlnzp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cashguo.top/gtvnrcksqh.html

[U105] JS：节流
来源：http://hz.zdqjudy.top/gtlfpkvxaf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ppjwa.cn/gtqajxmtpm.html

[U106] JS：日期格式化
来源：http://hz.jinyuanbaomall.cn/gtbfcawndp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhaomingkeji.xyz/gturibjfmo.html

[U107] JS：数字千分位
来源：http://hz.hysaishi.cn/gtfzelldvw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jyoumei.cn/gtwjsfsaib.html

[U108] JS：随机整数
来源：http://hz.shanyushiyangtech.top/gtubiqdbmg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jqgfzy.top/gtjurnkfht.html

[U109] JS：数组分组
来源：http://hz.yuanzhike.top/gtbjnykahu.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jianghu66.top/gtjckmszqp.html

[U110] JS：数组分块
来源：http://hz.haohaochexian.top/gtblhexatz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.guowangkeji.top/gtetacvlah.html

[U111] JS：对象转 Map
来源：http://hz.bjfxy.top/gtatglxzhl.html

new Map(Object.entries(obj))
来源：http://hz.svipenyu.cn/gttlzuxeue.html

[U112] JS：字符串补位
来源：http://hz.cucudq.cn/gtrhugpnql.html

"7".padStart(3, "0")
来源：http://hz.yangfankeji.com/gtrqcvderr.html

[U113] JS：正则替换全部
来源：http://hz.pycfn.com/gtmkbebdgr.html

s.replaceAll("a", "b")
来源：http://hz.tian-w.cn/gtmgjonddz.html

[U114] JS：JSON 深比较
来源：http://hz.smart0.xyz/gtgkojdaek.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.vqdsnc.cn/gtxkfejhgb.html

[U115] JS：生成 UUID
来源：http://hz.c1oappe.top/gtvcnvbkhz.html

crypto.randomUUID()
来源：http://hz.fengsongda.top/gtglygfeva.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.nwbrower.top/gttvoimqkb.html

/** @param {string} name */ function f(name) {}
来源：http://hz.fengsongda.top/gtxwhzssiz.html

[U117] JS：单元测试
来源：http://hz.shanyushiyangtech.top/gtwqanfxvt.html

npm i -D vitest;  npx vitest
来源：http://hz.nanxuanxn.top/gtbqmswlpa.html

[U118] JS：开发服务器
来源：http://hz.chenjidiqi.icu/gtkahbpncv.html

npm i -D vite;  npx vite
来源：http://hz.jqgufenzy.top/gtohovsuvb.html

[U119] JS：生产构建
来源：http://hz.chenzaomai.com/gtxturfctn.html

npx vite build
来源：http://hz.yj20258888.top/gtfvvnbhsp.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.sxryk.cn/gtqjtsseqs.html

import.meta.env.VITE_API_URL
来源：http://hz.zhiwuduotai.top/gtgnhogmnd.html

================================================================================
来源：http://hz.guannengcc.top/gttrbkyijs.html

统计汇总
来源：http://hz.hnxiangtu.top/gtqrayrfbb.html

================================================================================
来源：http://hz.yangfankeji.com/gtulequxut.html

按语言统计（条）：
来源：http://hz.jyoumei.cn/gtigbqdnut.html

Python ......... 252
来源：http://hz.zhongyouzk.top/gtjeoecvpk.html

PHP ............ 252
来源：http://hz.jinghuilouyu.cn/gtwxmmvkcn.html

JavaScript ..... 252
来源：http://hz.quarkkingdee.top/gtakbqqdcd.html

TypeScript ..... 212
来源：http://hz.yonumen.top/gtlcdqsuse.html

Java ........... 212
来源：http://hz.pengpengdd.cyou/gtlbeovass.html

Go ............. 212
来源：http://hz.chenlongwang.top/gtrdbpkbba.html

Ruby ........... 212
来源：http://hz.shanyushiyangtech.top/gtcfuopjlw.html

C# ............. 212
来源：http://hz.sxryk.cn/gtuegurevi.html

C .............. 30
来源：http://hz.yanxiufei.cn/gtnwblhixw.html

C++ ............ 30
来源：http://hz.gogol.net.cn/gtsoozmygk.html

SQL ............ 90
来源：http://hz.quarkkingdee.top/gtvgicufsh.html

Bash ........... 80
来源：http://hz.xylfe.cn/gtwvgiextu.html

Kotlin ......... 15
来源：http://hz.wangshuangyany.cn/gtzsrtitto.html

Swift .......... 15
来源：http://hz.quarkkingdee.top/gtarnuxbxm.html

Lua ............ 10
来源：http://hz.sxryk.cn/gtwwwfkcrl.html

Perl ........... 10
来源：http://hz.yanxiufei.cn/gthzlzrpnh.html

Scala .......... 10
来源：http://hz.hywenlv.cn/gtuquxswsf.html

------------------------------------
来源：http://hz.iojbl.cn/gtdbbzbbry.html

合计 ........... 2106 条
来源：http://hz.hfpthk.cn/gtnukuhksa.html

按章节统计：
来源：http://hz.yueranfly.top/gtdcwreilg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jianghu66.top/gtvjpqxrte.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.meibo888.top/gtxxtrpfpc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.pengpengdd.cyou/gtuquhzvwy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zycfv.cn/gtmftkoozd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.fzhhl.top/gtogtabvfc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.feifeiyinyue.top/gthypjumnq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.quarkkingdee.top/gtqnrycjxy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yuxming.cn/gttkhvdlsd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.daria6918.cn/gtmabhsldk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.shangyingyoupin.top/gtdgogbrio.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yvedp.cn/gtisvcesqe.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.vqdsnc.cn/gtodgbhopb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.tanke756.top/gtenadipwh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.chenzaomai.com/gtelptnomf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yangfankeji.com/gtbarmhose.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.hnqzz.top/gtldpzodhd.html

Q SQL 专题                              90
来源：http://hz.pycfn.com/gtfvyyamfk.html

R Bash 专题                             80
来源：http://hz.xylfe.cn/gthgimgmqj.html

S C / C++ 专题                          60
来源：http://hz.redwolf501.top/gttgfjtpwz.html

T 其他语言补充                          60
来源：http://hz.wangdashe.top/gtuqzdoimf.html


<!-- 参考信息 -->