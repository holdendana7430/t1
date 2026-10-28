代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sufxvd.cn/gtznotdtjl.html

[T59] Scala：循环
来源：http://hz.fengsongda.top/gtspdmsguk.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhengqikj.top/gtkhjqeaao.html

[T60] Scala：折叠
来源：http://hz.c1oappe.top/gtlodtbhbl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jqgfzy.top/gtpebcgdts.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtbflaaojn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.svipenyu.cn/gtwdqsmptb.html

================================================================================
来源：http://hz.redwolf501.top/gtixqayxpw.html

[U01] Py：创建虚拟环境
来源：http://hz.xylfe.cn/gtcsjsbpvf.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.shzxlz.cn/gtmvkhitir.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yj20258888.top/gtugudqxzh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.wangdashe.top/gtecgfrsmi.html

[U03] Py：加载 .env 配置
来源：http://hz.tanke756.top/gtombjbejs.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.daria6918.cn/gtlnagvafx.html

[U04] Py：变量调试打印
来源：http://hz.shangyingyoupin.top/gtnjvaelbl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hysaishi.cn/gtyhuptuug.html

[U05] Py：列表去重且保序
来源：http://hz.mhx1999.top/gtsrlzxtxj.html

list(dict.fromkeys(arr))
来源：http://hz.jinqigufen.top/gtyousyhxd.html

[U06] Py：合并两个字典
来源：http://hz.jyoumei.cn/gtqwcqrdhc.html

{**a, **b}
来源：http://hz.zhixingplan.top/gtqkbmrate.html

[U07] Py：反转字典键值
来源：http://hz.hfpthk.cn/gtxximqemn.html

{v: k for k, v in d.items()}
来源：http://hz.ppjwa.cn/gtmrcsbtkp.html

[U08] Py：展平二维列表
来源：http://hz.daxiang520.top/gtfpkhlqla.html

[y for x in nested for y in x]
来源：http://hz.guowangkeji.top/gtqtsnxhgy.html

[U09] Py：字典取最大值的键
来源：http://hz.jlsjyb.cn/gtqecfopqa.html

max(d, key=d.get)
来源：http://hz.shzxlz.cn/gtwawugaob.html

[U10] Py：按值排序字典
来源：http://hz.xuanzx.com/gtyubnbptl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.smart0.xyz/gtmihrxqdy.html

[U11] Py：生成器表达式
来源：http://hz.nanxuanxn.top/gthkwsbakc.html

(x * 2 for x in arr)
来源：http://hz.hnqzz.top/gturkoxpdw.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.xuetiantiany.cn/gtraumbrbi.html

Counter(arr).most_common(3)
来源：http://hz.shuidangran.top/gthzxarlwy.html

[U13] Py：固定长度队列
来源：http://hz.zhongyouzk.top/gtqcbzhfsg.html

deque(maxlen=10)
来源：http://hz.gzhubu.top/gtibhcblia.html

[U14] Py：分组收集到列表
来源：http://hz.jinyuanbaomall.cn/gtnlvemmko.html

defaultdict(list)
来源：http://hz.pengpengdd.cyou/gtuxmbvxnd.html

[U15] Py：高精度计时
来源：http://hz.jlsjyb.cn/gtagyqtpgy.html

t = time.perf_counter()
来源：http://hz.sweek.top/gttdmzquvc.html

[U16] Py：命令行参数解析
来源：http://hz.svipenyu.cn/gtetwbhmwb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hammf.cn/gtlpumvycg.html

[U17] Py：初始化日志
来源：http://hz.fzhhl.top/gtraknchgv.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zhijiandao.cn/gtxsjycfeq.html

[U18] Py：预编译正则
来源：http://hz.c1oappe.top/gtugkonufx.html

pat = re.compile(r"\d+")
来源：http://hz.c1oappe.top/gtzirvobri.html

[U19] Py：正则替换带回调
来源：http://hz.cashguo.top/gtgjbnrvky.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.shzxlz.cn/gtkigpzazv.html

[U20] Py：缓存函数结果
来源：http://hz.zhiwuduotai.top/gttozjlpcs.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shanyushiyangtech.top/gtchkgbjtm.html

[U21] Py：自定义上下文管理器
来源：http://hz.chenlongwang.top/gtmucjnduh.html

@contextlib.contextmanager
来源：http://hz.shzxlz.cn/gtqaavpznf.html

