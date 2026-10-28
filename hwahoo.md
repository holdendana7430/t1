代发 wailian999

[U03] Py：加载 .env 配置
来源：http://hz.jqgfzy.top/gtvcixmatw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zycfv.cn/gttwbkxjer.html

[U04] Py：变量调试打印
来源：http://hz.dianchejie.cn/gtpvhtlybh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.andypj.xyz/gtdvokibbi.html

[U05] Py：列表去重且保序
来源：http://hz.gzhubu.top/gtvxuuykuk.html

list(dict.fromkeys(arr))
来源：http://hz.zhaomingkeji.xyz/gttkwdmzlq.html

[U06] Py：合并两个字典
来源：http://hz.xuanzx.com/gtvnhbwtdf.html

{**a, **b}
来源：http://hz.316326.xyz/gtvvmvqhzp.html

[U07] Py：反转字典键值
来源：http://hz.ivvv.top/gtrvxrhbkr.html

{v: k for k, v in d.items()}
来源：http://hz.sxryk.cn/gtbbktvcqh.html

[U08] Py：展平二维列表
来源：http://hz.xziqi.cn/gtzrbypqkz.html

[y for x in nested for y in x]
来源：http://hz.snrcjt.cn/gtsethvbhg.html

[U09] Py：字典取最大值的键
来源：http://hz.yuxming.cn/gthmduxabf.html

max(d, key=d.get)
来源：http://hz.ybcxt.top/gtygnrpxjo.html

[U10] Py：按值排序字典
来源：http://hz.meibo888.top/gtkzkcctbl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ywan-chungtsiang.top/gtlhtoriel.html

[U11] Py：生成器表达式
来源：http://hz.zhixingplan.top/gtibrqzamu.html

(x * 2 for x in arr)
来源：http://hz.zhengqikj.top/gtmbahplsb.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhoulong.xyz/gtuzakqhre.html

Counter(arr).most_common(3)
来源：http://hz.meibo888.top/gtifidgaxf.html

[U13] Py：固定长度队列
来源：http://hz.yanxiufei.cn/gtnqpsbblj.html

deque(maxlen=10)
来源：http://hz.hywenlv.cn/gttbgsrwye.html

[U14] Py：分组收集到列表
来源：http://hz.sxryk.cn/gtbjjuceba.html

defaultdict(list)
来源：http://hz.zhengqikj.top/gtdaegbtkc.html

[U15] Py：高精度计时
来源：http://hz.svipenyu.cn/gtdlvmeplb.html

t = time.perf_counter()
来源：http://hz.hammf.cn/gtarqwnlsn.html

[U16] Py：命令行参数解析
来源：http://hz.kuanghao11.cn/gtaxfewyit.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.fzhhl.top/gtdtvkrfdg.html

[U17] Py：初始化日志
来源：http://hz.gaohongyu789.top/gtaqmokwhr.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.shuidangran.top/gtobxpqokf.html

[U18] Py：预编译正则
来源：http://hz.sysykeji.top/gtrhynmyyq.html

pat = re.compile(r"\d+")
来源：http://hz.tian-w.cn/gtmckyycjs.html

[U19] Py：正则替换带回调
来源：http://hz.jlsjyb.cn/gtooowryqb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.sweek.top/gtdmwpmeqc.html

[U20] Py：缓存函数结果
来源：http://hz.yuanzhike.top/gtedhjdfpp.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yuxming.cn/gtlzedkukt.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhiwuduotai.top/gtibuzyhqn.html

@contextlib.contextmanager
来源：http://hz.xylfe.cn/gthovklqal.html

[U22] Py：矩阵转置
来源：http://hz.jinqigufen.top/gtppndznoa.html

list(zip(*m))
来源：http://hz.zhijiandao.cn/gtcqjhfejz.html

[U23] Py：分块读取大文件
来源：http://hz.wangshuangyany.cn/gtbsudhurr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zhengqikj.top/gtogfzelyi.html

[U24] Py：路径操作
来源：http://hz.yj202588.top/gtudlawyzv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jinqigfzy.top/gtsmbgdlbt.html

[U25] Py：CSV 按字典读
来源：http://hz.ehwqpu.com/gtmqurzusb.html

csv.DictReader(f)
来源：http://hz.quarkkingdee.top/gtskxjwgti.html

[U26] Py：并发下载
来源：http://hz.pycfn.com/gtnedxpamh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.nwbrower.top/gtxpxooexk.html

