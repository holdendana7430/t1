代发 wailian999

[U13] Py：固定长度队列
来源：http://hz.iojbl.cn/gtbamubzhg.html

deque(maxlen=10)
来源：http://hz.pengpengdd.cyou/gtxvffcvps.html

[U14] Py：分组收集到列表
来源：http://hz.pycfn.com/gtzvwtmrov.html

defaultdict(list)
来源：http://hz.tianlin.xyz/gtlbcrlrqu.html

[U15] Py：高精度计时
来源：http://hz.xylfe.cn/gtmbnrtqkc.html

t = time.perf_counter()
来源：http://hz.shanyushiyangtech.top/gtzawxsevb.html

[U16] Py：命令行参数解析
来源：http://hz.zdqjudy.top/gtgyetftzh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.daria6918.cn/gtrwgdosdf.html

[U17] Py：初始化日志
来源：http://hz.yonumen.top/gtaycewzsy.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yueranfly.top/gtwotgnkgl.html

[U18] Py：预编译正则
来源：http://hz.meibo888.top/gtueyskrad.html

pat = re.compile(r"\d+")
来源：http://hz.sweek.top/gtqevguaah.html

[U19] Py：正则替换带回调
来源：http://hz.tanke756.top/gtwhtjfofs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.kuanghao11.cn/gtwrnfeygp.html

[U20] Py：缓存函数结果
来源：http://hz.mhx1999.top/gttxuqsqtz.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shanyushiyangkeji.top/gtaxzqtpop.html

[U21] Py：自定义上下文管理器
来源：http://hz.aibaodan.cn/gtdoecmfda.html

@contextlib.contextmanager
来源：http://hz.jianghu66.top/gtlegyqcfn.html

[U22] Py：矩阵转置
来源：http://hz.sweek.top/gtdvjbztfi.html

list(zip(*m))
来源：http://hz.yanxiufei.cn/gtwudxbgww.html

[U23] Py：分块读取大文件
来源：http://hz.jyoumei.cn/gtbyxxhxdv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.daxiang520.top/gtvnmxvocr.html

[U24] Py：路径操作
来源：http://hz.shanyushiyangtech.top/gtapjhstvp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.snrcjt.cn/gtiinngklb.html

[U25] Py：CSV 按字典读
来源：http://hz.chenlongwang.top/gtmiindozo.html

csv.DictReader(f)
来源：http://hz.ybcxt.top/gtnsrkkzky.html

[U26] Py：并发下载
来源：http://hz.quarkkingdee.top/gttfbypopa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.meibo888.top/gtmanbghbp.html

[U27] Py：异步 HTTP
来源：http://hz.xuetiantiany.cn/gtecpgyifx.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.havefunace.top/gtlwymslbc.html

[U28] Py：类型别名
来源：http://hz.yvedp.cn/gtwnhurjyv.html

UserId = int
来源：http://hz.yj20258.top/gtplbjpckg.html

[U29] Py：属性校验
来源：http://hz.zhengqikj.top/gtyflzgjwk.html

@property 与 @x.setter 配合
来源：http://hz.birdmap.top/gtwknapmdp.html

[U30] Py：数据类
来源：http://hz.cqqwz.cn/gtsaepzcoi.html

@dataclass(slots=True)
来源：http://hz.havefunace.top/gtqisuwerd.html

[U31] Py：单测
来源：http://hz.zhiwuduotai.top/gtsmjvfpgl.html

python -m pytest -q
来源：http://hz.ppjwa.cn/gthrjvuovh.html

[U32] Py：代码格式化
来源：http://hz.nanxinkj.top/gtjmbgtugq.html

ruff format . && ruff check --fix .
来源：http://hz.aibaodan.cn/gtprkpkmpa.html

[U33] Py：打包发布
来源：http://hz.hongshengwenyu.top/gtzzntdsrc.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yj20258888.top/gtxzlzzjsw.html

[U34] Py：判断编码
来源：http://hz.nanxuanxn.top/gtaxrcmfwx.html

chardet.detect(raw)
来源：http://hz.cdnleiting.top/gtakjraylc.html

[U35] Py：发送邮件
来源：http://hz.zhaomingkeji.xyz/gtdeilketb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.sweek.top/gthejqlmdi.html