[U22] Py：矩阵转置
来源：http://hz.meibo888.top/gtelmkjgea.html

list(zip(*m))
来源：http://hz.dianchejie.cn/gtnhgrqiyp.html

[U23] Py：分块读取大文件
来源：http://hz.ydzc1.top/gtyieqrzkr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yongpay.top/gtmpbllcqp.html

[U24] Py：路径操作
来源：http://hz.gaohongyu789.top/gtrckchrxf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.cheryme.top/gtzxyfnzok.html

[U25] Py：CSV 按字典读
来源：http://hz.smart0.xyz/gtumakxaok.html

csv.DictReader(f)
来源：http://hz.zdqjudy.top/gtspcihpzn.html

[U26] Py：并发下载
来源：http://hz.52xcode.cn/gtoltkmphq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhoulong.xyz/gtqfbketug.html

[U27] Py：异步 HTTP
来源：http://hz.shangyingyoupin.top/gtarohbvqv.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jyoumei.cn/gttnzumvoq.html

[U28] Py：类型别名
来源：http://hz.sufxvd.cn/gtzaktirve.html

UserId = int
来源：http://hz.ehwqpu.com/gtrlyeheky.html

[U29] Py：属性校验
来源：http://hz.jinqigufen.top/gtsmexfyyz.html

@property 与 @x.setter 配合
来源：http://hz.mhx1999.top/gtmrtpvkgl.html

[U30] Py：数据类
来源：http://hz.fengsongda.top/gthyokupog.html

@dataclass(slots=True)
来源：http://hz.hnxiangtu.top/gtwgkackxe.html

[U31] Py：单测
来源：http://hz.xziqi.cn/gttmbttwyr.html

python -m pytest -q
来源：http://hz.yanxiufei.cn/gthasusvmz.html

[U32] Py：代码格式化
来源：http://hz.pycfn.com/gtzncwbaif.html

ruff format . && ruff check --fix .
来源：http://hz.xuetiantiany.cn/gtqlyqemwz.html

[U33] Py：打包发布
来源：http://hz.feifeiyinyue.top/gtrhmgylfm.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yuanzhike.top/gteaxyypip.html

[U34] Py：判断编码
来源：http://hz.guannengcc.top/gtakmtkuqz.html

chardet.detect(raw)
来源：http://hz.tanke756.top/gtldyrdqdh.html

[U35] Py：发送邮件
来源：http://hz.yvedp.cn/gtegdzdfll.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yvedp.cn/gtgpcuqjdq.html

[U36] Py：定时任务
来源：http://hz.xingfuxueyuan.xyz/gtbdekgjgv.html

schedule.every(10).minutes.do(job)
来源：http://hz.hnqzz.top/gthxaaqdla.html

[U37] Py：读写 Excel
来源：http://hz.zhaomingkeji.xyz/gtraicvenn.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.sweek.top/gtqqxwbkqs.html

[U38] Py：获取脚本所在目录
来源：http://hz.hywenlv.cn/gtksbvbgtd.html

Path(__file__).resolve().parent
来源：http://hz.cheryme.top/gtcfzgddpg.html

[U39] Py：判断是否在交互环境
来源：http://hz.xziqi.cn/gtveijgeub.html

sys.stdout.isatty()
来源：http://hz.tianlin.xyz/gtzxhjgakp.html

[U40] Py：打印到标准错误
来源：http://hz.snrcjt.cn/gtivxxfdwq.html

print("err", file=sys.stderr)
来源：http://hz.zhengqikj.top/gtlcjmkhhh.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.mhx1999.top/gtfbtwgdaa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.snrcjt.cn/gttxfdcnfu.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.cdnleiting.top/gthghcawob.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.bjfxy.top/gtakdiijbj.html

[U43] PHP：声明命名空间
来源：http://hz.feifeiyinyue.top/gtrbhfmoig.html

namespace App\Http;
来源：http://hz.hnxiangtu.top/gtjktseijv.html

[U44] PHP：开启严格类型
来源：http://hz.ybcxt.top/gtxdigpgkb.html

declare(strict_types=1);
来源：http://hz.quarkkingdee.top/gtpfzwxfde.html

[U45] PHP：类型声明与返回类型
来源：http://hz.xylfe.cn/gtmixstpdb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jianghu66.top/gtdumemfod.html

[U46] PHP：可空类型
来源：http://hz.jyoumei.cn/gtgctdtgyc.html

