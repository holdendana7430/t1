代发 wailian999

find . -name "*.log" -type f
来源：http://hz.nanxuanxn.top/gtdxbssuwr.html

[R44] 按修改时间查找
来源：http://hz.jyoumei.cn/gtphddoawj.html

find . -mtime -7 -type f
来源：http://hz.zycfv.cn/gtocvlgsmc.html

[R45] 批量删除
来源：http://hz.nanxuanxn.top/gtnqmrhcij.html

find . -name "*.tmp" -delete
来源：http://hz.cashguo.top/gtyinjsada.html

[R46] 递归替换文件内容
来源：http://hz.jqgfzy.top/gtwwtqubvp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jlsjyb.cn/gtgzqeinnl.html

[R47] sed 单行替换
来源：http://hz.bjfxy.top/gtgpvtlhjc.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hfpthk.cn/gtgkahopzq.html

[R48] awk 取指定列
来源：http://hz.jinghuilouyu.cn/gtppauuyte.html

awk '{print $1, $3}' a.txt
来源：http://hz.aibaodan.cn/gtnytejxoy.html

[R49] awk 带条件
来源：http://hz.fzhhl.top/gtvntbrcxl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yangfankeji.com/gtivlhsylj.html

[R50] awk 求和
来源：http://hz.jqgufenzy.top/gtyjdnwyyc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhongyouzk.top/gtnxgnzwfq.html

[R51] 排序去重取前几
来源：http://hz.0kj1m.cn/gtoizmbpgw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jlsjyb.cn/gtiwmilrwd.html

[R52] 统计行数
来源：http://hz.smart0.xyz/gtmdnhfmjr.html

wc -l a.txt
来源：http://hz.yj20258.top/gtidgtprum.html

[R53] 查看文件头与实时尾
来源：http://hz.daxiang520.top/gtpoyczjvg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yuxming.cn/gtmazrfoxf.html

[R54] 比较两个文件
来源：http://hz.wangshuangyany.cn/gttfpubgwp.html

diff a.txt b.txt
来源：http://hz.nwbrower.top/gtyztmmrpc.html

[R55] 压缩与解压
来源：http://hz.xingfuxueyuan.xyz/gtyasdsldc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.quarkkingdee.top/gtduhghdhu.html

[R56] 远程拷贝
来源：http://hz.quarkkingdee.top/gtfimkybpr.html

scp file user@host:/path/
来源：http://hz.pycfn.com/gtyvpuxxyy.html

[R57] 远程执行命令
来源：http://hz.shanyushiyangkeji.top/gtcytyenxf.html

ssh user@host 'uptime'
来源：http://hz.shzxlz.cn/gtfyzcfcpd.html

[R58] 下载文件
来源：http://hz.jinghuilouyu.cn/gtxtsaqsbd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zdqjudy.top/gthndjkpkd.html

[R59] 发 POST JSON
来源：http://hz.tanke756.top/gtjjrxwhbp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.nanxuanxn.top/gtlikthsmt.html

[R60] 只看 HTTP 状态码
来源：http://hz.jyoumei.cn/gtxvjptvsp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.wangdashe.top/gtmxiusnay.html

[R61] 磁盘占用
来源：http://hz.ybcxt.top/gtrhkpeidq.html

df -h;  du -sh *
来源：http://hz.shzxlz.cn/gtuvwhlquc.html

[R62] 找最占空间的文件
来源：http://hz.sysykeji.top/gtnmwyaxzl.html

du -ah . | sort -rh | head -10
来源：http://hz.yuxming.cn/gtlwwmfkmo.html

[R63] 内存与进程
来源：http://hz.cucudq.cn/gtblmmltta.html

free -h;  ps aux | grep nginx
来源：http://hz.redwolf501.top/gtleqoetih.html

[R64] 结束进程
来源：http://hz.ehwqpu.com/gtirwwaprl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shuidangran.top/gtbjfykhnj.html

[R65] 查看端口占用
来源：http://hz.cashguo.top/gtdjwicjjm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.chenjidiqi.icu/gtgvzrqgdq.html

[R66] 定时任务
来源：http://hz.sufxvd.cn/gtxsswbpvw.html

crontab -e;  crontab -l
来源：http://hz.tian-w.cn/gtcyylbbcl.html

[R67] 生成随机十六进制串
来源：http://hz.hywenlv.cn/gtdomlosmf.html

openssl rand -hex 16
来源：http://hz.nanxuanxn.top/gtzbvfaswi.html

