代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sxryk.cn/gtyoyzqxvc.html

[T59] Scala：循环
来源：http://hz.jqgfzy.top/gtzqxjrfqa.html

for (i <- 1 to 10) println(i)
来源：http://hz.gotoacloud.top/gtmixjppow.html

[T60] Scala：折叠
来源：http://hz.snrcjt.cn/gtdlszytpd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.wangdashe.top/gtlpymbhrj.html

================================================================================
来源：http://hz.fengsongda.top/gthedudajz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.cdnleiting.top/gtpbcooeul.html

================================================================================
来源：http://hz.vqdsnc.cn/gtcrkmdnkq.html

[U01] Py：创建虚拟环境
来源：http://hz.chenlongwang.top/gtjiapzeud.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jiagoushi.top/gthmurmxbr.html

[U02] Py：导出 / 安装依赖
来源：http://hz.gogol.net.cn/gtmllmljuc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yuanzhike.top/gtylmxqqex.html

[U03] Py：加载 .env 配置
来源：http://hz.wangshuangyany.cn/gtojohshkw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.daria6918.cn/gtcemwwltl.html

[U04] Py：变量调试打印
来源：http://hz.daxiang520.top/gtogpsfpar.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yvedp.cn/gttztsjljg.html

[U05] Py：列表去重且保序
来源：http://hz.zycfv.cn/gtliysezpp.html

list(dict.fromkeys(arr))
来源：http://hz.fengsongda.top/gtieconfiw.html

[U06] Py：合并两个字典
来源：http://hz.daria6918.cn/gtdbtjvjug.html

{**a, **b}
来源：http://hz.meibo888.top/gtaeocgfyh.html

[U07] Py：反转字典键值
来源：http://hz.feifeiyinyue.top/gtnagmnlka.html

{v: k for k, v in d.items()}
来源：http://hz.cqqwz.cn/gtthmtkzcx.html

[U08] Py：展平二维列表
来源：http://hz.jqgufenzy.top/gteomrwkzn.html

[y for x in nested for y in x]
来源：http://hz.dashuyun.cn/gtgjgykfyc.html

[U09] Py：字典取最大值的键
来源：http://hz.kuanghao11.cn/gthvemyptg.html

max(d, key=d.get)
来源：http://hz.sxryk.cn/gtplpnjbat.html

[U10] Py：按值排序字典
来源：http://hz.birdmap.top/gtcoloppga.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yueranfly.top/gtefmrrsxd.html

[U11] Py：生成器表达式
来源：http://hz.nanxuanxn.top/gtiawcyiuo.html

(x * 2 for x in arr)
来源：http://hz.pengpengdd.cyou/gtmhfzgzst.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hammf.cn/gtzhrkpobv.html

Counter(arr).most_common(3)
来源：http://hz.shzxlz.cn/gtbaexvjju.html

[U13] Py：固定长度队列
来源：http://hz.shzxlz.cn/gtiqwwfacl.html

deque(maxlen=10)
来源：http://hz.tian-w.cn/gtrmoaswtc.html

[U14] Py：分组收集到列表
来源：http://hz.vqdsnc.cn/gtknlvjgug.html

defaultdict(list)
来源：http://hz.yj20258.top/gtaxcqtjdq.html

[U15] Py：高精度计时
来源：http://hz.jiagoushi.top/gtnkctjkdn.html

t = time.perf_counter()
来源：http://hz.gzhubu.top/gtepkpnscy.html

[U16] Py：命令行参数解析
来源：http://hz.nanxuanxn.top/gtmdaavxhg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.nwbrower.top/gtghaijqpj.html

[U17] Py：初始化日志
来源：http://hz.ivvv.top/gtkdwkrfev.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ivvv.top/gtmizidsdz.html

[U18] Py：预编译正则
来源：http://hz.gaohongyu789.top/gtcxpfnfxu.html

pat = re.compile(r"\d+")
来源：http://hz.hammf.cn/gtmvpcmpsx.html

[U19] Py：正则替换带回调
来源：http://hz.ydzc1.top/gtptozqmrv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hfpthk.cn/gtccvhmsjg.html

[U20] Py：缓存函数结果
来源：http://hz.shzxlz.cn/gtgwpmiaom.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhengqikj.top/gtgrqaviak.html

[U21] Py：自定义上下文管理器
来源：http://hz.ehwqpu.com/gtzkghixxd.html