?string $name = null
来源：http://hz.0kj1m.cn/gtmofybdrc.html

[U47] PHP：联合类型
来源：http://hz.gzhubu.top/gtsvwafnoy.html

int|string $id
来源：http://hz.shanyushiyangkeji.top/gtecypjrao.html

[U48] PHP：纯枚举
来源：http://hz.0kj1m.cn/gtcmgyjtcv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.tianlin.xyz/gtcegtqpoa.html

[U49] PHP：只读属性
来源：http://hz.wangdashe.top/gtkfxdrrwr.html

public readonly string $name
来源：http://hz.hnxiangtu.top/gtiwgefmsl.html

[U50] PHP：构造器属性提升
来源：http://hz.shangyingyoupin.top/gtipymxsas.html

public function __construct(private int $id) {}
来源：http://hz.smart0.xyz/gtcjlvxhcq.html

[U51] PHP：数组解构
来源：http://hz.jinyuanbaomall.cn/gtiwwberps.html

[$a, $b] = $arr;
来源：http://hz.iojbl.cn/gthizrsywu.html

[U52] PHP：箭头函数
来源：http://hz.yvedp.cn/gtpaelgajm.html

$double = fn($x) => $x * 2;
来源：http://hz.sufxvd.cn/gtbuolbacf.html

[U53] PHP：空合并运算符
来源：http://hz.shzxlz.cn/gtefdardej.html

$v = $a ?? $b ?? "default";
来源：http://hz.yueranfly.top/gtolhorokm.html

[U54] PHP：空安全调用
来源：http://hz.yueranfly.top/gtfldarncx.html

$obj?->method()
来源：http://hz.wangshuangyany.cn/gtgcvtvumw.html

[U55] PHP：match 表达式
来源：http://hz.zhengqikj.top/gtenxybmbf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ydjk.org.cn/gtryilblcw.html

[U56] PHP：命名参数
来源：http://hz.jlsjyb.cn/gtxijxquak.html

f(a: 1, b: 2)
来源：http://hz.snrcjt.cn/gtskvkifxi.html

[U57] PHP：字符串插值
来源：http://hz.chenlongwang.top/gtuaasrgha.html

"值: {$a}"
来源：http://hz.havefunace.top/gtcohdmzme.html

[U58] PHP：数组三件套
来源：http://hz.aibaodan.cn/gtemtqdxie.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yanxiufei.cn/gtgnkcfnmz.html

[U59] PHP：自定义排序
来源：http://hz.chenzaomai.com/gtemfxtzwp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ppjwa.cn/gthpgwtwko.html

[U60] PHP：JSON 编解码
来源：http://hz.nwbrower.top/gtkophlyie.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yanxiufei.cn/gtjpbjenmh.html

[U61] PHP：正则
来源：http://hz.daria6918.cn/gtlgwjtlxe.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.ehwqpu.com/gtzrwmpmyb.html

[U62] PHP：日期对象
来源：http://hz.hnxiangtu.top/gtbdhmjwop.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.fengsongda.top/gtjqielgtj.html

[U63] PHP：文件读写
来源：http://hz.jiagoushi.top/gtsrklopoq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yangfankeji.com/gtttltnwvb.html

[U64] PHP：目录遍历
来源：http://hz.yueranfly.top/gtzhjmvljy.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jinyuanbaomall.cn/gtqksatsdm.html

[U65] PHP：会话
来源：http://hz.pycfn.com/gtsenxwyzv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zhiwuduotai.top/gtqimpiuoy.html

[U66] PHP：设置 Cookie
来源：http://hz.tian-w.cn/gtrfhunykw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jinyuanbaomall.cn/gtnrmhhjgy.html

[U67] PHP：处理文件上传
来源：http://hz.tanke756.top/gtcoxfsruk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.cucudq.cn/gtysxllpxb.html

[U68] PHP：PDO 连接
来源：http://hz.ehwqpu.com/gtkdruljva.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.quarkkingdee.top/gtcuplyegw.html

[U69] PHP：PDO 预处理
来源：http://hz.redwolf501.top/gtmffhxsrp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.snrcjt.cn/gtdcffwskf.html

[U70] PHP：PDO 事务
来源：http://hz.daria6918.cn/gtkzlolzjf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.sufxvd.cn/gtmsfdoacl.html

[U71] PHP：抛出异常
来源：http://hz.daxiang520.top/gtdfrtwofb.html