[U36] Py：定时任务
来源：http://hz.chenzaomai.com/gtnkivjnrl.html

schedule.every(10).minutes.do(job)
来源：http://hz.dianchejie.cn/gtdawiukmf.html

[U37] Py：读写 Excel
来源：http://hz.xingfuxueyuan.xyz/gttpavemdo.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhiwuduotai.top/gtkxttxzjh.html

[U38] Py：获取脚本所在目录
来源：http://hz.kuanghao11.cn/gttgkcziat.html

Path(__file__).resolve().parent
来源：http://hz.zycfv.cn/gtkbvsjinq.html

[U39] Py：判断是否在交互环境
来源：http://hz.wangdashe.top/gtmhkittys.html

sys.stdout.isatty()
来源：http://hz.jinyuanbaomall.cn/gtmmbiptos.html

[U40] Py：打印到标准错误
来源：http://hz.jianghu66.top/gtrnxdovtv.html

print("err", file=sys.stderr)
来源：http://hz.hammf.cn/gtezncrhlz.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.hfpthk.cn/gtuhomkbxj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.sysykeji.top/gtqafifvyy.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yongpay.top/gtumnhujuy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.aizwys.cn/gtvwdnzjcu.html

[U43] PHP：声明命名空间
来源：http://hz.guowangkeji.top/gtawjlxflq.html

namespace App\Http;
来源：http://hz.yongpay.top/gtogqrvgjp.html

[U44] PHP：开启严格类型
来源：http://hz.nwbrower.top/gtmghtxevd.html

declare(strict_types=1);
来源：http://hz.yvedp.cn/gtajjzoizn.html

[U45] PHP：类型声明与返回类型
来源：http://hz.316326.xyz/gtfvdbhzon.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cdnleiting.top/gtfbmbqbvn.html

[U46] PHP：可空类型
来源：http://hz.pycfn.com/gtmlsmtrfg.html

?string $name = null
来源：http://hz.jinqigufen.top/gtwwckbijc.html

[U47] PHP：联合类型
来源：http://hz.ydzc1.top/gtkzrtccvs.html

int|string $id
来源：http://hz.hnxiangtu.top/gtdfkgpyof.html

[U48] PHP：纯枚举
来源：http://hz.gotoacloud.top/gtcgmhpjke.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.cheryme.top/gtguavcqbb.html

[U49] PHP：只读属性
来源：http://hz.52xcode.cn/gtpqmgengs.html

public readonly string $name
来源：http://hz.iojbl.cn/gtiwhmboka.html

[U50] PHP：构造器属性提升
来源：http://hz.shangyingyoupin.top/gtmydfmeoy.html

public function __construct(private int $id) {}
来源：http://hz.ywan-chungtsiang.top/gtrsqzaocu.html

[U51] PHP：数组解构
来源：http://hz.tanke756.top/gtujimaojh.html

[$a, $b] = $arr;
来源：http://hz.tian-w.cn/gtlqczyorg.html

[U52] PHP：箭头函数
来源：http://hz.zhaomingkeji.xyz/gtoqxuxnjk.html

$double = fn($x) => $x * 2;
来源：http://hz.xziqi.cn/gtqsjudymt.html

[U53] PHP：空合并运算符
来源：http://hz.redwolf501.top/gthwdwrmqo.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhiwuduotai.top/gtjettvlzj.html

[U54] PHP：空安全调用
来源：http://hz.redwolf501.top/gthpkrifcj.html

$obj?->method()
来源：http://hz.yuanzhike.top/gtomkhnles.html

[U55] PHP：match 表达式
来源：http://hz.yj20258.top/gtyqhezvvc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.chenlongwang.top/gtobkdsavz.html

[U56] PHP：命名参数
来源：http://hz.gogol.net.cn/gtisdfankv.html

f(a: 1, b: 2)
来源：http://hz.yuxming.cn/gtwbwwwuic.html

[U57] PHP：字符串插值
来源：http://hz.xylfe.cn/gtkiqdxsjz.html

"值: {$a}"
来源：http://hz.yj202588.top/gtcrwozhrt.html

[U58] PHP：数组三件套
来源：http://hz.hammf.cn/gtftlxpmux.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yueranfly.top/gtzvgilmko.html