[U27] Py：异步 HTTP
来源：http://hz.gogol.net.cn/gtpphqdaeb.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.chenlongwang.top/gtuhthaush.html

[U28] Py：类型别名
来源：http://hz.havefunace.top/gtvonhtghg.html

UserId = int
来源：http://hz.sysykeji.top/gttzilodoq.html

[U29] Py：属性校验
来源：http://hz.zhoulong.xyz/gtmgivbaqv.html

@property 与 @x.setter 配合
来源：http://hz.tianlin.xyz/gteudaumzt.html

[U30] Py：数据类
来源：http://hz.cashguo.top/gtjqsfhfkm.html

@dataclass(slots=True)
来源：http://hz.cdnleiting.top/gtvuttlzum.html

[U31] Py：单测
来源：http://hz.shuidangran.top/gtystizsio.html

python -m pytest -q
来源：http://hz.fengsongda.top/gticnrkstj.html

[U32] Py：代码格式化
来源：http://hz.ydzc1.top/gtsbfmxilo.html

ruff format . && ruff check --fix .
来源：http://hz.guowangkeji.top/gtnpajgqfs.html

[U33] Py：打包发布
来源：http://hz.gogol.net.cn/gtxbxyyvtf.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.snrcjt.cn/gtqdwsgdyw.html

[U34] Py：判断编码
来源：http://hz.aizwys.cn/gtqtlklbxc.html

chardet.detect(raw)
来源：http://hz.xziqi.cn/gtugsyhpim.html

[U35] Py：发送邮件
来源：http://hz.zhengqikj.top/gtmsnwvjrb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cqqwz.cn/gtuioktctd.html

[U36] Py：定时任务
来源：http://hz.cqqwz.cn/gtcoohxcgc.html

schedule.every(10).minutes.do(job)
来源：http://hz.jqgufenzy.top/gtwcvyluxi.html

[U37] Py：读写 Excel
来源：http://hz.quarkkingdee.top/gtzcdpqtho.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.guannengcc.top/gtelhdhoop.html

[U38] Py：获取脚本所在目录
来源：http://hz.ivvv.top/gtmyzvcvej.html

Path(__file__).resolve().parent
来源：http://hz.hywenlv.cn/gtljlppnpi.html

[U39] Py：判断是否在交互环境
来源：http://hz.yonumen.top/gtzshoknnm.html

sys.stdout.isatty()
来源：http://hz.zhaomingkeji.xyz/gtllutyagn.html

[U40] Py：打印到标准错误
来源：http://hz.cucudq.cn/gtnsojzbke.html

print("err", file=sys.stderr)
来源：http://hz.andypj.xyz/gtgxzcapwv.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yongpay.top/gtsediipgz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.0kj1m.cn/gteazippqz.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.aizwys.cn/gtzfxfuvrj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.pycfn.com/gtsbsmdzek.html

[U43] PHP：声明命名空间
来源：http://hz.aibaodan.cn/gtfptruaki.html

namespace App\Http;
来源：http://hz.ydzc1.top/gtgtoirzam.html

[U44] PHP：开启严格类型
来源：http://hz.ydzc1.top/gtodhlkyms.html

declare(strict_types=1);
来源：http://hz.tianlin.xyz/gtvhdfcgki.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yuanzhike.top/gtebxyixlv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dashuyun.cn/gtaooaktzi.html

[U46] PHP：可空类型
来源：http://hz.shanyushiyangkeji.top/gtrinoogci.html

?string $name = null
来源：http://hz.yuxming.cn/gtnmgibzam.html

[U47] PHP：联合类型
来源：http://hz.jiagoushi.top/gtsciytreq.html

int|string $id
来源：http://hz.snrcjt.cn/gttfdunnck.html

[U48] PHP：纯枚举
来源：http://hz.hywenlv.cn/gtpskmkaxz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.tianlin.xyz/gttozjwjqb.html

[U49] PHP：只读属性
来源：http://hz.snrcjt.cn/gtfnqmrunc.html

public readonly string $name
来源：http://hz.cheryme.top/gtxqwcdrno.html

[U50] PHP：构造器属性提升
来源：http://hz.pycfn.com/gtwodhujvt.html

public function __construct(private int $id) {}
来源：http://hz.jyoumei.cn/gthakqbczm.html

[U51] PHP：数组解构
来源：http://hz.tianlin.xyz/gtcycmtirf.html