throw new RuntimeException("失败", 500);
来源：http://hz.jqgfzy.top/gtvteupcmn.html

[U72] PHP：写错误日志
来源：http://hz.dianchejie.cn/gtsuggsimt.html

error_log("失败: " . $e->getMessage());
来源：http://hz.xuanzx.com/gtkboeirld.html

[U73] PHP：读取 ini 配置
来源：http://hz.daria6918.cn/gtjvypqrxq.html

parse_ini_file("config.ini", true)
来源：http://hz.zhoulong.xyz/gtphkegtbv.html

[U74] PHP：读取环境变量
来源：http://hz.ybcxt.top/gtyogiepxu.html

getenv("APP_ENV") ?: "production"
来源：http://hz.aizwys.cn/gtdhqxdgel.html

[U75] PHP：依赖注入
来源：http://hz.xylfe.cn/gtzxkivuwj.html

composer require psr/container
来源：http://hz.kuanghao11.cn/gtyjaefmik.html

[U76] PHP：简单路由
来源：http://hz.shzxlz.cn/gtsdxmlavu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hywenlv.cn/gtmlhwxjed.html

[U77] PHP：模板渲染
来源：http://hz.iojbl.cn/gtiqoekjzu.html

composer require twig/twig
来源：http://hz.yj20258.top/gtkfrslaia.html

[U78] PHP：单元测试
来源：http://hz.yonumen.top/gtxmadvrcj.html

composer require --dev phpunit/phpunit
来源：http://hz.daxiang520.top/gtislvfcdh.html

[U79] PHP：静态分析
来源：http://hz.sufxvd.cn/gtwcboczno.html

composer require --dev phpstan/phpstan
来源：http://hz.yj20258888.top/gthixboikf.html

[U80] PHP：代码规范修复
来源：http://hz.meibo888.top/gtrwsqxiub.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhiwuduotai.top/gtaprcriev.html

[U81] JS：初始化项目
来源：http://hz.havefunace.top/gtvjmcxhyz.html

npm init -y;  npm i express
来源：http://hz.shuidangran.top/gtqntccrlx.html

[U82] JS：package.json 脚本
来源：http://hz.yangfankeji.com/gtjcasbywn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.birdmap.top/gtuvepefdr.html

[U83] JS：ES Module 导入导出
来源：http://hz.jinghuilouyu.cn/gtnqtetxpd.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.hongshengwenyu.top/gtcxjlsymj.html

[U84] JS：CommonJS 写法
来源：http://hz.nanxuanxn.top/gtukqeiawu.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zycfv.cn/gtzhtxnjsp.html

[U85] JS：可选链
来源：http://hz.cqqwz.cn/gtatdjkwon.html

a?.b?.c
来源：http://hz.dianchejie.cn/gtpxkniiug.html

[U86] JS：空值合并
来源：http://hz.xylfe.cn/gtmzewltva.html

a ?? b
来源：http://hz.52xcode.cn/gtpjjfdnjj.html

[U87] JS：解构默认值
来源：http://hz.vqdsnc.cn/gtqnsvjllf.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zycfv.cn/gtecafvjsj.html

[U88] JS：对象展开合并
来源：http://hz.kuanghao11.cn/gtmfxklvru.html

{ ...a, ...b }
来源：http://hz.wangdashe.top/gtxpxqsaud.html

[U89] JS：数组去重
来源：http://hz.ppjwa.cn/gtgqzgrwbo.html

[...new Set(arr)]
来源：http://hz.sufxvd.cn/gtgvuuekvn.html

[U90] JS：数字数组排序
来源：http://hz.kuanghao11.cn/gtmomavsrj.html