[R68] 计算文件校验值
来源：http://hz.aizwys.cn/gtmzxkqkdj.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sysykeji.top/gtvhbamkep.html

[R69] 生成随机密码
来源：http://hz.feifeiyinyue.top/gtkocbruin.html

head -c 16 /dev/urandom | base64
来源：http://hz.yueranfly.top/gtismscvzz.html

[R70] 时间戳与互转
来源：http://hz.xuetiantiany.cn/gtyqksggih.html

date +%s;  date -d @1700000000
来源：http://hz.yanxiufei.cn/gtorzxfstx.html

[R71] 日期格式化
来源：http://hz.ehwqpu.com/gtqzzlglgo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gaohongyu789.top/gtzxivmxqx.html

[R72] 等待端口就绪
来源：http://hz.ywan-chungtsiang.top/gtvqmszqky.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.feifeiyinyue.top/gtjdfawkgm.html

[R73] 分割大日志
来源：http://hz.xuanzx.com/gtuztpdlsq.html

split -l 1000 big.log part_
来源：http://hz.yueranfly.top/gtgqwvxxlu.html

[R74] 批量重命名
来源：http://hz.xinyue.icu/gtbvljlxtk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gogol.net.cn/gtssujnhsr.html

[R75] 导出环境变量
来源：http://hz.shanyushiyangtech.top/gtsdzegocz.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sxryk.cn/gtugyjattx.html

[R76] 使用临时文件
来源：http://hz.gotoacloud.top/gtmtalkksv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ybcxt.top/gtduxckhjn.html

[R77] 读取用户输入
来源：http://hz.jlsjyb.cn/gtxuxaupon.html

read -rp "请输入: " ans
来源：http://hz.zhengqikj.top/gtkhnnoliv.html

[R78] 交互式菜单
来源：http://hz.yongpay.top/gtokffyvrc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhaomingkeji.xyz/gthgobwkhn.html

[R79] 解析命令行选项
来源：http://hz.aibaodan.cn/gtkxepexlm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cheryme.top/gtmutcxuuh.html

[R80] 查看脚本执行耗时
来源：http://hz.ppjwa.cn/gtfduofdfa.html

time ./run.sh
来源：http://hz.yuanzhike.top/gttxkxjnfr.html

================================================================================
来源：http://hz.52xcode.cn/gtsgtiszrp.html

S. C / C++ 专题
来源：http://hz.cheryme.top/gtkdhcjdhk.html

================================================================================
来源：http://hz.guowangkeji.top/gttqhjdwnu.html

[S01] C：Hello World
来源：http://hz.daria6918.cn/gtrwkgoiyv.html

#include <stdio.h>
来源：http://hz.ppjwa.cn/gtjozpnqit.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hysaishi.cn/gtrajmrqkn.html

[S02] C：变量与格式化输出
来源：http://hz.hongshengwenyu.top/gtkkfdtkno.html

int a = 10; printf("%d\n", a);
来源：http://hz.tianlin.xyz/gtunrzbbjc.html

[S03] C：读入整数
来源：http://hz.yanxiufei.cn/gtefgkmgup.html

int x; scanf("%d", &x);
来源：http://hz.guowangkeji.top/gtvfocwkai.html

[S04] C：字符串复制
来源：http://hz.yj202588.top/gtvghjsxfm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.quarkkingdee.top/gtcyyroagp.html

[S05] C：字符串长度
来源：http://hz.redwolf501.top/gtejtetoeg.html

strlen(s)
来源：http://hz.jinqigfzy.top/gtxpupgojp.html

[S06] C：字符串比较
来源：http://hz.pycfn.com/gtsmpptsxk.html

strcmp(a, b) == 0
来源：http://hz.shanyushiyangkeji.top/gtxntvxhya.html

[S07] C：数组遍历求和
来源：http://hz.redwolf501.top/gtmaluadro.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ydzc1.top/gtruzjmbnk.html

[S08] C：动态内存分配与释放
来源：http://hz.zhengqikj.top/gtvcbnzvgl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ydjk.org.cn/gtcciutigj.html

[S09] C：结构体定义与初始化
来源：http://hz.nanxinkj.top/gtukvufbjp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xylfe.cn/gtybcmneho.html

[S10] C：指针与解引用
来源：http://hz.jiagoushi.top/gtrgbydjmw.html

int *p = &a;  *p = 5;
来源：http://hz.yuanzhike.top/gtmaokxoac.html

