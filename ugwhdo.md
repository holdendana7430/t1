代发 wailian999

[U13] Py：固定长度队列
来源：http://hz.yanxiufei.cn/gtkuuwfipq.html

deque(maxlen=10)
来源：http://hz.chenjidiqi.icu/gtodwtahqb.html

[U14] Py：分组收集到列表
来源：http://hz.sxryk.cn/gtlhfjxuin.html

defaultdict(list)
来源：http://hz.dashuyun.cn/gtgmxmlszf.html

[U15] Py：高精度计时
来源：http://hz.zhengqikj.top/gtxwdozhdl.html

t = time.perf_counter()
来源：http://hz.zhengqikj.top/gtjvnusiuj.html

[U16] Py：命令行参数解析
来源：http://hz.ehwqpu.com/gtrkdvpufp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hywenlv.cn/gtxdkvbwmn.html

[U17] Py：初始化日志
来源：http://hz.sweek.top/gtxnxvuvxz.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.aibaodan.cn/gtaviweqlw.html

[U18] Py：预编译正则
来源：http://hz.yanxiufei.cn/gtlxnbpipw.html

pat = re.compile(r"\d+")
来源：http://hz.xylfe.cn/gtwzyqkihl.html

[U19] Py：正则替换带回调
来源：http://hz.yj20258.top/gthojpkgbz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jinyuanbaomall.cn/gtyyvedifl.html

[U20] Py：缓存函数结果
来源：http://hz.dashuyun.cn/gtaeyhhzlz.html

@functools.lru_cache(maxsize=None)
来源：http://hz.wangshuangyany.cn/gtmhvxcxjr.html

[U21] Py：自定义上下文管理器
来源：http://hz.ywan-chungtsiang.top/gttgnsyklq.html

@contextlib.contextmanager
来源：http://hz.cheryme.top/gtxpifqkqm.html

[U22] Py：矩阵转置
来源：http://hz.xziqi.cn/gtamiljgtg.html

list(zip(*m))
来源：http://hz.yueranfly.top/gtjjajjvoc.html

[U23] Py：分块读取大文件
来源：http://hz.ehwqpu.com/gtoqltolln.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.dianchejie.cn/gtuusojkoj.html

[U24] Py：路径操作
来源：http://hz.quarkkingdee.top/gttsuwhime.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jlsjyb.cn/gthawxnfxz.html

[U25] Py：CSV 按字典读
来源：http://hz.hnxiangtu.top/gtbpcvdiny.html

csv.DictReader(f)
来源：http://hz.pengpengdd.cyou/gtvzoiyoge.html

[U26] Py：并发下载
来源：http://hz.wangshuangyany.cn/gtarqkmtiz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jqgufenzy.top/gtjbsndjzs.html

[U27] Py：异步 HTTP
来源：http://hz.cqqwz.cn/gtjugcbshp.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jinqigfzy.top/gtpyeepxrj.html

[U28] Py：类型别名
来源：http://hz.cashguo.top/gtlarnmsph.html

UserId = int
来源：http://hz.yj20258888.top/gtfivssejl.html

[U29] Py：属性校验
来源：http://hz.xziqi.cn/gtaiyulvgf.html

@property 与 @x.setter 配合
来源：http://hz.yonumen.top/gtuvafgfmu.html

[U30] Py：数据类
来源：http://hz.hysaishi.cn/gtduqibyrm.html

@dataclass(slots=True)
来源：http://hz.ehwqpu.com/gtupvxcntr.html

[U31] Py：单测
来源：http://hz.hnxiangtu.top/gtgystzlfh.html

python -m pytest -q
来源：http://hz.ehwqpu.com/gtmmvdyipc.html

[U32] Py：代码格式化
来源：http://hz.birdmap.top/gtvtgsbklz.html

ruff format . && ruff check --fix .
来源：http://hz.aibaodan.cn/gtlsiqocgi.html

[U33] Py：打包发布
来源：http://hz.hywenlv.cn/gthkoyvikf.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.svipenyu.cn/gtiadidkxx.html

[U34] Py：判断编码
来源：http://hz.cheryme.top/gtmehzwglo.html

chardet.detect(raw)
来源：http://hz.316326.xyz/gtkmuaxuiz.html