@contextlib.contextmanager
来源：http://hz.yvedp.cn/gtxcqwukoo.html

[U22] Py：矩阵转置
来源：http://hz.hongshengwenyu.top/gtpfitntbd.html

list(zip(*m))
来源：http://hz.chenzaomai.com/gteyhhqmpb.html

[U23] Py：分块读取大文件
来源：http://hz.jinghuilouyu.cn/gtjlpjdpyp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jianghu66.top/gtqrfzprfr.html

[U24] Py：路径操作
来源：http://hz.ywan-chungtsiang.top/gtsfzkfsdc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.0kj1m.cn/gtmqgssjkc.html

[U25] Py：CSV 按字典读
来源：http://hz.meibo888.top/gtbghzkach.html

csv.DictReader(f)
来源：http://hz.cheryme.top/gteawuvnhu.html

[U26] Py：并发下载
来源：http://hz.smart0.xyz/gtykynjfvo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.aibaodan.cn/gtfkjmymhe.html

[U27] Py：异步 HTTP
来源：http://hz.cheryme.top/gtxnkvpctx.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yanxiufei.cn/gtoyflbeaq.html

[U28] Py：类型别名
来源：http://hz.chenzaomai.com/gtqecqoozr.html

UserId = int
来源：http://hz.jinghuilouyu.cn/gtnggnzxzk.html

[U29] Py：属性校验
来源：http://hz.vqdsnc.cn/gtkbxlcfat.html

@property 与 @x.setter 配合
来源：http://hz.fengsongda.top/gtpaejwddg.html

[U30] Py：数据类
来源：http://hz.sweek.top/gtvdeaadjm.html

@dataclass(slots=True)
来源：http://hz.jianghu66.top/gtfmsnodyj.html

[U31] Py：单测
来源：http://hz.sysykeji.top/gtyrlhbjbe.html

python -m pytest -q
来源：http://hz.nanxinkj.top/gtxugprcnn.html

[U32] Py：代码格式化
来源：http://hz.bjfxy.top/gtxgqsctmf.html

ruff format . && ruff check --fix .
来源：http://hz.ivvv.top/gtekdliwjx.html

[U33] Py：打包发布
来源：http://hz.redwolf501.top/gtpekilhzf.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hysaishi.cn/gtgrabrlaz.html

[U34] Py：判断编码
来源：http://hz.52xcode.cn/gtuyopleuf.html

chardet.detect(raw)
来源：http://hz.quarkkingdee.top/gtmiolvbtm.html

[U35] Py：发送邮件
来源：http://hz.ivvv.top/gtfmwldnyp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.bjfxy.top/gtuambhaaw.html

[U36] Py：定时任务
来源：http://hz.hammf.cn/gtebkugdzs.html

schedule.every(10).minutes.do(job)
来源：http://hz.chenjidiqi.icu/gtuwurklgo.html

[U37] Py：读写 Excel
来源：http://hz.nwbrower.top/gtmcpvbhty.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yj202588.top/gtbjixxmke.html

[U38] Py：获取脚本所在目录
来源：http://hz.yuanzhike.top/gtbyzsfuqg.html

Path(__file__).resolve().parent
来源：http://hz.ehwqpu.com/gtrhzfjlvq.html

[U39] Py：判断是否在交互环境
来源：http://hz.aibaodan.cn/gtfyzjfrai.html

sys.stdout.isatty()
来源：http://hz.fzhhl.top/gthqgsxdij.html

[U40] Py：打印到标准错误
来源：http://hz.pengpengdd.cyou/gtnknerztx.html

print("err", file=sys.stderr)
来源：http://hz.cucudq.cn/gtixcrkbar.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yj20258.top/gtagqsbrtk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.aizwys.cn/gtkbpdmcvb.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jqgfzy.top/gtdxzsldwh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.smart0.xyz/gtqhkkdcrw.html

[U43] PHP：声明命名空间
来源：http://hz.daxiang520.top/gtvpckjwne.html

namespace App\Http;
来源：http://hz.guannengcc.top/gtdnvnawfv.html

[U44] PHP：开启严格类型
来源：http://hz.hysaishi.cn/gtltaiebgk.html

declare(strict_types=1);
来源：http://hz.ydzc1.top/gtnzmcland.html

[U45] PHP：类型声明与返回类型
来源：http://hz.wangshuangyany.cn/gtcccfcwpm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zycfv.cn/gtjqhxxspn.html