[S11] C：逐行读文件
来源：http://hz.andypj.xyz/gtpexurhex.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sufxvd.cn/gtvizcsrdj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ydjk.org.cn/gtqhlvdgbg.html

fclose(f);
来源：http://hz.shanyushiyangtech.top/gtlwwcodqr.html

[S12] C：写文件
来源：http://hz.nanxinkj.top/gtdromllml.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.guowangkeji.top/gtqwkfzhmi.html

[S13] C：宏定义
来源：http://hz.316326.xyz/gtwvzfiasn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sufxvd.cn/gtdcxedrnq.html

[S14] C：枚举
来源：http://hz.sysykeji.top/gtpnikwhkg.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.sufxvd.cn/gtnssyxsej.html

[S15] C：类型转换
来源：http://hz.yangfankeji.com/gttdohubdk.html

(double) a / b
来源：http://hz.hnxiangtu.top/gtmvtxvriy.html

[S16] C：位操作置位
来源：http://hz.zhijiandao.cn/gtkzrhqtse.html

x |= (1 << 3);
来源：http://hz.xingfuxueyuan.xyz/gthczsrydj.html

[S17] C：安全拼接字符串
来源：http://hz.cqqwz.cn/gtdboiftnz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xuanzx.com/gtefxaqjjg.html

[S18] C：命令行参数
来源：http://hz.zhaomingkeji.xyz/gtuafcprbl.html

int main(int argc, char **argv)
来源：http://hz.havefunace.top/gtmfmrglib.html

[S19] C：快速排序
来源：http://hz.ydzc1.top/gtutbpuipq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yonumen.top/gtsdocchot.html

[S20] C：二分查找
来源：http://hz.ivvv.top/gtoskftrdh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.daria6918.cn/gtdeqztjdn.html

[S21] C：字符类别判断
来源：http://hz.nanxinkj.top/gtuwmmkgjw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cdnleiting.top/gtigtqngbf.html

[S22] C：字符串转数字
来源：http://hz.sxryk.cn/gtownrbbzv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.fengsongda.top/gttpfkgcmr.html

[S23] C：随机数
来源：http://hz.jlsjyb.cn/gtrxyagtfa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.wangshuangyany.cn/gtqhqbpkip.html

[S24] C：获取本地时间
来源：http://hz.chenlongwang.top/gtswenixqj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.aibaodan.cn/gtmnnokdam.html

[S25] C：内存拷贝
来源：http://hz.shuidangran.top/gtfbknxjwc.html

memcpy(dst, src, n);
来源：http://hz.jqgufenzy.top/gteidipqct.html

[S26] C：内存清零
来源：http://hz.hammf.cn/gtxhrnlnoe.html

memset(a, 0, sizeof a);
来源：http://hz.shzxlz.cn/gtsywuzdkx.html

[S27] C：定义常量
来源：http://hz.fzhhl.top/gtfuiyucej.html

const double PI = 3.14159;
来源：http://hz.zdqjudy.top/gtrhxiisob.html

[S28] C：静态变量
来源：http://hz.nanxuanxn.top/gtcsqpynrk.html

static int counter = 0;
来源：http://hz.hammf.cn/gtujkbqmme.html

[S29] C：变参函数
来源：http://hz.gotoacloud.top/gtfpgllwfk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinqigfzy.top/gthgwcqumr.html

[S30] C：头文件保护
来源：http://hz.xylfe.cn/gtqsqytohp.html

#ifndef X_H
来源：http://hz.sufxvd.cn/gtzavflqph.html

#define X_H
来源：http://hz.ppjwa.cn/gtxccitbss.html

#endif
来源：http://hz.smart0.xyz/gtphsqpbme.html

[S31] C++：Hello World
来源：http://hz.gaohongyu789.top/gtzenweoqe.html

#include <iostream>
来源：http://hz.smart0.xyz/gtblolkmrh.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.0kj1m.cn/gtzuhlreza.html

[S32] C++：字符串
来源：http://hz.sysykeji.top/gtszckyjix.html

std::string s = "hi";  s += "!";
来源：http://hz.meibo888.top/gtysvscuii.html

[S33] C++：vector 增删
来源：http://hz.xuetiantiany.cn/gtxfhsaolw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jinqigfzy.top/gtytltoihd.html

[S34] C++：遍历 vector
来源：http://hz.hfpthk.cn/gtlhdpbxaz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinghuilouyu.cn/gtmzcadpde.html

[S35] C++：map
来源：http://hz.tianlin.xyz/gtjaugfsia.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shzxlz.cn/gttldxtwwq.html