[U35] Py：发送邮件
来源：http://hz.c1oappe.top/gtchfrroao.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zycfv.cn/gtsyyqfgdh.html

[U36] Py：定时任务
来源：http://hz.daria6918.cn/gtgibgikts.html

schedule.every(10).minutes.do(job)
来源：http://hz.fzhhl.top/gtpqrwlbqo.html

[U37] Py：读写 Excel
来源：http://hz.yj20258.top/gtrbvgqhae.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hysaishi.cn/gtibjxkome.html

[U38] Py：获取脚本所在目录
来源：http://hz.hnxiangtu.top/gtqvmxackf.html

Path(__file__).resolve().parent
来源：http://hz.shuidangran.top/gtvloopjnl.html

[U39] Py：判断是否在交互环境
来源：http://hz.sweek.top/gtusfvrqur.html

sys.stdout.isatty()
来源：http://hz.jlsjyb.cn/gtdwnpswdt.html

[U40] Py：打印到标准错误
来源：http://hz.yuanzhike.top/gthjynkqls.html

print("err", file=sys.stderr)
来源：http://hz.bjfxy.top/gtwjqfzfsh.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.snrcjt.cn/gtpvjdzywd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.haohaochexian.top/gtargsbabm.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zycfv.cn/gtaoyusaxo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.52xcode.cn/gtgaeyipkk.html

[U43] PHP：声明命名空间
来源：http://hz.xinyue.icu/gtgbctgmaf.html

namespace App\Http;
来源：http://hz.jqgfzy.top/gtdlloclpp.html

[U44] PHP：开启严格类型
来源：http://hz.cheryme.top/gtdgrsvolk.html

declare(strict_types=1);
来源：http://hz.tianlin.xyz/gtmjejqaco.html

[U45] PHP：类型声明与返回类型
来源：http://hz.pycfn.com/gtrsrcffsa.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pengpengdd.cyou/gtddphgkbr.html

[U46] PHP：可空类型
来源：http://hz.yvedp.cn/gtqyjsgrfb.html

?string $name = null
来源：http://hz.zhiwuduotai.top/gtxfbnvzur.html

[U47] PHP：联合类型
来源：http://hz.jinqigfzy.top/gtnezuphqe.html

int|string $id
来源：http://hz.zdqjudy.top/gthwyeqpel.html

[U48] PHP：纯枚举
来源：http://hz.hnxiangtu.top/gthpovosjy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ppjwa.cn/gtabeyqtfk.html

[U49] PHP：只读属性
来源：http://hz.xziqi.cn/gtehhwlqfl.html

public readonly string $name
来源：http://hz.dianchejie.cn/gtqmmlceya.html

[U50] PHP：构造器属性提升
来源：http://hz.yuxming.cn/gtzzdcgrvs.html

public function __construct(private int $id) {}
来源：http://hz.havefunace.top/gtxatyijuq.html

[U51] PHP：数组解构
来源：http://hz.fzhhl.top/gtyxaadpxt.html

[$a, $b] = $arr;
来源：http://hz.chenlongwang.top/gtjlcylcdd.html

[U52] PHP：箭头函数
来源：http://hz.meibo888.top/gtlxpkkqps.html

$double = fn($x) => $x * 2;
来源：http://hz.dashuyun.cn/gtbawsvvhu.html

[U53] PHP：空合并运算符
来源：http://hz.mhx1999.top/gtixwnfled.html

$v = $a ?? $b ?? "default";
来源：http://hz.cashguo.top/gtzljftpia.html

[U54] PHP：空安全调用
来源：http://hz.aibaodan.cn/gtgfltifqz.html

$obj?->method()
来源：http://hz.jiagoushi.top/gtitkpovvr.html

[U55] PHP：match 表达式
来源：http://hz.vqdsnc.cn/gtbsmvrbdg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.fzhhl.top/gtzgsjrusm.html

[U56] PHP：命名参数
来源：http://hz.daxiang520.top/gttipxoqeg.html

f(a: 1, b: 2)
来源：http://hz.zhixingplan.top/gtyoabllua.html

[U57] PHP：字符串插值
来源：http://hz.dashuyun.cn/gtaqmsmbex.html

"值: {$a}"
来源：http://hz.tian-w.cn/gtqhxywjgq.html