[$a, $b] = $arr;
来源：http://hz.ywan-chungtsiang.top/gthioagnvx.html

[U52] PHP：箭头函数
来源：http://hz.cucudq.cn/gtnomwtxrb.html

$double = fn($x) => $x * 2;
来源：http://hz.yuxming.cn/gtizofdkpf.html

[U53] PHP：空合并运算符
来源：http://hz.ppjwa.cn/gtbqmzylfa.html

$v = $a ?? $b ?? "default";
来源：http://hz.hammf.cn/gtgiudkrrz.html

[U54] PHP：空安全调用
来源：http://hz.cdnleiting.top/gtijfxiiqm.html

$obj?->method()
来源：http://hz.ydjk.org.cn/gtmzfwamgd.html

[U55] PHP：match 表达式
来源：http://hz.guowangkeji.top/gthkercahe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zycfv.cn/gtttjbxvrq.html

[U56] PHP：命名参数
来源：http://hz.jinqigfzy.top/gtofdinbsl.html

f(a: 1, b: 2)
来源：http://hz.ehwqpu.com/gtzhnkmqxa.html

[U57] PHP：字符串插值
来源：http://hz.ppjwa.cn/gtvkgqcghv.html

"值: {$a}"
来源：http://hz.zhengqikj.top/gthauwlbsy.html

[U58] PHP：数组三件套
来源：http://hz.havefunace.top/gtdftahzeu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.ybcxt.top/gtvzrihymv.html

[U59] PHP：自定义排序
来源：http://hz.feifeiyinyue.top/gtysneywre.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ppjwa.cn/gtmxnaliyy.html

[U60] PHP：JSON 编解码
来源：http://hz.svipenyu.cn/gthqqnpnmy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhijiandao.cn/gtxfuaehut.html

[U61] PHP：正则
来源：http://hz.chenzaomai.com/gtjqjbtdvg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.havefunace.top/gteeupugim.html

[U62] PHP：日期对象
来源：http://hz.yj202588.top/gthchtovvd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.nanxinkj.top/gtvtkfkkwk.html

[U63] PHP：文件读写
来源：http://hz.xuetiantiany.cn/gtnnkocgwd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.fengsongda.top/gtbuwkypse.html

[U64] PHP：目录遍历
来源：http://hz.andypj.xyz/gtmilpiqdp.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ehwqpu.com/gthhgyngsb.html

[U65] PHP：会话
来源：http://hz.wangshuangyany.cn/gtcqdiclst.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.cucudq.cn/gtpbmmgnnq.html

[U66] PHP：设置 Cookie
来源：http://hz.cucudq.cn/gtowbvqlbl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yuanzhike.top/gthnqwgpzt.html

[U67] PHP：处理文件上传
来源：http://hz.9152youxi.cn/gtcwkaklof.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.shangyingyoupin.top/gtgtwzdnei.html

[U68] PHP：PDO 连接
来源：http://hz.sxryk.cn/gtwxbuegvn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zhengqikj.top/gtrloffhlj.html

[U69] PHP：PDO 预处理
来源：http://hz.xinyue.icu/gtlgbpvwzw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.shanyushiyangtech.top/gtkvtxhwdq.html

[U70] PHP：PDO 事务
来源：http://hz.zhixingplan.top/gtveqoxrmu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.fengsongda.top/gtojeroiow.html

[U71] PHP：抛出异常
来源：http://hz.zhengqikj.top/gtjdbajamz.html

throw new RuntimeException("失败", 500);
来源：http://hz.guowangkeji.top/gthglrsvhp.html

[U72] PHP：写错误日志
来源：http://hz.yuxming.cn/gtkxbdpgbh.html

error_log("失败: " . $e->getMessage());
来源：http://hz.xylfe.cn/gtzbqgixut.html

[U73] PHP：读取 ini 配置
来源：http://hz.dianchejie.cn/gtujcmppqv.html

parse_ini_file("config.ini", true)
来源：http://hz.fzhhl.top/gtvboaufsy.html

[U74] PHP：读取环境变量
来源：http://hz.52xcode.cn/gtdktdvomm.html

getenv("APP_ENV") ?: "production"
来源：http://hz.xuetiantiany.cn/gtqxuczabl.html

[U75] PHP：依赖注入
来源：http://hz.zycfv.cn/gtigrytunz.html

composer require psr/container
来源：http://hz.hnqzz.top/gtotbaybxr.html