[S36] C++：unordered_map
来源：http://hz.zhoulong.xyz/gtzikifvqy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gaohongyu789.top/gtcgzleeox.html

[S37] C++：set
来源：http://hz.sysykeji.top/gtctqjkhbf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ydzc1.top/gtsexeaqhn.html

[S38] C++：排序
来源：http://hz.cashguo.top/gtkbpywphp.html

std::sort(v.begin(), v.end());
来源：http://hz.birdmap.top/gtujnqadyx.html

[S39] C++：自定义比较器排序
来源：http://hz.nanxinkj.top/gtuvqusmxd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.wangdashe.top/gtmmnjifcz.html

[S40] C++：查找元素
来源：http://hz.tanke756.top/gtluinxtkn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hnxiangtu.top/gtebphdisk.html

[S41] C++：类与构造函数
来源：http://hz.sxryk.cn/gtkhidwlms.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jqgufenzy.top/gthlwdaies.html

[S42] C++：继承与虚函数
来源：http://hz.hnqzz.top/gtcbubkmxp.html

class B : public Base { public: void f() override {} };
来源：http://hz.wangdashe.top/gtmnodqads.html

[S43] C++：智能指针
来源：http://hz.chenzaomai.com/gtjsztowsb.html

auto p = std::make_unique<int>(5);
来源：http://hz.meibo888.top/gtpoobjdiq.html

[S44] C++：引用传参
来源：http://hz.xinyue.icu/gtjdvqnqha.html

void inc(int &x) { ++x; }
来源：http://hz.shanyushiyangtech.top/gtfsmwmprn.html

[S45] C++：lambda
来源：http://hz.hywenlv.cn/gtdwhmilpy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinghuilouyu.cn/gtywsidwku.html

[S46] C++：函数模板
来源：http://hz.guannengcc.top/gtfwqcxqmi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.daxiang520.top/gtiqajxqbg.html

[S47] C++：结构化绑定遍历
来源：http://hz.yanxiufei.cn/gtcmaqfurq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gzhubu.top/gtptubadkf.html

[S48] C++：逐行读文件
来源：http://hz.birdmap.top/gtnigxrnua.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.9152youxi.cn/gtiofkakqd.html

while (std::getline(in, line)) { }
来源：http://hz.shanyushiyangtech.top/gtrkrzdeqh.html

[S49] C++：写文件
来源：http://hz.pycfn.com/gtydcpweso.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhaomingkeji.xyz/gtitzvgloh.html

[S50] C++：格式化数字
来源：http://hz.gotoacloud.top/gtblswfzfb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hnxiangtu.top/gtnhzmpepv.html

[S51] C++：显式类型转换
来源：http://hz.svipenyu.cn/gtqbksvfeo.html

static_cast<double>(a) / b
来源：http://hz.iojbl.cn/gtascqhzjr.html

[S52] C++：const 与 noexcept
来源：http://hz.ppjwa.cn/gttxsynayp.html

int size() const noexcept { return n_; }
来源：http://hz.ywan-chungtsiang.top/gtgzmsxrho.html

[S53] C++：移动语义
来源：http://hz.sufxvd.cn/gtywynpodb.html

std::vector<int> w = std::move(v);
来源：http://hz.sysykeji.top/gtjhpjjcfc.html

[S54] C++：异常处理
来源：http://hz.xylfe.cn/gtpxsqirzf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ivvv.top/gtbibtvlfr.html

[S55] C++：结构化绑定
来源：http://hz.yongpay.top/gtglshcluu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jinqigufen.top/gtcirxieok.html

[S56] C++：optional
来源：http://hz.cheryme.top/gtzafvxkpw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ehwqpu.com/gtpulqcnxn.html

[S57] C++：编译期常量
来源：http://hz.fzhhl.top/gtuzahzics.html

constexpr int N = 10;
来源：http://hz.ybcxt.top/gtrspenvik.html

[S58] C++：命名空间
来源：http://hz.wangshuangyany.cn/gtdkhemwnd.html

namespace ns { int f() { return 1; } }
来源：http://hz.shzxlz.cn/gtoxzrfldy.html

[S59] C++：静态断言
来源：http://hz.dianchejie.cn/gtnmxzzkap.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.dianchejie.cn/gtrcdsnvoq.html

[S60] C++：遍历并删除元素
来源：http://hz.dashuyun.cn/gtjvwvixch.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gotoacloud.top/gtecrpzzfz.html