[U58] PHP：数组三件套
来源：http://hz.xinyue.icu/gtsvaopcsd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.tianlin.xyz/gtvryjcjxr.html

[U59] PHP：自定义排序
来源：http://hz.ivvv.top/gtnvjijhvy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gaohongyu789.top/gtuibrmkud.html

[U60] PHP：JSON 编解码
来源：http://hz.aizwys.cn/gtkdkbccqc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.meibo888.top/gtuplkciwm.html

[U61] PHP：正则
来源：http://hz.cucudq.cn/gtycglpjmm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.iojbl.cn/gtkurzpyei.html

[U62] PHP：日期对象
来源：http://hz.fengsongda.top/gthtfdpoaj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.tian-w.cn/gtqucfmgur.html

[U63] PHP：文件读写
来源：http://hz.hongshengwenyu.top/gtsikiueub.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.hysaishi.cn/gtterwjriq.html

[U64] PHP：目录遍历
来源：http://hz.dashuyun.cn/gtiwgsngfw.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.chenlongwang.top/gtzvzhursi.html

[U65] PHP：会话
来源：http://hz.yuxming.cn/gtahswhxjm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hnxiangtu.top/gtozwbvefn.html

[U66] PHP：设置 Cookie
来源：http://hz.zycfv.cn/gtnaiwbhyb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jyoumei.cn/gtcxnueoqa.html

[U67] PHP：处理文件上传
来源：http://hz.zhijiandao.cn/gtjpuzvlvg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.tianlin.xyz/gtcbriotrw.html

[U68] PHP：PDO 连接
来源：http://hz.jinqigfzy.top/gtcsyjsnth.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.wangdashe.top/gtrzqbflmw.html

[U69] PHP：PDO 预处理
来源：http://hz.haohaochexian.top/gtgaqnkgws.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.cucudq.cn/gtaqsvdzsf.html

[U70] PHP：PDO 事务
来源：http://hz.yuanzhike.top/gthiifmrft.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.gotoacloud.top/gtkymzulvp.html

[U71] PHP：抛出异常
来源：http://hz.daxiang520.top/gtzkctlsxs.html

throw new RuntimeException("失败", 500);
来源：http://hz.pycfn.com/gtfnpcayej.html

[U72] PHP：写错误日志
来源：http://hz.quarkkingdee.top/gtrskjgiod.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yvedp.cn/gtxhoscrye.html

[U73] PHP：读取 ini 配置
来源：http://hz.jinqigfzy.top/gtjsbnalkq.html

parse_ini_file("config.ini", true)
来源：http://hz.vqdsnc.cn/gtgdtsjuaw.html

[U74] PHP：读取环境变量
来源：http://hz.yongpay.top/gtxrtwqhro.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zhoulong.xyz/gtgkhoaqcd.html

[U75] PHP：依赖注入
来源：http://hz.nwbrower.top/gtqiieojoo.html

composer require psr/container
来源：http://hz.zycfv.cn/gtseumzzkw.html

[U76] PHP：简单路由
来源：http://hz.gotoacloud.top/gtgbmdkjtr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.iojbl.cn/gtnzfiwboy.html

[U77] PHP：模板渲染
来源：http://hz.jinyuanbaomall.cn/gturwwmefm.html

composer require twig/twig
来源：http://hz.tanke756.top/gtyxkoutev.html

[U78] PHP：单元测试
来源：http://hz.hnxiangtu.top/gtwvhmgedx.html

composer require --dev phpunit/phpunit
来源：http://hz.redwolf501.top/gtpshrqdln.html

[U79] PHP：静态分析
来源：http://hz.jqgufenzy.top/gtoephlftb.html

composer require --dev phpstan/phpstan
来源：http://hz.zhiwuduotai.top/gtsbtuwqbb.html

[U80] PHP：代码规范修复
来源：http://hz.shuidangran.top/gtrpftlbwo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.wangshuangyany.cn/gtcdagdwfh.html

[U81] JS：初始化项目
来源：http://hz.kuanghao11.cn/gtmezdedyg.html

npm init -y;  npm i express
来源：http://hz.hfpthk.cn/gtvjhsifmn.html

[U82] JS：package.json 脚本
来源：http://hz.fzhhl.top/gtpcmvoxwk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.pengpengdd.cyou/gtkfhbkrsz.html