[U46] PHP：可空类型
来源：http://hz.andypj.xyz/gtjjufwtnf.html

?string $name = null
来源：http://hz.ywan-chungtsiang.top/gthpkjqvcf.html

[U47] PHP：联合类型
来源：http://hz.yongpay.top/gtrflzkqwz.html

int|string $id
来源：http://hz.hysaishi.cn/gtsvefonpa.html

[U48] PHP：纯枚举
来源：http://hz.nwbrower.top/gtcnqagrfi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.svipenyu.cn/gtybzrdnyi.html

[U49] PHP：只读属性
来源：http://hz.chenjidiqi.icu/gthbnkqgyn.html

public readonly string $name
来源：http://hz.nanxinkj.top/gttrnfomoa.html

[U50] PHP：构造器属性提升
来源：http://hz.sweek.top/gtfkayjsak.html

public function __construct(private int $id) {}
来源：http://hz.xuanzx.com/gtgmcgcyzq.html

[U51] PHP：数组解构
来源：http://hz.fzhhl.top/gtbbyofexn.html

[$a, $b] = $arr;
来源：http://hz.hnxiangtu.top/gtrufpewfi.html

[U52] PHP：箭头函数
来源：http://hz.pycfn.com/gtjmgmxshn.html

$double = fn($x) => $x * 2;
来源：http://hz.jqgufenzy.top/gtponjvsyf.html

[U53] PHP：空合并运算符
来源：http://hz.aizwys.cn/gtfcpgxojf.html

$v = $a ?? $b ?? "default";
来源：http://hz.quarkkingdee.top/gtzdfsyjjj.html

[U54] PHP：空安全调用
来源：http://hz.zhoulong.xyz/gteoayueil.html

$obj?->method()
来源：http://hz.cucudq.cn/gtglukqvsa.html

[U55] PHP：match 表达式
来源：http://hz.0kj1m.cn/gtalvysuss.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.guannengcc.top/gtzpadrowt.html

[U56] PHP：命名参数
来源：http://hz.hammf.cn/gtbunoeenm.html

f(a: 1, b: 2)
来源：http://hz.aizwys.cn/gtxnpivokm.html

[U57] PHP：字符串插值
来源：http://hz.nanxuanxn.top/gtavzbsnlw.html

"值: {$a}"
来源：http://hz.chenlongwang.top/gteohntcli.html

[U58] PHP：数组三件套
来源：http://hz.nanxuanxn.top/gtbvylxcjv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.xinyue.icu/gtyvajalta.html

[U59] PHP：自定义排序
来源：http://hz.guannengcc.top/gthsdrkcpw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhongyouzk.top/gtlwhoxllc.html

[U60] PHP：JSON 编解码
来源：http://hz.hysaishi.cn/gtpjjszilq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ybcxt.top/gtcmkougfq.html

[U61] PHP：正则
来源：http://hz.yj202588.top/gtxmafrbiu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.feifeiyinyue.top/gtismmbalo.html

[U62] PHP：日期对象
来源：http://hz.pengpengdd.cyou/gtzbwztzoo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zhixingplan.top/gtcmxwevuk.html

[U63] PHP：文件读写
来源：http://hz.fengsongda.top/gttaobilnh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.chenjidiqi.icu/gtudkzcoqw.html

[U64] PHP：目录遍历
来源：http://hz.zhixingplan.top/gtbiawrvmc.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ehwqpu.com/gtcdcnctyw.html

[U65] PHP：会话
来源：http://hz.andypj.xyz/gtgjiyolit.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jinghuilouyu.cn/gttlxbasxm.html

[U66] PHP：设置 Cookie
来源：http://hz.hnxiangtu.top/gtegidonvo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.snrcjt.cn/gtmirgcxiy.html

[U67] PHP：处理文件上传
来源：http://hz.zhengqikj.top/gtynfwurmt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhaomingkeji.xyz/gtveayiqnc.html

[U68] PHP：PDO 连接
来源：http://hz.daxiang520.top/gteceycuzz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zhengqikj.top/gtxlvukffd.html

[U69] PHP：PDO 预处理
来源：http://hz.ywan-chungtsiang.top/gtopntxemb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.cheryme.top/gtcuopzwxf.html

[U70] PHP：PDO 事务
来源：http://hz.shanyushiyangtech.top/gtzuxyhaie.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.fengsongda.top/gtfoaisjpw.html