================================================================================
来源：http://hz.mhx1999.top/gtatyhjemh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.haohaochexian.top/gtwaynsder.html

================================================================================
来源：http://hz.xuanzx.com/gtwrsyvjtn.html

[T01] Kotlin：Hello World
来源：http://hz.gzhubu.top/gtfqssuokc.html

println("Hello")
来源：http://hz.iojbl.cn/gtyyamivdg.html

[T02] Kotlin：变量
来源：http://hz.hongshengwenyu.top/gthvmtkdze.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jinqigufen.top/gtbqizdvjl.html

[T03] Kotlin：字符串模板
来源：http://hz.birdmap.top/gtbeeapyfr.html

"值: $b"
来源：http://hz.aibaodan.cn/gtyguwvtbt.html

[T04] Kotlin：空安全
来源：http://hz.fzhhl.top/gtnmedbtfk.html

val n: String? = null;  n?.length
来源：http://hz.ppjwa.cn/gtcujqaepf.html

[T05] Kotlin：when 表达式
来源：http://hz.c1oappe.top/gtjtrsetpo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.0kj1m.cn/gtnkhrarzj.html

[T06] Kotlin：集合映射
来源：http://hz.guowangkeji.top/gtihllmhan.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.dashuyun.cn/gtcppqrbks.html

[T07] Kotlin：集合过滤
来源：http://hz.guannengcc.top/gttondtbnk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cqqwz.cn/gtnqnpquml.html

[T08] Kotlin：数据类
来源：http://hz.zhijiandao.cn/gtrfebfycn.html

data class User(val name: String, val age: Int)
来源：http://hz.zhaomingkeji.xyz/gtxrhjobjd.html

[T09] Kotlin：扩展函数
来源：http://hz.aizwys.cn/gtftuhtcbv.html

fun String.exclaim() = this + "!"
来源：http://hz.zhijiandao.cn/gtnxocosfr.html

[T10] Kotlin：默认参数
来源：http://hz.hywenlv.cn/gtueaaevcx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinqigfzy.top/gtxpamqdvw.html

[T11] Kotlin：协程
来源：http://hz.feifeiyinyue.top/gtvaqvomhw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.svipenyu.cn/gtpitpijxe.html

[T12] Kotlin：解构声明
来源：http://hz.jiagoushi.top/gtdzfrbwuw.html

val (a, b) = Pair(1, 2)
来源：http://hz.havefunace.top/gtcudzptci.html

[T13] Kotlin：只读 Map
来源：http://hz.jlsjyb.cn/gtrkdwbwou.html

val m = mapOf("a" to 1)
来源：http://hz.zhongyouzk.top/gthzrfhxqd.html

[T14] Kotlin：循环
来源：http://hz.jlsjyb.cn/gtfylohger.html

for (i in 1..10) println(i)
来源：http://hz.chenjidiqi.icu/gtvoqecatm.html

[T15] Kotlin：接口
来源：http://hz.cqqwz.cn/gtdcsdliel.html

interface Shape { fun area(): Double }
来源：http://hz.tanke756.top/gterypxsgg.html

[T16] Swift：Hello World
来源：http://hz.cucudq.cn/gtwcafxogc.html

print("Hello")
来源：http://hz.cheryme.top/gtmgwvcnaf.html

[T17] Swift：变量与常量
来源：http://hz.zhongyouzk.top/gteygmixni.html

var a = 1;  let b = 2
来源：http://hz.yueranfly.top/gtpwwtcaxx.html

[T18] Swift：字符串插值
来源：http://hz.zhijiandao.cn/gtcuycgony.html

"值: \(b)"
来源：http://hz.jinqigufen.top/gtqwjzeoym.html

[T19] Swift：可选绑定
来源：http://hz.jlsjyb.cn/gtpaofomon.html

if let n = opt { print(n) }
来源：http://hz.chenzaomai.com/gtbxspnfbn.html

[T20] Swift：数组操作
来源：http://hz.hammf.cn/gtbuozhekd.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hfpthk.cn/gtbeajheaw.html

[T21] Swift：遍历
来源：http://hz.gogol.net.cn/gtfbpulyuz.html

for x in a { print(x) }
来源：http://hz.nwbrower.top/gtdqukkiyw.html

[T22] Swift：字典
来源：http://hz.shangyingyoupin.top/gtsleonxkb.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yonumen.top/gtpejiagif.html

[T23] Swift：函数
来源：http://hz.yanxiufei.cn/gtkjlflqse.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinqigufen.top/gtwlbazvtl.html