[U83] JS：ES Module 导入导出
来源：http://hz.shangyingyoupin.top/gtdmdnrlui.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yuanzhike.top/gtpejkfoxq.html

[U84] JS：CommonJS 写法
来源：http://hz.xziqi.cn/gtfqjalubi.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yangfankeji.com/gtixauvonx.html

[U85] JS：可选链
来源：http://hz.xuetiantiany.cn/gtzcbbjaqh.html

a?.b?.c
来源：http://hz.fzhhl.top/gtdkkisroy.html

[U86] JS：空值合并
来源：http://hz.sufxvd.cn/gtqeirpunl.html

a ?? b
来源：http://hz.jinghuilouyu.cn/gtokdorbef.html

[U87] JS：解构默认值
来源：http://hz.hywenlv.cn/gtehrpgvug.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yj202588.top/gtwfwbdgnx.html

[U88] JS：对象展开合并
来源：http://hz.ppjwa.cn/gtepurdqwt.html

{ ...a, ...b }
来源：http://hz.hnqzz.top/gtzapzwuxx.html

[U89] JS：数组去重
来源：http://hz.pycfn.com/gtcaagqrue.html

[...new Set(arr)]
来源：http://hz.cashguo.top/gtsdfpqbai.html

[U90] JS：数字数组排序
来源：http://hz.zhiwuduotai.top/gtahofkxpl.html

[...arr].sort((a, b) => a - b)
来源：http://hz.nanxuanxn.top/gtcszaczkw.html

[U91] JS：对象键值遍历
来源：http://hz.yueranfly.top/gtghxxpjbt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.nwbrower.top/gtdbywnpmz.html

[U92] JS：深拷贝
来源：http://hz.cheryme.top/gtilbicpry.html

structuredClone(obj)
来源：http://hz.nwbrower.top/gtcfimgqne.html

[U93] JS：模板字符串
来源：http://hz.sysykeji.top/gtalrogwnd.html

`共 ${n} 条`
来源：http://hz.iojbl.cn/gtjwpbsghf.html

[U94] JS：箭头函数
来源：http://hz.yanxiufei.cn/gtwerzuyhy.html

const double = x => x * 2;
来源：http://hz.jinghuilouyu.cn/gttgfdhvdg.html

[U95] JS：Promise 包装
来源：http://hz.vqdsnc.cn/gtzghxhewz.html

new Promise((resolve, reject) => {})
来源：http://hz.ppjwa.cn/gtlsogrydc.html

[U96] JS：async/await 与异常
来源：http://hz.hammf.cn/gtmtyrrwku.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ywan-chungtsiang.top/gtnqimxrdv.html

[U97] JS：并发请求
来源：http://hz.zhoulong.xyz/gtlurxbaay.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtjtnyybxn.html

[U98] JS：fetch 带 JSON
来源：http://hz.tanke756.top/gtflnknfix.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.jqgufenzy.top/gtnyfqbowq.html

[U99] JS：事件监听
来源：http://hz.yuxming.cn/gtpdsiuixm.html

el.addEventListener("click", e => {})
来源：http://hz.tianlin.xyz/gtentbozii.html

[U100] JS：DOM 查询
来源：http://hz.hysaishi.cn/gtjxaphgzv.html

document.querySelector(".item")
来源：http://hz.birdmap.top/gtqluwfutv.html

[U101] JS：classList 操作
来源：http://hz.cqqwz.cn/gtuoaanysd.html

el.classList.toggle("active")
来源：http://hz.yueranfly.top/gtcnfvcygi.html

[U102] JS：本地存储
来源：http://hz.birdmap.top/gtqtrukvyr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jyoumei.cn/gttjxiyrtk.html

[U103] JS：定时器
来源：http://hz.xziqi.cn/gtdwlhqqqr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.guowangkeji.top/gtoledyama.html

[U104] JS：防抖
来源：http://hz.ydjk.org.cn/gthdrrkspv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guowangkeji.top/gtwtfcyjxa.html

[U105] JS：节流
来源：http://hz.gogol.net.cn/gtztevjakm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.svipenyu.cn/gtclolgrzt.html

[U106] JS：日期格式化
来源：http://hz.yonumen.top/gtelizruqh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.gogol.net.cn/gthzoydeth.html