[U71] PHP：抛出异常
来源：http://hz.shanyushiyangtech.top/gtywzgvvxe.html

throw new RuntimeException("失败", 500);
来源：http://hz.jinyuanbaomall.cn/gtoywcsewm.html

[U72] PHP：写错误日志
来源：http://hz.0kj1m.cn/gtwfevqvde.html

error_log("失败: " . $e->getMessage());
来源：http://hz.52xcode.cn/gtpcgbhtkw.html

[U73] PHP：读取 ini 配置
来源：http://hz.aizwys.cn/gtshuggfhh.html

parse_ini_file("config.ini", true)
来源：http://hz.nanxuanxn.top/gtypvslbig.html

[U74] PHP：读取环境变量
来源：http://hz.chenlongwang.top/gtfippfrzh.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zhixingplan.top/gtzfqkzlek.html

[U75] PHP：依赖注入
来源：http://hz.yuxming.cn/gtrcfojabg.html

composer require psr/container
来源：http://hz.fzhhl.top/gtphwayhkv.html

[U76] PHP：简单路由
来源：http://hz.zycfv.cn/gtmbgiidpp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yvedp.cn/gtopcrqcxr.html

[U77] PHP：模板渲染
来源：http://hz.jyoumei.cn/gtbmebsgvu.html

composer require twig/twig
来源：http://hz.shzxlz.cn/gtjwhzjdpw.html

[U78] PHP：单元测试
来源：http://hz.yj20258.top/gtdkuffeog.html

composer require --dev phpunit/phpunit
来源：http://hz.sufxvd.cn/gtxngjqktx.html

[U79] PHP：静态分析
来源：http://hz.xuetiantiany.cn/gtglkmatfk.html

composer require --dev phpstan/phpstan
来源：http://hz.iojbl.cn/gtipodmgtz.html

[U80] PHP：代码规范修复
来源：http://hz.zhoulong.xyz/gtuneamhoe.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.aibaodan.cn/gtytwmakdc.html

[U81] JS：初始化项目
来源：http://hz.ehwqpu.com/gtqlpyswsw.html

npm init -y;  npm i express
来源：http://hz.gotoacloud.top/gtevkexeld.html

[U82] JS：package.json 脚本
来源：http://hz.yj20258.top/gtzpvbspmp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.gaohongyu789.top/gtjjecezwj.html

[U83] JS：ES Module 导入导出
来源：http://hz.dashuyun.cn/gtlrzdgtdt.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.bjfxy.top/gtyjxprzfc.html

[U84] JS：CommonJS 写法
来源：http://hz.tanke756.top/gtvvimlmid.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yonumen.top/gtfxrihikm.html

[U85] JS：可选链
来源：http://hz.zhoulong.xyz/gtrucqtpjs.html

a?.b?.c
来源：http://hz.kuanghao11.cn/gthkbmisnn.html

[U86] JS：空值合并
来源：http://hz.jyoumei.cn/gtuxqecfhb.html

a ?? b
来源：http://hz.sxryk.cn/gtbqykotws.html

[U87] JS：解构默认值
来源：http://hz.sufxvd.cn/gtpvqlpoax.html

const { a = 1, b = 2 } = obj;
来源：http://hz.sweek.top/gtqpiaqyac.html

[U88] JS：对象展开合并
来源：http://hz.feifeiyinyue.top/gtvxvrlnlj.html

{ ...a, ...b }
来源：http://hz.yvedp.cn/gtonouxmjy.html

[U89] JS：数组去重
来源：http://hz.52xcode.cn/gtciuxwjmw.html

[...new Set(arr)]
来源：http://hz.yangfankeji.com/gtlbvexocs.html

[U90] JS：数字数组排序
来源：http://hz.cucudq.cn/gtwftfwyrx.html