[U59] PHP：自定义排序
来源：http://hz.gotoacloud.top/gtxtgqxsul.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ywan-chungtsiang.top/gtgowchucq.html

[U60] PHP：JSON 编解码
来源：http://hz.cashguo.top/gtvdvjeuke.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.gaohongyu789.top/gtxmftcnrh.html

[U61] PHP：正则
来源：http://hz.tianlin.xyz/gtzhhkbedj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.ybcxt.top/gtiwfefwcq.html

[U62] PHP：日期对象
来源：http://hz.yuxming.cn/gtaxbiruwd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.dashuyun.cn/gthaaqnayp.html

[U63] PHP：文件读写
来源：http://hz.gogol.net.cn/gtnnzpgeai.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.pycfn.com/gtoiujktmu.html

[U64] PHP：目录遍历
来源：http://hz.wangdashe.top/gtciskhctf.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.sxryk.cn/gtdpejiskn.html

[U65] PHP：会话
来源：http://hz.yanxiufei.cn/gtaffcprob.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.shanyushiyangtech.top/gthibichiz.html

[U66] PHP：设置 Cookie
来源：http://hz.nanxinkj.top/gtdkgeffau.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhiwuduotai.top/gtreauwvcy.html

[U67] PHP：处理文件上传
来源：http://hz.jinqigfzy.top/gtuufjybuv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhixingplan.top/gthbtphqqw.html

[U68] PHP：PDO 连接
来源：http://hz.gogol.net.cn/gtyuiokdrd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zdqjudy.top/gtdbzufsfv.html

[U69] PHP：PDO 预处理
来源：http://hz.chenzaomai.com/gttbgpjdzf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zhiwuduotai.top/gtnbkrmbda.html

[U70] PHP：PDO 事务
来源：http://hz.yangfankeji.com/gtschedirs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.vqdsnc.cn/gtqhcpowoy.html

[U71] PHP：抛出异常
来源：http://hz.xziqi.cn/gtntrqhrzk.html

throw new RuntimeException("失败", 500);
来源：http://hz.smart0.xyz/gtlqoxtaqh.html

[U72] PHP：写错误日志
来源：http://hz.nanxinkj.top/gtzvsotesl.html

error_log("失败: " . $e->getMessage());
来源：http://hz.gzhubu.top/gtzdihfavg.html

[U73] PHP：读取 ini 配置
来源：http://hz.hnqzz.top/gtqsbfursx.html

parse_ini_file("config.ini", true)
来源：http://hz.jiagoushi.top/gttcjgazef.html

[U74] PHP：读取环境变量
来源：http://hz.ydjk.org.cn/gtfupjkeqo.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jianghu66.top/gtkvquvwuw.html

[U75] PHP：依赖注入
来源：http://hz.yj202588.top/gtwkuplrem.html

composer require psr/container
来源：http://hz.xylfe.cn/gtaqkmmtvs.html

[U76] PHP：简单路由
来源：http://hz.yanxiufei.cn/gtpbzqmgxg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.nanxinkj.top/gtxllzlguv.html

[U77] PHP：模板渲染
来源：http://hz.tian-w.cn/gtdiyaoabc.html

composer require twig/twig
来源：http://hz.cashguo.top/gtnreheahm.html

[U78] PHP：单元测试
来源：http://hz.jinyuanbaomall.cn/gtvfirjacl.html

composer require --dev phpunit/phpunit
来源：http://hz.cqqwz.cn/gtzbbcddaw.html

[U79] PHP：静态分析
来源：http://hz.feifeiyinyue.top/gtrumdinyi.html

composer require --dev phpstan/phpstan
来源：http://hz.sysykeji.top/gtojkdyokb.html

[U80] PHP：代码规范修复
来源：http://hz.zhongyouzk.top/gtmpahimij.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.ppjwa.cn/gtnhvekxiq.html

[U81] JS：初始化项目
来源：http://hz.ydjk.org.cn/gttjopahsj.html

npm init -y;  npm i express
来源：http://hz.9152youxi.cn/gtgtoyqvzz.html

[U82] JS：package.json 脚本
来源：http://hz.jinyuanbaomall.cn/gtjcuhftnp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zhengqikj.top/gtgppemttf.html

[U83] JS：ES Module 导入导出
来源：http://hz.ybcxt.top/gtfdqjurgy.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.ywan-chungtsiang.top/gtiuoeanhb.html