[U107] JS：数字千分位
来源：http://hz.c1oappe.top/gtyjahqket.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yonumen.top/gthpuzdivw.html

[U108] JS：随机整数
来源：http://hz.tanke756.top/gtyflxrhku.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.aibaodan.cn/gtriacspog.html

[U109] JS：数组分组
来源：http://hz.c1oappe.top/gtnyfshylf.html

Object.groupBy(arr, x => x.type)
来源：http://hz.zhixingplan.top/gtjauykfqh.html

[U110] JS：数组分块
来源：http://hz.tanke756.top/gthosryrme.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.gotoacloud.top/gtiokbchrj.html

[U111] JS：对象转 Map
来源：http://hz.0kj1m.cn/gtvjtxpmos.html

new Map(Object.entries(obj))
来源：http://hz.kuanghao11.cn/gttnnethaz.html

[U112] JS：字符串补位
来源：http://hz.redwolf501.top/gtncokrzla.html

"7".padStart(3, "0")
来源：http://hz.yanxiufei.cn/gtttiahrxu.html

[U113] JS：正则替换全部
来源：http://hz.birdmap.top/gtwehfkvir.html

s.replaceAll("a", "b")
来源：http://hz.pycfn.com/gtxybcgfkv.html

[U114] JS：JSON 深比较
来源：http://hz.hywenlv.cn/gtgpxyhtrm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gogol.net.cn/gtqajxvnke.html

[U115] JS：生成 UUID
来源：http://hz.redwolf501.top/gtrotophmn.html

crypto.randomUUID()
来源：http://hz.yvedp.cn/gtotqnmetb.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.haohaochexian.top/gtmeykiobv.html

/** @param {string} name */ function f(name) {}
来源：http://hz.sxryk.cn/gtysncekub.html

[U117] JS：单元测试
来源：http://hz.aizwys.cn/gtzrypaarh.html

npm i -D vitest;  npx vitest
来源：http://hz.yonumen.top/gtosmpobwj.html

[U118] JS：开发服务器
来源：http://hz.xinyue.icu/gthrxmpdxm.html

npm i -D vite;  npx vite
来源：http://hz.cheryme.top/gtykgrnvoo.html

[U119] JS：生产构建
来源：http://hz.daria6918.cn/gtrqdwkiji.html

npx vite build
来源：http://hz.yvedp.cn/gttphifsus.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xinyue.icu/gtnenskrhe.html

import.meta.env.VITE_API_URL
来源：http://hz.pycfn.com/gtatfiwxgi.html

================================================================================
来源：http://hz.snrcjt.cn/gtqadtwitd.html

统计汇总
来源：http://hz.yonumen.top/gtgbnayhfa.html

================================================================================
来源：http://hz.xylfe.cn/gtgwwlliaj.html

按语言统计（条）：
来源：http://hz.jinqigfzy.top/gtzuzvcqxo.html

Python ......... 252
来源：http://hz.meibo888.top/gtperzpopf.html

PHP ............ 252
来源：http://hz.cheryme.top/gtkbisxefz.html

JavaScript ..... 252
来源：http://hz.ybcxt.top/gtkyanlrnc.html

TypeScript ..... 212
来源：http://hz.mhx1999.top/gtavffllmc.html

Java ........... 212
来源：http://hz.9152youxi.cn/gteiwfvedw.html

Go ............. 212
来源：http://hz.hongshengwenyu.top/gtizpuxtok.html

Ruby ........... 212
来源：http://hz.guannengcc.top/gtdikobwbz.html

C# ............. 212
来源：http://hz.jianghu66.top/gtmhttfgxb.html

C .............. 30
来源：http://hz.cashguo.top/gtrnuhpxxm.html

C++ ............ 30
来源：http://hz.wangshuangyany.cn/gtlokrqsld.html

SQL ............ 90
来源：http://hz.jianghu66.top/gtbzweudtz.html

Bash ........... 80
来源：http://hz.aibaodan.cn/gteujdjedo.html

Kotlin ......... 15
来源：http://hz.meibo888.top/gttpgaqagy.html

Swift .......... 15
来源：http://hz.birdmap.top/gtzegancto.html

Lua ............ 10
来源：http://hz.cdnleiting.top/gtmyfygjuv.html

Perl ........... 10
来源：http://hz.iojbl.cn/gtzsnciwyy.html