[U76] PHP：简单路由
来源：http://hz.yuanzhike.top/gtfjvttjrd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jqgufenzy.top/gtvjhrbgsx.html

[U77] PHP：模板渲染
来源：http://hz.ywan-chungtsiang.top/gtwhgsifsp.html

composer require twig/twig
来源：http://hz.ywan-chungtsiang.top/gtbujowkln.html

[U78] PHP：单元测试
来源：http://hz.xuetiantiany.cn/gtaebhgyis.html

composer require --dev phpunit/phpunit
来源：http://hz.shuidangran.top/gtbgbtburc.html

[U79] PHP：静态分析
来源：http://hz.chenlongwang.top/gtjhnojlpi.html

composer require --dev phpstan/phpstan
来源：http://hz.daxiang520.top/gtqhskspja.html

[U80] PHP：代码规范修复
来源：http://hz.gotoacloud.top/gtrshrkgoc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hongshengwenyu.top/gtwiowacpq.html

[U81] JS：初始化项目
来源：http://hz.nanxinkj.top/gtwbudxdfu.html

npm init -y;  npm i express
来源：http://hz.zhaomingkeji.xyz/gtkbohbpiv.html

[U82] JS：package.json 脚本
来源：http://hz.ivvv.top/gtytkctngj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.andypj.xyz/gttihoiyop.html

[U83] JS：ES Module 导入导出
来源：http://hz.havefunace.top/gtmtrpvygz.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yueranfly.top/gttepfhaem.html

[U84] JS：CommonJS 写法
来源：http://hz.xingfuxueyuan.xyz/gtykruewly.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.gzhubu.top/gtbdckgoue.html

[U85] JS：可选链
来源：http://hz.vqdsnc.cn/gtlizxjlzh.html

a?.b?.c
来源：http://hz.chenjidiqi.icu/gtslswqxlu.html

[U86] JS：空值合并
来源：http://hz.cashguo.top/gtdzckzgvf.html

a ?? b
来源：http://hz.ywan-chungtsiang.top/gtkvuwzvlp.html

[U87] JS：解构默认值
来源：http://hz.jiagoushi.top/gtimthxjcc.html

const { a = 1, b = 2 } = obj;
来源：http://hz.pengpengdd.cyou/gtdyctkinx.html

[U88] JS：对象展开合并
来源：http://hz.chenzaomai.com/gtigreeert.html

{ ...a, ...b }
来源：http://hz.xingfuxueyuan.xyz/gtgpaenjqe.html

[U89] JS：数组去重
来源：http://hz.hongshengwenyu.top/gttgayghim.html

[...new Set(arr)]
来源：http://hz.zhijiandao.cn/gtjfgzbevd.html

[U90] JS：数字数组排序
来源：http://hz.yvedp.cn/gtatycieij.html

[...arr].sort((a, b) => a - b)
来源：http://hz.mhx1999.top/gtrfymkkhb.html

[U91] JS：对象键值遍历
来源：http://hz.jinqigufen.top/gtkzeglltt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yj20258888.top/gthsvlvygw.html

[U92] JS：深拷贝
来源：http://hz.pengpengdd.cyou/gtxqwpiwqa.html

structuredClone(obj)
来源：http://hz.ydzc1.top/gtqqpoeyct.html

[U93] JS：模板字符串
来源：http://hz.ppjwa.cn/gtfbylyali.html

`共 ${n} 条`
来源：http://hz.hammf.cn/gtbfdfgpwc.html

[U94] JS：箭头函数
来源：http://hz.meibo888.top/gtafhnfnsn.html

const double = x => x * 2;
来源：http://hz.hnqzz.top/gtfjgzqbzo.html

[U95] JS：Promise 包装
来源：http://hz.yangfankeji.com/gtftcsgsci.html

new Promise((resolve, reject) => {})
来源：http://hz.sxryk.cn/gtvaoomazp.html

[U96] JS：async/await 与异常
来源：http://hz.guowangkeji.top/gthrksfrff.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xylfe.cn/gtfcpunags.html

[U97] JS：并发请求
来源：http://hz.gotoacloud.top/gtlgsgdmwz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hnxiangtu.top/gtizjjymhq.html

[U98] JS：fetch 带 JSON
来源：http://hz.tanke756.top/gtmhwhnrnl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.shangyingyoupin.top/gthlwozlzl.html