[U84] JS：CommonJS 写法
来源：http://hz.xingfuxueyuan.xyz/gtigvwsmei.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.ehwqpu.com/gtvqlehtsc.html

[U85] JS：可选链
来源：http://hz.gzhubu.top/gtfyrkjfls.html

a?.b?.c
来源：http://hz.tian-w.cn/gtpzomtkuf.html

[U86] JS：空值合并
来源：http://hz.iojbl.cn/gtaqhyrymw.html

a ?? b
来源：http://hz.wangdashe.top/gtqnkmxcov.html

[U87] JS：解构默认值
来源：http://hz.hnqzz.top/gtvxfnuzip.html

const { a = 1, b = 2 } = obj;
来源：http://hz.chenjidiqi.icu/gtpeozlhjf.html

[U88] JS：对象展开合并
来源：http://hz.zdqjudy.top/gtoygzrxaf.html

{ ...a, ...b }
来源：http://hz.gzhubu.top/gtpmpkqgbz.html

[U89] JS：数组去重
来源：http://hz.jinqigufen.top/gtefxgdtwe.html

[...new Set(arr)]
来源：http://hz.yueranfly.top/gtuhrtypqk.html

[U90] JS：数字数组排序
来源：http://hz.hongshengwenyu.top/gthohfnvyk.html