Scala .......... 10
来源：http://hz.smart0.xyz/gthtlwhzin.html

------------------------------------
来源：http://hz.meibo888.top/gtojzflntj.html

合计 ........... 2106 条
来源：http://hz.gaohongyu789.top/gtwgfqhdds.html

按章节统计：
来源：http://hz.fengsongda.top/gtsimxbwoa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.cucudq.cn/gtxfovkgpu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.shangyingyoupin.top/gtunnvgcna.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.hywenlv.cn/gtgfetvdve.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.sysykeji.top/gtymvcusru.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hongshengwenyu.top/gtwfvewcdx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.gzhubu.top/gtpygjpzvt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.andypj.xyz/gtzxrwevie.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.sweek.top/gtqsfufnzw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gtavcpdcqf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zhixingplan.top/gtizbmunyz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.dashuyun.cn/gttrjehrnc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.havefunace.top/gtedkhzzyo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jqgufenzy.top/gtcjduaxjs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.gotoacloud.top/gtfqmttbsc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.ybcxt.top/gtpijbinio.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yuanzhike.top/gtinrqhmpa.html

Q SQL 专题                              90
来源：http://hz.yueranfly.top/gtcfswjyll.html

R Bash 专题                             80
来源：http://hz.yuxming.cn/gtkyzxnsko.html

S C / C++ 专题                          60
来源：http://hz.c1oappe.top/gtkpzurima.html

T 其他语言补充                          60
来源：http://hz.ywan-chungtsiang.top/gtqaeolcsy.html

U 高频实用片段                         120
来源：http://hz.meibo888.top/gtchipylpa.html

------------------------------------
来源：http://hz.shanyushiyangkeji.top/gtclxmiapn.html

合计                                  2106 条
来源：http://hz.sxryk.cn/gtdnzgfyzc.html

--------------------------------------------------------------------------------
来源：http://hz.cucudq.cn/gtmsqizjbg.html

使用提醒
来源：http://hz.yangfankeji.com/gtmjdubken.html

--------------------------------------------------------------------------------
来源：http://hz.zhijiandao.cn/gteombaftu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.snrcjt.cn/gtpttgdstp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.nwbrower.top/gtmehiqbpx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yangfankeji.com/gtlscrkwxf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zhiwuduotai.top/gtionnkmma.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.fzhhl.top/gtsqgnsade.html

—— 文件结束 ——
来源：http://hz.sweek.top/gtclgfscbx.html

================================================================================
来源：http://hz.zhixingplan.top/gtkcdykrzq.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.dashuyun.cn/gtxsumvdsy.html

Common Programming Examples Cheat Book
来源：http://hz.yuanzhike.top/gtgykfogla.html

================================================================================
来源：http://hz.yonumen.top/gtyeerummv.html

【收录内容】
来源：http://hz.yuxming.cn/gtuppaveqi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.nanxinkj.top/gthydktptf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.hysaishi.cn/gtdkahuzwc.html

SQL · Bash · C · C++
来源：http://hz.iojbl.cn/gtwfcovkmn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.xinyue.icu/gtmywymgso.html

【使用说明】
来源：http://hz.havefunace.top/gtvquscwyt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hfpthk.cn/gtqykvzzyz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.9152youxi.cn/gtmrqxpnez.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yanxiufei.cn/gtpgqjxcoa.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.xylfe.cn/gtqlengkyg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.zhijiandao.cn/gtetnnmlaz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.xingfuxueyuan.xyz/gtwddhmrva.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.xylfe.cn/gtpucpejrf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.jqgufenzy.top/gtggtggxpm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.ivvv.top/gtwsobrrsv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.c1oappe.top/gtknrlkvco.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.gzhubu.top/gtrtgavrds.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.wangdashe.top/gtrlijtyvg.html

【文件统计】
来源：http://hz.jianghu66.top/gtidrujwva.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.pycfn.com/gtpzrkjrqz.html

--------------------------------------------------------------------------------
来源：http://hz.zhixingplan.top/gttvjltttw.html

目  录
来源：http://hz.guannengcc.top/gtfjafmwlq.html

--------------------------------------------------------------------------------
来源：http://hz.yonumen.top/gtewvljfwp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.snrcjt.cn/gtfjuuiiaj.html


<!-- 参考信息 -->