[T24] Swift：闭包
来源：http://hz.cqqwz.cn/gtnryftdtx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.gzhubu.top/gtlquyfbuz.html

[T25] Swift：结构体
来源：http://hz.hywenlv.cn/gtalxxzosk.html

struct P { var x: Int }
来源：http://hz.tian-w.cn/gtsjabkvew.html

[T26] Swift：类与重写
来源：http://hz.xinyue.icu/gtvsmumcyy.html

class A: Base { override func f() {} }
来源：http://hz.jqgufenzy.top/gtqambufag.html

[T27] Swift：错误处理
来源：http://hz.shanyushiyangtech.top/gtrrqixgsi.html

do { try f() } catch { print(error) }
来源：http://hz.fzhhl.top/gtrorkygcl.html

[T28] Swift：枚举
来源：http://hz.andypj.xyz/gtbwoqhatw.html

enum Color { case red, green }
来源：http://hz.ehwqpu.com/gtlakgolyp.html

[T29] Swift：guard 提前返回
来源：http://hz.xziqi.cn/gtexvmiodx.html

guard let x = opt else { return }
来源：http://hz.xylfe.cn/gtfuviepkf.html

[T30] Swift：协议
来源：http://hz.wangdashe.top/gtlrihgrht.html

protocol Shape { func area() -> Double }
来源：http://hz.daxiang520.top/gtehepsnsq.html

[T31] Lua：Hello World
来源：http://hz.shanyushiyangkeji.top/gtqefdberm.html

print("Hello")
来源：http://hz.hongshengwenyu.top/gtgfhoypuf.html

[T32] Lua：局部变量
来源：http://hz.zhixingplan.top/gtlizrdlyp.html

local a = 1
来源：http://hz.xingfuxueyuan.xyz/gtjbbjsauf.html

[T33] Lua：表（数组）
来源：http://hz.jlsjyb.cn/gtqrafvduv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.chenjidiqi.icu/gtaslkubgj.html

[T34] Lua：遍历表
来源：http://hz.guowangkeji.top/gtuccoeabj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ehwqpu.com/gtoxpanxlt.html

[T35] Lua：字典表
来源：http://hz.yonumen.top/gtoikavceu.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ehwqpu.com/gtdxygsshi.html

[T36] Lua：函数
来源：http://hz.yongpay.top/gtbkxwosmo.html

function add(a, b) return a + b end
来源：http://hz.yj202588.top/gtusdolxmh.html

[T37] Lua：字符串拼接
来源：http://hz.ydzc1.top/gtwhteqdar.html

"a" .. "b"
来源：http://hz.cashguo.top/gtdlmtakfa.html

[T38] Lua：条件
来源：http://hz.yuxming.cn/gtwrrnkxim.html

if x > 0 then print("正") end
来源：http://hz.redwolf501.top/gtcfunpyqc.html

[T39] Lua：模式匹配
来源：http://hz.shuidangran.top/gtrlrndglu.html

string.find(s, "%d+")
来源：http://hz.xuanzx.com/gtxsbpnwpq.html

[T40] Lua：元表
来源：http://hz.316326.xyz/gtvruskeic.html

setmetatable({}, { __index = base })
来源：http://hz.ybcxt.top/gtryftrotf.html

[T41] Perl：Hello World
来源：http://hz.xuetiantiany.cn/gtcsnrhjjt.html

print "Hello\n";
来源：http://hz.yj20258.top/gttuvwzvlo.html

[T42] Perl：变量类型
来源：http://hz.gogol.net.cn/gtzelwnhoe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.shuidangran.top/gtqfhwalbt.html

[T43] Perl：字符串插值
来源：http://hz.birdmap.top/gtiysarvfh.html

"值: $a"
来源：http://hz.tian-w.cn/gtwjguiihk.html

[T44] Perl：条件
来源：http://hz.ywan-chungtsiang.top/gtmpemtzoa.html

if ($a > 0) { print "正"; }
来源：http://hz.xuanzx.com/gtfgealhlh.html

[T45] Perl：数组遍历
来源：http://hz.yj20258.top/gtvfgjukzm.html

for my $x (@arr) { print $x; }
来源：http://hz.tian-w.cn/gtbvdrtxhy.html

[T46] Perl：哈希操作
来源：http://hz.ybcxt.top/gtkyqrxexf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ppjwa.cn/gtpzbwjtll.html


<!-- 参考信息 -->