[U99] JS：事件监听
来源：http://hz.yvedp.cn/gtgldhtips.html

el.addEventListener("click", e => {})
来源：http://hz.smart0.xyz/gtkjhlwetv.html

[U100] JS：DOM 查询
来源：http://hz.ydjk.org.cn/gtwwscxavs.html

document.querySelector(".item")
来源：http://hz.ehwqpu.com/gtzlvpqwgy.html

[U101] JS：classList 操作
来源：http://hz.haohaochexian.top/gtkpjbowan.html

el.classList.toggle("active")
来源：http://hz.fengsongda.top/gtyvtsdgqf.html

[U102] JS：本地存储
来源：http://hz.nanxinkj.top/gtctipbxrt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.guowangkeji.top/gtnmlmyihc.html

[U103] JS：定时器
来源：http://hz.chenzaomai.com/gtcozwbcyk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.birdmap.top/gtrabnhbtn.html

[U104] JS：防抖
来源：http://hz.ydzc1.top/gtsalgeqfp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.redwolf501.top/gtlqxubxfm.html

[U105] JS：节流
来源：http://hz.andypj.xyz/gtnzzsocqq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.snrcjt.cn/gtjsurocgm.html

[U106] JS：日期格式化
来源：http://hz.sufxvd.cn/gtuoztlvaf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.aizwys.cn/gtuocnzvdc.html

[U107] JS：数字千分位
来源：http://hz.gzhubu.top/gtucqxuyoz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhijiandao.cn/gtsvdpkkpe.html

[U108] JS：随机整数
来源：http://hz.svipenyu.cn/gtlunetqra.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zhaomingkeji.xyz/gtoltrjfpw.html

[U109] JS：数组分组
来源：http://hz.yj20258.top/gtagrdzprc.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jlsjyb.cn/gtujdygbma.html

[U110] JS：数组分块
来源：http://hz.xingfuxueyuan.xyz/gtplxdvfuk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.9152youxi.cn/gtnnnqqxti.html

[U111] JS：对象转 Map
来源：http://hz.zhengqikj.top/gteraiijtg.html

new Map(Object.entries(obj))
来源：http://hz.sufxvd.cn/gtbdmojoje.html

[U112] JS：字符串补位
来源：http://hz.snrcjt.cn/gtggphyvch.html

"7".padStart(3, "0")
来源：http://hz.fengsongda.top/gtvngqveqe.html

[U113] JS：正则替换全部
来源：http://hz.jianghu66.top/gtthiwpzwt.html

s.replaceAll("a", "b")
来源：http://hz.birdmap.top/gtrrbtxjnl.html

[U114] JS：JSON 深比较
来源：http://hz.gaohongyu789.top/gteafwlksu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgfzy.top/gtdkolmgbu.html

[U115] JS：生成 UUID
来源：http://hz.cucudq.cn/gthhcvidws.html

crypto.randomUUID()
来源：http://hz.fzhhl.top/gtgddlvxxh.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.xuetiantiany.cn/gtdlxvxbwa.html

/** @param {string} name */ function f(name) {}
来源：http://hz.xziqi.cn/gtgwevmryh.html

[U117] JS：单元测试
来源：http://hz.ehwqpu.com/gtqzoggyng.html

npm i -D vitest;  npx vitest
来源：http://hz.hywenlv.cn/gtgznmbmdd.html

[U118] JS：开发服务器
来源：http://hz.pengpengdd.cyou/gtkscmefou.html

npm i -D vite;  npx vite
来源：http://hz.jiagoushi.top/gteoedsiby.html

[U119] JS：生产构建
来源：http://hz.xinyue.icu/gtbhefzjor.html

npx vite build
来源：http://hz.yueranfly.top/gtukjltpok.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zdqjudy.top/gtfecjzfbj.html

import.meta.env.VITE_API_URL
来源：http://hz.zhaomingkeji.xyz/gtbxxplxqw.html

================================================================================
来源：http://hz.mhx1999.top/gtjhoxvvzc.html

统计汇总
来源：http://hz.xinyue.icu/gttwdlzebk.html

================================================================================
来源：http://hz.xziqi.cn/gtszqyccfz.html

按语言统计（条）：
来源：http://hz.andypj.xyz/gtaeirhrej.html

Python ......... 252
来源：http://hz.svipenyu.cn/gtgmlczpky.html

PHP ............ 252
来源：http://hz.wangdashe.top/gtvngirhqn.html