[...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtjiuqeoaq.html

[U91] JS：对象键值遍历
来源：http://hz.sweek.top/gttaipqgmi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jyoumei.cn/gtasultzdd.html

[U92] JS：深拷贝
来源：http://hz.cashguo.top/gtilqvxlmr.html

structuredClone(obj)
来源：http://hz.smart0.xyz/gtguyrdcqk.html

[U93] JS：模板字符串
来源：http://hz.pycfn.com/gtwhsebiiq.html

`共 ${n} 条`
来源：http://hz.sysykeji.top/gtqncovskw.html

[U94] JS：箭头函数
来源：http://hz.cashguo.top/gtmkrimgia.html

const double = x => x * 2;
来源：http://hz.bjfxy.top/gtemfawfcn.html

[U95] JS：Promise 包装
来源：http://hz.yonumen.top/gtecfuaady.html

new Promise((resolve, reject) => {})
来源：http://hz.andypj.xyz/gttzjvglij.html

[U96] JS：async/await 与异常
来源：http://hz.shanyushiyangtech.top/gtvkvtgwoa.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtjcmxmgjs.html

[U97] JS：并发请求
来源：http://hz.zhiwuduotai.top/gtwmjgfpkb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.vqdsnc.cn/gtqesjnlpj.html

[U98] JS：fetch 带 JSON
来源：http://hz.sysykeji.top/gthtbpykkg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.xuanzx.com/gtnbygczni.html

[U99] JS：事件监听
来源：http://hz.jqgufenzy.top/gtbyylfnxy.html

el.addEventListener("click", e => {})
来源：http://hz.316326.xyz/gtzivdgpxv.html

[U100] JS：DOM 查询
来源：http://hz.zhijiandao.cn/gtgonqwixs.html

document.querySelector(".item")
来源：http://hz.shangyingyoupin.top/gtkgccnwxm.html

[U101] JS：classList 操作
来源：http://hz.zhongyouzk.top/gtllbskwxu.html

el.classList.toggle("active")
来源：http://hz.vqdsnc.cn/gtmxpmjgho.html

[U102] JS：本地存储
来源：http://hz.yangfankeji.com/gtifnxkptd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.chenjidiqi.icu/gtifvohkcn.html

[U103] JS：定时器
来源：http://hz.hnqzz.top/gtfcmtpqnz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.pengpengdd.cyou/gtwpsyabap.html

[U104] JS：防抖
来源：http://hz.meibo888.top/gtbrdiogty.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gogol.net.cn/gtdojupphp.html

[U105] JS：节流
来源：http://hz.bjfxy.top/gtwqpfvlgb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhixingplan.top/gtbdutfkbe.html

[U106] JS：日期格式化
来源：http://hz.ydzc1.top/gtnvatwlaj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yj20258.top/gtqphmctpu.html

[U107] JS：数字千分位
来源：http://hz.meibo888.top/gtozzhcses.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.gaohongyu789.top/gtnpdgooah.html

[U108] JS：随机整数
来源：http://hz.ivvv.top/gtongmkwcr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hfpthk.cn/gtqeaawizm.html

[U109] JS：数组分组
来源：http://hz.shanyushiyangtech.top/gthgcdwfpk.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cdnleiting.top/gtnevbtmku.html

[U110] JS：数组分块
来源：http://hz.zhoulong.xyz/gtmxvihngz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.xziqi.cn/gtarkeuyka.html

[U111] JS：对象转 Map
来源：http://hz.yongpay.top/gtwrmdmaby.html

new Map(Object.entries(obj))
来源：http://hz.yj20258.top/gtcrguguvn.html

[U112] JS：字符串补位
来源：http://hz.wangdashe.top/gthqfmhsqy.html

"7".padStart(3, "0")
来源：http://hz.svipenyu.cn/gtrwkikqsb.html

[U113] JS：正则替换全部
来源：http://hz.jyoumei.cn/gtggvaapsu.html

s.replaceAll("a", "b")
来源：http://hz.feifeiyinyue.top/gtexizrcis.html

[U114] JS：JSON 深比较
来源：http://hz.yonumen.top/gtempaqxxf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hywenlv.cn/gtwmqvtzdh.html

[U115] JS：生成 UUID
来源：http://hz.daxiang520.top/gtcxggheep.html

crypto.randomUUID()
来源：http://hz.wangshuangyany.cn/gtzkslnwcv.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.52xcode.cn/gtnhsuwhzf.html

/** @param {string} name */ function f(name) {}
来源：http://hz.shzxlz.cn/gtvcjpzbrk.html

[U117] JS：单元测试
来源：http://hz.cheryme.top/gtuwcnwmmq.html

npm i -D vitest;  npx vitest
来源：http://hz.xinyue.icu/gtbegmgpcw.html

[U118] JS：开发服务器
来源：http://hz.sweek.top/gtccvrqxjx.html

npm i -D vite;  npx vite
来源：http://hz.xziqi.cn/gtvnatnojv.html

[U119] JS：生产构建
来源：http://hz.quarkkingdee.top/gtutnhppqx.html

npx vite build
来源：http://hz.hywenlv.cn/gtsqjsiqib.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.snrcjt.cn/gtdtparmwo.html

import.meta.env.VITE_API_URL
来源：http://hz.bjfxy.top/gthuvqjzqz.html

================================================================================
来源：http://hz.yanxiufei.cn/gtjcpoibnb.html

统计汇总
来源：http://hz.zdqjudy.top/gtutybhtnv.html

================================================================================
来源：http://hz.andypj.xyz/gtbmkrdezk.html

按语言统计（条）：
来源：http://hz.jinyuanbaomall.cn/gthjyililh.html

Python ......... 252
来源：http://hz.hnxiangtu.top/gtqiodumvy.html

PHP ............ 252
来源：http://hz.guowangkeji.top/gtxfjwxqzm.html

JavaScript ..... 252
来源：http://hz.birdmap.top/gtxxfwidjb.html

TypeScript ..... 212
来源：http://hz.aibaodan.cn/gteheunsva.html

Java ........... 212
来源：http://hz.yj20258888.top/gtmbnyjszo.html

Go ............. 212
来源：http://hz.sufxvd.cn/gtnkuhgxrx.html

Ruby ........... 212
来源：http://hz.shanyushiyangkeji.top/gtqaarvmzr.html

C# ............. 212
来源：http://hz.yuanzhike.top/gtrjsgoxtv.html

C .............. 30
来源：http://hz.yongpay.top/gtzfiqsniv.html

C++ ............ 30
来源：http://hz.fengsongda.top/gtbbzngjxm.html

SQL ............ 90
来源：http://hz.gotoacloud.top/gtbrebvtwx.html

Bash ........... 80
来源：http://hz.ehwqpu.com/gtiedastcb.html

Kotlin ......... 15
来源：http://hz.shzxlz.cn/gtormntslg.html

Swift .......... 15
来源：http://hz.hysaishi.cn/gthubojgen.html

Lua ............ 10
来源：http://hz.hongshengwenyu.top/gtvsgnhowf.html

Perl ........... 10
来源：http://hz.ywan-chungtsiang.top/gtafujwlpa.html

Scala .......... 10
来源：http://hz.haohaochexian.top/gtuczxhlnh.html

------------------------------------
来源：http://hz.yonumen.top/gtceoemuhc.html

合计 ........... 2106 条
来源：http://hz.gzhubu.top/gtsvhbvqmh.html

按章节统计：
来源：http://hz.snrcjt.cn/gtkdnmvhxg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jinqigufen.top/gtwpdvhoel.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.xingfuxueyuan.xyz/gtnketxfpr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhengqikj.top/gtttkupcvw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.chenjidiqi.icu/gtzgzmfeqi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.wangshuangyany.cn/gtsgtheznx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zdqjudy.top/gthemvpflx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yanxiufei.cn/gtdczqddtc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.jinqigfzy.top/gtnrhqlqxj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yueranfly.top/gtegmpotds.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yuanzhike.top/gtetmxbkdx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.52xcode.cn/gtxrzjtexh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.wangshuangyany.cn/gtazhdvtmj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jinqigfzy.top/gtxjobyvmz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.svipenyu.cn/gteamojwfl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.svipenyu.cn/gtfdyxcfuv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.birdmap.top/gtfxzvfehh.html

Q SQL 专题                              90
来源：http://hz.0kj1m.cn/gtqnzqutss.html

R Bash 专题                             80
来源：http://hz.zhoulong.xyz/gtvqwvwpli.html

S C / C++ 专题                          60
来源：http://hz.xuanzx.com/gtqrbtbqgh.html

T 其他语言补充                          60
来源：http://hz.gogol.net.cn/gtwgvqduzf.html

U 高频实用片段                         120
来源：http://hz.zhaomingkeji.xyz/gtkmyyqwls.html

------------------------------------
来源：http://hz.hysaishi.cn/gtpoylqnwk.html

合计                                  2106 条
来源：http://hz.hammf.cn/gtsfjyblxw.html

--------------------------------------------------------------------------------
来源：http://hz.iojbl.cn/gtvriavwsz.html

使用提醒
来源：http://hz.yangfankeji.com/gttfoecgwt.html

--------------------------------------------------------------------------------
来源：http://hz.birdmap.top/gtdqkyusoc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zycfv.cn/gtjxlzzwsg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yongpay.top/gtobtwewoc.html


<!-- 参考信息 -->