[...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangtech.top/gtbiczduwp.html

[U91] JS：对象键值遍历
来源：http://hz.jyoumei.cn/gtpavpjvgd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.hnxiangtu.top/gtofkfgwss.html

[U92] JS：深拷贝
来源：http://hz.iojbl.cn/gtmwxjbxfn.html

structuredClone(obj)
来源：http://hz.chenlongwang.top/gtkwxopzst.html

[U93] JS：模板字符串
来源：http://hz.yangfankeji.com/gtcmlmjllh.html

`共 ${n} 条`
来源：http://hz.hfpthk.cn/gtqbjeatxu.html

[U94] JS：箭头函数
来源：http://hz.ppjwa.cn/gtnbluzlzw.html

const double = x => x * 2;
来源：http://hz.jlsjyb.cn/gtzgnlmsov.html

[U95] JS：Promise 包装
来源：http://hz.zdqjudy.top/gtyogmzajp.html

new Promise((resolve, reject) => {})
来源：http://hz.zhixingplan.top/gtgvfttkxs.html

[U96] JS：async/await 与异常
来源：http://hz.daxiang520.top/gtvnqhjdrc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.gogol.net.cn/gtewwkzlfm.html

[U97] JS：并发请求
来源：http://hz.wangdashe.top/gtwtkjoxee.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hongshengwenyu.top/gtbednrics.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhiwuduotai.top/gtbefgrkci.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hongshengwenyu.top/gthwvjypox.html

[U99] JS：事件监听
来源：http://hz.ehwqpu.com/gtcskzoqco.html

el.addEventListener("click", e => {})
来源：http://hz.ydzc1.top/gthqgwwisj.html

[U100] JS：DOM 查询
来源：http://hz.daria6918.cn/gtckljddfi.html

document.querySelector(".item")
来源：http://hz.havefunace.top/gtakobepux.html

[U101] JS：classList 操作
来源：http://hz.zhoulong.xyz/gtjalqyhtk.html

el.classList.toggle("active")
来源：http://hz.zhiwuduotai.top/gtsqemjgdg.html

[U102] JS：本地存储
来源：http://hz.guowangkeji.top/gtdrmkdyft.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.meibo888.top/gtrqhaunbo.html

[U103] JS：定时器
来源：http://hz.xylfe.cn/gtznvuwmni.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xuanzx.com/gtsryzknil.html

[U104] JS：防抖
来源：http://hz.gotoacloud.top/gtvhdcgrtm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxuanxn.top/gtaicsajxk.html

[U105] JS：节流
来源：http://hz.jinyuanbaomall.cn/gtynagdxlm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.daxiang520.top/gtiwcodydj.html

[U106] JS：日期格式化
来源：http://hz.jianghu66.top/gtzcpueopf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.xuetiantiany.cn/gtikkcifkf.html

[U107] JS：数字千分位
来源：http://hz.xziqi.cn/gtdmjrnhxg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhengqikj.top/gtoyhrsibp.html

[U108] JS：随机整数
来源：http://hz.ivvv.top/gtdigbrevf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yuanzhike.top/gtlcrosjhi.html

[U109] JS：数组分组
来源：http://hz.nwbrower.top/gtwiaqlqto.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cashguo.top/gtggawuycn.html

[U110] JS：数组分块
来源：http://hz.52xcode.cn/gttfjohhkg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.nanxuanxn.top/gttxsdicks.html

[U111] JS：对象转 Map
来源：http://hz.cucudq.cn/gtvtbeuzdh.html

new Map(Object.entries(obj))
来源：http://hz.zhoulong.xyz/gtomryiifd.html

[U112] JS：字符串补位
来源：http://hz.vqdsnc.cn/gttlzzqdmn.html

"7".padStart(3, "0")
来源：http://hz.hongshengwenyu.top/gtgusikduo.html

[U113] JS：正则替换全部
来源：http://hz.zhiwuduotai.top/gtaxgqvzxg.html

s.replaceAll("a", "b")
来源：http://hz.dianchejie.cn/gtwigsakzr.html

[U114] JS：JSON 深比较
来源：http://hz.cdnleiting.top/gtczzzxjnl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sufxvd.cn/gthawewbcl.html

[U115] JS：生成 UUID
来源：http://hz.zhiwuduotai.top/gtylmwongk.html

crypto.randomUUID()
来源：http://hz.chenjidiqi.icu/gthjjboysz.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.aizwys.cn/gtrygvsogz.html

/** @param {string} name */ function f(name) {}
来源：http://hz.nanxuanxn.top/gtxeuxekbr.html

[U117] JS：单元测试
来源：http://hz.xuetiantiany.cn/gtgqhoohhw.html

npm i -D vitest;  npx vitest
来源：http://hz.yuxming.cn/gtooadbvvb.html

[U118] JS：开发服务器
来源：http://hz.yonumen.top/gtxjswhzgk.html

npm i -D vite;  npx vite
来源：http://hz.kuanghao11.cn/gtvajilifn.html

[U119] JS：生产构建
来源：http://hz.ivvv.top/gtwtxzsujj.html

npx vite build
来源：http://hz.fzhhl.top/gtaukcofsf.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hfpthk.cn/gthqaksawf.html

import.meta.env.VITE_API_URL
来源：http://hz.gzhubu.top/gtkihmsltn.html

================================================================================
来源：http://hz.meibo888.top/gtdwqjdiax.html

统计汇总
来源：http://hz.kuanghao11.cn/gtzurbuzuc.html

================================================================================
来源：http://hz.quarkkingdee.top/gtgewewqtv.html

按语言统计（条）：
来源：http://hz.shanyushiyangtech.top/gtledbpcjk.html

Python ......... 252
来源：http://hz.jiagoushi.top/gtrlvucsfu.html

PHP ............ 252
来源：http://hz.tanke756.top/gtsykenikm.html

JavaScript ..... 252
来源：http://hz.cucudq.cn/gtdniqzirj.html

TypeScript ..... 212
来源：http://hz.yueranfly.top/gtigmjlizl.html

Java ........... 212
来源：http://hz.chenjidiqi.icu/gtshlxwfic.html

Go ............. 212
来源：http://hz.bjfxy.top/gtlsdelahk.html

Ruby ........... 212
来源：http://hz.daria6918.cn/gtouhreiix.html

C# ............. 212
来源：http://hz.snrcjt.cn/gtomtmebpx.html

C .............. 30
来源：http://hz.chenzaomai.com/gthyllucdb.html

C++ ............ 30
来源：http://hz.pycfn.com/gttjaeauhz.html

SQL ............ 90
来源：http://hz.hnxiangtu.top/gtkysvlnbk.html

Bash ........... 80
来源：http://hz.shuidangran.top/gtzrtvtycp.html

Kotlin ......... 15
来源：http://hz.shangyingyoupin.top/gtrrtjrubm.html

Swift .......... 15
来源：http://hz.yj202588.top/gtppfmhtar.html

Lua ............ 10
来源：http://hz.guowangkeji.top/gtkkzqrvvm.html

Perl ........... 10
来源：http://hz.fzhhl.top/gtbrrartsc.html

Scala .......... 10
来源：http://hz.aizwys.cn/gtbqprdmxa.html

------------------------------------
来源：http://hz.yj202588.top/gtbibscpuj.html

合计 ........... 2106 条
来源：http://hz.wangdashe.top/gtkyvxyhxl.html

按章节统计：
来源：http://hz.jinyuanbaomall.cn/gttzeevdlw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xingfuxueyuan.xyz/gtqqrkmcmj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hfpthk.cn/gtsjchxwoi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zdqjudy.top/gtgrwwujul.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.cqqwz.cn/gtlqrdkgrp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.sweek.top/gtxpsdymrg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.hysaishi.cn/gtwbnktvio.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hammf.cn/gtpdyciqmd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.xinyue.icu/gtarrtsunp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yangfankeji.com/gtcafvtdcv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.cashguo.top/gtkgnewimq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.xuanzx.com/gtgnymlslm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.ehwqpu.com/gtybgjwhsr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.snrcjt.cn/gtgmyguums.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.sysykeji.top/gtyvzhairf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhaomingkeji.xyz/gtykvsoyby.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.wangshuangyany.cn/gtgplfzivn.html

Q SQL 专题                              90
来源：http://hz.jqgfzy.top/gthmhmjytq.html

R Bash 专题                             80
来源：http://hz.smart0.xyz/gtnrldghvb.html

S C / C++ 专题                          60
来源：http://hz.yvedp.cn/gtwmblhmip.html

T 其他语言补充                          60
来源：http://hz.andypj.xyz/gtpzclajpv.html

U 高频实用片段                         120
来源：http://hz.jlsjyb.cn/gtntkoqpya.html

------------------------------------
来源：http://hz.xingfuxueyuan.xyz/gtbzxvtios.html

合计                                  2106 条
来源：http://hz.316326.xyz/gthnrqqvdp.html

--------------------------------------------------------------------------------
来源：http://hz.chenjidiqi.icu/gtlqtkisda.html

使用提醒
来源：http://hz.zhongyouzk.top/gtgqwsjbyl.html

--------------------------------------------------------------------------------
来源：http://hz.zdqjudy.top/gtrccvfbgj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.gotoacloud.top/gtowmervml.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.shzxlz.cn/gtbfgrclgn.html


<!-- 参考信息 -->