JavaScript ..... 252
来源：http://hz.nwbrower.top/gtddstyrhh.html

TypeScript ..... 212
来源：http://hz.hnqzz.top/gtkrnxfgpz.html

Java ........... 212
来源：http://hz.yvedp.cn/gttimmjdsp.html

Go ............. 212
来源：http://hz.shanyushiyangtech.top/gthxldgvgb.html

Ruby ........... 212
来源：http://hz.ywan-chungtsiang.top/gtkypdwkja.html

C# ............. 212
来源：http://hz.cucudq.cn/gtwojhtjzs.html

C .............. 30
来源：http://hz.andypj.xyz/gtewccskro.html

C++ ............ 30
来源：http://hz.xingfuxueyuan.xyz/gtkrpalmje.html

SQL ............ 90
来源：http://hz.chenjidiqi.icu/gtsvcrxgyj.html

Bash ........... 80
来源：http://hz.wangdashe.top/gteookpmpe.html

Kotlin ......... 15
来源：http://hz.aibaodan.cn/gtbcbmcvpw.html

Swift .......... 15
来源：http://hz.dashuyun.cn/gtyhvslkqr.html

Lua ............ 10
来源：http://hz.cucudq.cn/gtvljvlwia.html

Perl ........... 10
来源：http://hz.shzxlz.cn/gtclsshgdu.html

Scala .......... 10
来源：http://hz.iojbl.cn/gtwwrvzscy.html

------------------------------------
来源：http://hz.gaohongyu789.top/gtpeabibil.html

合计 ........... 2106 条
来源：http://hz.xuetiantiany.cn/gtpvpntfxs.html

按章节统计：
来源：http://hz.chenjidiqi.icu/gtjsklfmwa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.smart0.xyz/gtnyddglep.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.gogol.net.cn/gtpvpzoywj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yuanzhike.top/gtzhmghypq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jinqigufen.top/gtvcujotos.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hysaishi.cn/gtnsldubak.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.ywan-chungtsiang.top/gtykrdnikp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.tianlin.xyz/gttmrmgevn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yj202588.top/gtyqmfsend.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jiagoushi.top/gtobabolek.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.shanyushiyangkeji.top/gtcyqloldq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.svipenyu.cn/gttvdmrorl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.gaohongyu789.top/gtrayajnlx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.daria6918.cn/gtxknolxek.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.chenjidiqi.icu/gtegfctccx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.shanyushiyangkeji.top/gtcncoqbfc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zycfv.cn/gtkfuhyqfy.html

Q SQL 专题                              90
来源：http://hz.52xcode.cn/gtuzonteap.html

R Bash 专题                             80
来源：http://hz.wangdashe.top/gthozvxovr.html

S C / C++ 专题                          60
来源：http://hz.kuanghao11.cn/gtokpuoisq.html

T 其他语言补充                          60
来源：http://hz.chenjidiqi.icu/gtmijaihyp.html

U 高频实用片段                         120
来源：http://hz.redwolf501.top/gtqmddkcnt.html

------------------------------------
来源：http://hz.chenjidiqi.icu/gtiqkfqzob.html

合计                                  2106 条
来源：http://hz.yj202588.top/gtfruyerun.html

--------------------------------------------------------------------------------
来源：http://hz.xziqi.cn/gtkiotpnjj.html

使用提醒
来源：http://hz.jqgfzy.top/gtoxpfchkm.html

--------------------------------------------------------------------------------
来源：http://hz.yvedp.cn/gtptspcwbn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.c1oappe.top/gtpsyszpaq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yj20258888.top/gtuujgpopd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hywenlv.cn/gtpipmevzs.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jqgfzy.top/gtzhqjidjl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yj202588.top/gtyutwfwou.html

—— 文件结束 ——
来源：http://hz.sufxvd.cn/gtndcgzojk.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtnfhpnrgj.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yj202588.top/gtzafknvnc.html

Common Programming Examples Cheat Book
来源：http://hz.xinyue.icu/gtltydvarg.html

================================================================================
来源：http://hz.dashuyun.cn/gtvjthvwpd.html

【收录内容】
来源：http://hz.shzxlz.cn/gtrkmvihaa.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.gzhubu.top/gtkiqjdlps.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.ywan-chungtsiang.top/gteyncmgfo.html

SQL · Bash · C · C++
来源：http://hz.zycfv.cn/gtyeicvoet.html


<!-- 参考信息 -->