[...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtoqhkuvqw.html

[U91] JS：对象键值遍历
来源：http://hz.jinghuilouyu.cn/gttrlnrkwb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.tian-w.cn/gtjxbgxdzs.html

[U92] JS：深拷贝
来源：http://hz.0kj1m.cn/gtzmgpipwb.html

structuredClone(obj)
来源：http://hz.chenjidiqi.icu/gtmhxdisuu.html

[U93] JS：模板字符串
来源：http://hz.feifeiyinyue.top/gtykiiszda.html

`共 ${n} 条`
来源：http://hz.jyoumei.cn/gtvqpmbwur.html

[U94] JS：箭头函数
来源：http://hz.sufxvd.cn/gtlngmfmht.html

const double = x => x * 2;
来源：http://hz.yj20258888.top/gtaqvbpzvk.html

[U95] JS：Promise 包装
来源：http://hz.nwbrower.top/gttviscwko.html

new Promise((resolve, reject) => {})
来源：http://hz.yangfankeji.com/gtbczxikvy.html

[U96] JS：async/await 与异常
来源：http://hz.chenjidiqi.icu/gtchxcbyra.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jiagoushi.top/gtqibdtfxo.html

[U97] JS：并发请求
来源：http://hz.yj20258.top/gtgtjglajt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jianghu66.top/gtvcffovgp.html

[U98] JS：fetch 带 JSON
来源：http://hz.yuxming.cn/gtdnljwxyp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.wangshuangyany.cn/gtgjvggivj.html

[U99] JS：事件监听
来源：http://hz.redwolf501.top/gtgqogqpzd.html

el.addEventListener("click", e => {})
来源：http://hz.wangshuangyany.cn/gtxreigqzn.html

[U100] JS：DOM 查询
来源：http://hz.ehwqpu.com/gttssyxdhg.html

document.querySelector(".item")
来源：http://hz.cdnleiting.top/gtgipgqdmb.html

[U101] JS：classList 操作
来源：http://hz.tianlin.xyz/gtxevodohf.html

el.classList.toggle("active")
来源：http://hz.yj202588.top/gtxyhsjcwq.html

[U102] JS：本地存储
来源：http://hz.yongpay.top/gtrgaotkap.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.wangshuangyany.cn/gtkzfyotqa.html

[U103] JS：定时器
来源：http://hz.shanyushiyangtech.top/gtveyaqbgx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.sysykeji.top/gtrybbdyng.html

[U104] JS：防抖
来源：http://hz.yonumen.top/gtdzzytpeu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hywenlv.cn/gtasymtonq.html

[U105] JS：节流
来源：http://hz.cheryme.top/gtffnvpzya.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.shanyushiyangtech.top/gtsbbcrusn.html

[U106] JS：日期格式化
来源：http://hz.yj20258888.top/gtlxymquhi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.andypj.xyz/gtmxyozrvy.html

[U107] JS：数字千分位
来源：http://hz.guannengcc.top/gtfmegthlo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.cashguo.top/gtowcixiao.html

[U108] JS：随机整数
来源：http://hz.vqdsnc.cn/gthpslipaa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jiagoushi.top/gtlyfknwmv.html

[U109] JS：数组分组
来源：http://hz.zhengqikj.top/gtkroaoavn.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yueranfly.top/gtenrurtkc.html

[U110] JS：数组分块
来源：http://hz.shuidangran.top/gtdrhwmnon.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.xinyue.icu/gtqfkatoch.html

[U111] JS：对象转 Map
来源：http://hz.jianghu66.top/gtqkqyqznq.html

new Map(Object.entries(obj))
来源：http://hz.xinyue.icu/gtoxltjkrd.html

[U112] JS：字符串补位
来源：http://hz.iojbl.cn/gtofxeobuj.html

"7".padStart(3, "0")
来源：http://hz.cashguo.top/gtgxrykkjn.html

[U113] JS：正则替换全部
来源：http://hz.yuxming.cn/gtxnewmcqe.html

s.replaceAll("a", "b")
来源：http://hz.shangyingyoupin.top/gttpwlljye.html

[U114] JS：JSON 深比较
来源：http://hz.jqgufenzy.top/gtoywmdfnb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.andypj.xyz/gtjhbqzrpc.html

[U115] JS：生成 UUID
来源：http://hz.nwbrower.top/gtmmydvbhj.html

crypto.randomUUID()
来源：http://hz.tanke756.top/gttmpjxgga.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.tian-w.cn/gtlmzieupm.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yuxming.cn/gtmrhdnrfm.html

[U117] JS：单元测试
来源：http://hz.xinyue.icu/gtkjkopazp.html

npm i -D vitest;  npx vitest
来源：http://hz.zhoulong.xyz/gteqmuniff.html

[U118] JS：开发服务器
来源：http://hz.wangdashe.top/gtvdvqszxg.html

npm i -D vite;  npx vite
来源：http://hz.tianlin.xyz/gtcspopual.html

[U119] JS：生产构建
来源：http://hz.ivvv.top/gtjrvdlvtq.html

npx vite build
来源：http://hz.nanxinkj.top/gtvfutbvsu.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yongpay.top/gtlyszoogz.html

import.meta.env.VITE_API_URL
来源：http://hz.0kj1m.cn/gtaxxityon.html

================================================================================
来源：http://hz.ehwqpu.com/gtfxojeexw.html

统计汇总
来源：http://hz.cashguo.top/gttoiapypa.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtoulvlwhl.html

按语言统计（条）：
来源：http://hz.zhixingplan.top/gtexzzpoen.html

Python ......... 252
来源：http://hz.yanxiufei.cn/gthxnoavyg.html

PHP ............ 252
来源：http://hz.hfpthk.cn/gtzuyhlzmr.html

JavaScript ..... 252
来源：http://hz.tianlin.xyz/gtrqfdzosj.html

TypeScript ..... 212
来源：http://hz.jqgufenzy.top/gtktganjdn.html

Java ........... 212
来源：http://hz.ydjk.org.cn/gtbkujshss.html

Go ............. 212
来源：http://hz.shzxlz.cn/gtstdwxwda.html

Ruby ........... 212
来源：http://hz.hywenlv.cn/gttfghsqxg.html

C# ............. 212
来源：http://hz.ybcxt.top/gtqednplyj.html

C .............. 30
来源：http://hz.nanxuanxn.top/gtonhnncuq.html

C++ ............ 30
来源：http://hz.0kj1m.cn/gtdtrhylrk.html

SQL ............ 90
来源：http://hz.tian-w.cn/gtnndzosya.html

Bash ........... 80
来源：http://hz.jinghuilouyu.cn/gtjenyhdjz.html

Kotlin ......... 15
来源：http://hz.gzhubu.top/gtzozdngos.html

Swift .......... 15
来源：http://hz.nanxuanxn.top/gtfirrnint.html

Lua ............ 10
来源：http://hz.shangyingyoupin.top/gtiteijien.html

Perl ........... 10
来源：http://hz.ehwqpu.com/gttwxtesgn.html

Scala .......... 10
来源：http://hz.dashuyun.cn/gticjmlawa.html

------------------------------------
来源：http://hz.svipenyu.cn/gtxxelwqbn.html

合计 ........... 2106 条
来源：http://hz.yanxiufei.cn/gtovacphpr.html

按章节统计：
来源：http://hz.bjfxy.top/gtuaakjijk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhijiandao.cn/gtcrpffous.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yj202588.top/gtpimcjoir.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.tianlin.xyz/gticrpujsf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.pengpengdd.cyou/gtkoxjriqs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.gogol.net.cn/gtmqhgbtkm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.guowangkeji.top/gtxhfgvaxa.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.fengsongda.top/gtahhfvuzc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.mhx1999.top/gtylcioxej.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.xingfuxueyuan.xyz/gtjwkrnizx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hongshengwenyu.top/gtzhkhycja.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.bjfxy.top/gtqejizhdn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.xylfe.cn/gtoehkmvdf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.hnqzz.top/gttavqmfaq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.chenjidiqi.icu/gtkiezzfbt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.ydjk.org.cn/gtqaprzjyf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yanxiufei.cn/gtevngkaxf.html

Q SQL 专题                              90
来源：http://hz.yanxiufei.cn/gtbvgchopk.html

R Bash 专题                             80
来源：http://hz.daria6918.cn/gtgzstjpyy.html

S C / C++ 专题                          60
来源：http://hz.hnxiangtu.top/gtrzwanygz.html

T 其他语言补充                          60
来源：http://hz.ppjwa.cn/gtdpfyqmvi.html

U 高频实用片段                         120
来源：http://hz.shanyushiyangkeji.top/gtrzwmhfwf.html

------------------------------------
来源：http://hz.hnqzz.top/gtvrrnextl.html

合计                                  2106 条
来源：http://hz.yanxiufei.cn/gtbuvurzoo.html

--------------------------------------------------------------------------------
来源：http://hz.ywan-chungtsiang.top/gtupqttjrr.html

使用提醒
来源：http://hz.yj20258.top/gtqrfojqpp.html

--------------------------------------------------------------------------------
来源：http://hz.cqqwz.cn/gtzffpgtbw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yanxiufei.cn/gtgcoffosv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jlsjyb.cn/gtpqflhldk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.sxryk.cn/gtfdlwpsyu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zycfv.cn/gtubiqqzkb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.dianchejie.cn/gttghonbdn.html

—— 文件结束 ——
来源：http://hz.zhijiandao.cn/gtgfyqzfpb.html

================================================================================
来源：http://hz.ivvv.top/gtrllcpzog.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.guannengcc.top/gtrpmujofm.html

Common Programming Examples Cheat Book
来源：http://hz.bjfxy.top/gtoebmsmdt.html

================================================================================
来源：http://hz.redwolf501.top/gtbxeojuue.html

【收录内容】
来源：http://hz.tanke756.top/gtecwoawmb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jianghu66.top/gtjkdidrer.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.xuetiantiany.cn/gtbgtiynvh.html

SQL · Bash · C · C++
来源：http://hz.havefunace.top/gttuebwdpr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.pycfn.com/gtuoczmsyu.html

【使用说明】
来源：http://hz.dianchejie.cn/gtbzgoehje.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hfpthk.cn/gtmmthzsou.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.xuetiantiany.cn/gtsqkyzkuf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.fzhhl.top/gtzrrkjrxw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.hammf.cn/gtkoewotwc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.svipenyu.cn/gtmhzqaioi.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.ivvv.top/gtfexiqhxr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.xingfuxueyuan.xyz/gtukpluhqv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.nanxinkj.top/gtvbbcolvp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.kuanghao11.cn/gthcoqzmuj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.tanke756.top/gtfhhyyvxx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jqgfzy.top/gtcucjozfj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.tianlin.xyz/gtyygijmzv.html

【文件统计】
来源：http://hz.yanxiufei.cn/gtavidfgjh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.zhoulong.xyz/gtfzvnybvi.html

--------------------------------------------------------------------------------
来源：http://hz.zhijiandao.cn/gtlnsgjhdk.html

目  录
来源：http://hz.xinyue.icu/gtzhdhjfeg.html

--------------------------------------------------------------------------------
来源：http://hz.sysykeji.top/gtkiziygqz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.havefunace.top/gtluqiegpa.html


<!-- 参考信息 -->