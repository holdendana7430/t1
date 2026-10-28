代发 wailian999

cmd > out.log 2>&1
来源：http://hz.havefunace.top/gthmgdpzzc.html

[R40] 追加写日志
来源：http://hz.jyoumei.cn/gtglsppjqq.html

echo "log" >> out.log
来源：http://hz.meibo888.top/gtauhqityy.html

[R41] 丢弃输出
来源：http://hz.xinyue.icu/gtobgijrhy.html

cmd >/dev/null 2>&1
来源：http://hz.hnxiangtu.top/gtwddjzhkk.html

[R42] 输入重定向
来源：http://hz.svipenyu.cn/gtpjrnrfzq.html

wc -l < a.txt
来源：http://hz.aibaodan.cn/gtyqklpjiw.html

[R43] 按名字查找文件
来源：http://hz.shuidangran.top/gtoukgecqk.html

find . -name "*.log" -type f
来源：http://hz.xinyue.icu/gtngruapeh.html

[R44] 按修改时间查找
来源：http://hz.svipenyu.cn/gthmzxrzwg.html

find . -mtime -7 -type f
来源：http://hz.sxryk.cn/gtkkfnmxdo.html

[R45] 批量删除
来源：http://hz.jlsjyb.cn/gtgxhtzsxf.html

find . -name "*.tmp" -delete
来源：http://hz.aizwys.cn/gtvmzlntdj.html

[R46] 递归替换文件内容
来源：http://hz.cqqwz.cn/gtjfsqatal.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hongshengwenyu.top/gtqugbbqqs.html

[R47] sed 单行替换
来源：http://hz.pengpengdd.cyou/gtafppfjwr.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xziqi.cn/gtgsjdnivg.html

[R48] awk 取指定列
来源：http://hz.c1oappe.top/gtvvlzmixh.html

awk '{print $1, $3}' a.txt
来源：http://hz.yongpay.top/gthjnjirnp.html

[R49] awk 带条件
来源：http://hz.c1oappe.top/gtcokjelhc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jqgufenzy.top/gtrrhkaqnc.html

[R50] awk 求和
来源：http://hz.aizwys.cn/gtuqdiikpn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhijiandao.cn/gtqijnking.html

[R51] 排序去重取前几
来源：http://hz.aizwys.cn/gtczeuvssb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.guowangkeji.top/gtqjeoihpo.html

[R52] 统计行数
来源：http://hz.jinghuilouyu.cn/gtifdvrqwf.html

wc -l a.txt
来源：http://hz.xuetiantiany.cn/gtoasrsjhu.html

[R53] 查看文件头与实时尾
来源：http://hz.hnqzz.top/gtoumigtfp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ydzc1.top/gthwwllppe.html

[R54] 比较两个文件
来源：http://hz.nwbrower.top/gtwkjdhpfx.html

diff a.txt b.txt
来源：http://hz.zhiwuduotai.top/gtalpzrpdk.html

[R55] 压缩与解压
来源：http://hz.cheryme.top/gtqfqabtdq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.dianchejie.cn/gtbxejsovy.html

[R56] 远程拷贝
来源：http://hz.ppjwa.cn/gtbjobbjyf.html

scp file user@host:/path/
来源：http://hz.smart0.xyz/gtcpuberaz.html

[R57] 远程执行命令
来源：http://hz.redwolf501.top/gtylwlpdxn.html

ssh user@host 'uptime'
来源：http://hz.xingfuxueyuan.xyz/gtznfvbuwj.html

[R58] 下载文件
来源：http://hz.cheryme.top/gtboltfrwz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.tanke756.top/gttdtbhfbx.html

[R59] 发 POST JSON
来源：http://hz.yonumen.top/gtvonkevoj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cqqwz.cn/gtkgjxvjvw.html

[R60] 只看 HTTP 状态码
来源：http://hz.316326.xyz/gtpuvxspgl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.pengpengdd.cyou/gtciqoljvt.html

[R61] 磁盘占用
来源：http://hz.zycfv.cn/gtczcqhgxy.html

df -h;  du -sh *
来源：http://hz.wangdashe.top/gtwrgkivow.html

[R62] 找最占空间的文件
来源：http://hz.tanke756.top/gttgqfuguh.html

du -ah . | sort -rh | head -10
来源：http://hz.sysykeji.top/gtgetbkmic.html

[R63] 内存与进程
来源：http://hz.xuetiantiany.cn/gtdfugoewk.html

free -h;  ps aux | grep nginx
来源：http://hz.gogol.net.cn/gtfzjsujph.html

[R64] 结束进程
来源：http://hz.gzhubu.top/gtmbjwobuw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.tianlin.xyz/gtaeovoujd.html

[R65] 查看端口占用
来源：http://hz.cheryme.top/gthwyjjnsp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.snrcjt.cn/gtjbuknntq.html

[R66] 定时任务
来源：http://hz.jqgfzy.top/gtpnrwotxi.html

crontab -e;  crontab -l
来源：http://hz.bjfxy.top/gtmenmtijc.html

[R67] 生成随机十六进制串
来源：http://hz.quarkkingdee.top/gtekhshekb.html

openssl rand -hex 16
来源：http://hz.shanyushiyangtech.top/gtaawcfhjs.html

[R68] 计算文件校验值
来源：http://hz.chenlongwang.top/gthdiviuir.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ehwqpu.com/gtgtwllnuz.html

[R69] 生成随机密码
来源：http://hz.haohaochexian.top/gtjeayouqd.html

head -c 16 /dev/urandom | base64
来源：http://hz.hywenlv.cn/gtudsvtgrx.html

[R70] 时间戳与互转
来源：http://hz.snrcjt.cn/gtfiwrkhip.html

date +%s;  date -d @1700000000
来源：http://hz.gogol.net.cn/gtgxipvzlg.html

[R71] 日期格式化
来源：http://hz.ydzc1.top/gtuuymojuc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.smart0.xyz/gtiawkwozw.html

[R72] 等待端口就绪
来源：http://hz.yj20258.top/gtcwfgwwbg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jianghu66.top/gtwgbgfbxi.html

[R73] 分割大日志
来源：http://hz.316326.xyz/gtdlqtoqze.html

split -l 1000 big.log part_
来源：http://hz.andypj.xyz/gthqspgimq.html

[R74] 批量重命名
来源：http://hz.jlsjyb.cn/gtabyonqfw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hnxiangtu.top/gtuhzwwsly.html

[R75] 导出环境变量
来源：http://hz.zhixingplan.top/gtvareykmt.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.tanke756.top/gtjvggdmqn.html

[R76] 使用临时文件
来源：http://hz.xinyue.icu/gtbkppcwfc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenzaomai.com/gtcnlxjnxy.html

[R77] 读取用户输入
来源：http://hz.zhoulong.xyz/gtpzqlqawp.html

read -rp "请输入: " ans
来源：http://hz.andypj.xyz/gtcnizwugv.html

[R78] 交互式菜单
来源：http://hz.smart0.xyz/gtftxrwlbm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.nwbrower.top/gtddshdeyz.html

[R79] 解析命令行选项
来源：http://hz.sufxvd.cn/gteksalbrv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.redwolf501.top/gtahzcaqcy.html

[R80] 查看脚本执行耗时
来源：http://hz.zhengqikj.top/gtlzjmkthc.html

time ./run.sh
来源：http://hz.ehwqpu.com/gtdbsjezpp.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtluntgjjz.html

S. C / C++ 专题
来源：http://hz.shzxlz.cn/gtxhtbnnbp.html

================================================================================
来源：http://hz.jinqigfzy.top/gthwwdgsar.html

[S01] C：Hello World
来源：http://hz.hywenlv.cn/gtwmzhoaqc.html

#include <stdio.h>
来源：http://hz.dashuyun.cn/gtqbuvfufo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.aizwys.cn/gtbelplprg.html

[S02] C：变量与格式化输出
来源：http://hz.yuxming.cn/gtjotqhjjr.html

int a = 10; printf("%d\n", a);
来源：http://hz.yj20258.top/gtbemlujbe.html

[S03] C：读入整数
来源：http://hz.chenjidiqi.icu/gtxjhizanr.html

int x; scanf("%d", &x);
来源：http://hz.zhongyouzk.top/gtfdzaiaef.html

[S04] C：字符串复制
来源：http://hz.shuidangran.top/gtcpvntcso.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hfpthk.cn/gtvffwgdnm.html

[S05] C：字符串长度
来源：http://hz.9152youxi.cn/gtaubdyzzh.html

strlen(s)
来源：http://hz.havefunace.top/gtjxtbyade.html

[S06] C：字符串比较
来源：http://hz.yonumen.top/gtzcdzqgov.html

strcmp(a, b) == 0
来源：http://hz.jinghuilouyu.cn/gtrbzkvqpd.html

[S07] C：数组遍历求和
来源：http://hz.gotoacloud.top/gtfmaatstc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.0kj1m.cn/gtogipazim.html

[S08] C：动态内存分配与释放
来源：http://hz.tianlin.xyz/gtyxyzifzp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ybcxt.top/gtrrfyxjbb.html

[S09] C：结构体定义与初始化
来源：http://hz.yongpay.top/gtavlxtwve.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cheryme.top/gtduyovkbr.html

[S10] C：指针与解引用
来源：http://hz.xuetiantiany.cn/gtpxkkkfga.html

int *p = &a;  *p = 5;
来源：http://hz.gotoacloud.top/gtqjogfmrv.html

[S11] C：逐行读文件
来源：http://hz.quarkkingdee.top/gtmeffggir.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cucudq.cn/gtluuyotme.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hfpthk.cn/gtdpgtlzgf.html

fclose(f);
来源：http://hz.zhiwuduotai.top/gtrqvihjnv.html

[S12] C：写文件
来源：http://hz.zhaomingkeji.xyz/gtkrvgentw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.daria6918.cn/gtxirmtaxe.html

[S13] C：宏定义
来源：http://hz.xziqi.cn/gtzrsigphi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yvedp.cn/gtksvpvrsi.html

[S14] C：枚举
来源：http://hz.cqqwz.cn/gtvosnekpg.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ydzc1.top/gtqnoerdia.html

[S15] C：类型转换
来源：http://hz.tanke756.top/gtlxkzddux.html

(double) a / b
来源：http://hz.sxryk.cn/gtshmspyzs.html

[S16] C：位操作置位
来源：http://hz.ivvv.top/gtarjctrwe.html

x |= (1 << 3);
来源：http://hz.smart0.xyz/gtjympmtdt.html

[S17] C：安全拼接字符串
来源：http://hz.shanyushiyangtech.top/gtrtiyieqb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xuetiantiany.cn/gtxruvhzud.html

[S18] C：命令行参数
来源：http://hz.cqqwz.cn/gtuzuflrmh.html

int main(int argc, char **argv)
来源：http://hz.jinghuilouyu.cn/gtfblidhsv.html

[S19] C：快速排序
来源：http://hz.sweek.top/gtxvwepwdm.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yonumen.top/gtfxgtxhls.html

[S20] C：二分查找
来源：http://hz.daxiang520.top/gtiwtgrrzw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.fengsongda.top/gtcuhwkhfg.html

[S21] C：字符类别判断
来源：http://hz.smart0.xyz/gtkbfwcynp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.bjfxy.top/gtxqkyewch.html

[S22] C：字符串转数字
来源：http://hz.zhiwuduotai.top/gtsakwbnce.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xuetiantiany.cn/gtcwvvcwng.html

[S23] C：随机数
来源：http://hz.pengpengdd.cyou/gtvhojazhf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.52xcode.cn/gtbhivcrdm.html

[S24] C：获取本地时间
来源：http://hz.cashguo.top/gtnbyupfsy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.gotoacloud.top/gthaztaulc.html

[S25] C：内存拷贝
来源：http://hz.shanyushiyangtech.top/gtmgxopuys.html

memcpy(dst, src, n);
来源：http://hz.yvedp.cn/gtxpujuhrb.html

[S26] C：内存清零
来源：http://hz.xuetiantiany.cn/gtljqzxfah.html

memset(a, 0, sizeof a);
来源：http://hz.0kj1m.cn/gthnquzdod.html

[S27] C：定义常量
来源：http://hz.hysaishi.cn/gtcclglehf.html

const double PI = 3.14159;
来源：http://hz.hammf.cn/gtapsuqifq.html

[S28] C：静态变量
来源：http://hz.guannengcc.top/gtnniilzdu.html

static int counter = 0;
来源：http://hz.havefunace.top/gtzcghnbgk.html

[S29] C：变参函数
来源：http://hz.chenjidiqi.icu/gtdxvzmqrm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinghuilouyu.cn/gtnhudztal.html

[S30] C：头文件保护
来源：http://hz.9152youxi.cn/gtonawxbeg.html

#ifndef X_H
来源：http://hz.zhijiandao.cn/gtmojtqrqr.html

#define X_H
来源：http://hz.shuidangran.top/gtbnucgggv.html

#endif
来源：http://hz.jianghu66.top/gtffsygdme.html

[S31] C++：Hello World
来源：http://hz.nanxinkj.top/gtkdjbaohy.html

#include <iostream>
来源：http://hz.zhijiandao.cn/gtphgaafqn.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.bjfxy.top/gtufirvpwz.html

[S32] C++：字符串
来源：http://hz.ydzc1.top/gtbrepwuhh.html

std::string s = "hi";  s += "!";
来源：http://hz.yj202588.top/gtdkghftzu.html

[S33] C++：vector 增删
来源：http://hz.yongpay.top/gtrnlzaahh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tianlin.xyz/gtkqlwyjux.html

[S34] C++：遍历 vector
来源：http://hz.chenlongwang.top/gtzxhjyzdm.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sysykeji.top/gtvcobxyvb.html

[S35] C++：map
来源：http://hz.ydzc1.top/gtpstececu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cdnleiting.top/gtzrfffvvj.html

[S36] C++：unordered_map
来源：http://hz.zhengqikj.top/gtkoaplwaz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenlongwang.top/gtuwvgtnye.html

[S37] C++：set
来源：http://hz.guannengcc.top/gtcmworfdh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.iojbl.cn/gtvzxwixxe.html

[S38] C++：排序
来源：http://hz.0kj1m.cn/gtuzhkdbox.html

std::sort(v.begin(), v.end());
来源：http://hz.cdnleiting.top/gtgnkwryrn.html

[S39] C++：自定义比较器排序
来源：http://hz.sweek.top/gtylcclwic.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.smart0.xyz/gtndtwtzeg.html

[S40] C++：查找元素
来源：http://hz.svipenyu.cn/gtwsgscels.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jianghu66.top/gtvjdfkjnn.html

[S41] C++：类与构造函数
来源：http://hz.ydzc1.top/gttorelkdg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sweek.top/gtuyiuswep.html

[S42] C++：继承与虚函数
来源：http://hz.52xcode.cn/gtctbwxina.html

class B : public Base { public: void f() override {} };
来源：http://hz.sufxvd.cn/gtjpyjdbln.html

[S43] C++：智能指针
来源：http://hz.yonumen.top/gtclzejfez.html

auto p = std::make_unique<int>(5);
来源：http://hz.andypj.xyz/gttjovlvcd.html

[S44] C++：引用传参
来源：http://hz.zhixingplan.top/gtzsecvnwa.html

void inc(int &x) { ++x; }
来源：http://hz.meibo888.top/gtwirmdvqu.html

[S45] C++：lambda
来源：http://hz.cheryme.top/gtgfcaxmoj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jqgufenzy.top/gtapjrqidg.html

[S46] C++：函数模板
来源：http://hz.sxryk.cn/gtuchzqqrm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.c1oappe.top/gtsptaqluo.html

[S47] C++：结构化绑定遍历
来源：http://hz.tanke756.top/gtujmrimkm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yj202588.top/gtzeqjvjyx.html

[S48] C++：逐行读文件
来源：http://hz.xziqi.cn/gtdvljakhw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenzaomai.com/gtxgzwhaed.html

while (std::getline(in, line)) { }
来源：http://hz.jinyuanbaomall.cn/gtyonxvghf.html

[S49] C++：写文件
来源：http://hz.redwolf501.top/gtrybjwwpd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yj20258.top/gtgozuhwll.html

[S50] C++：格式化数字
来源：http://hz.jqgfzy.top/gtqfvlqsua.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhongyouzk.top/gtkmvejkjn.html

[S51] C++：显式类型转换
来源：http://hz.jqgufenzy.top/gtmyjffoze.html

static_cast<double>(a) / b
来源：http://hz.zhiwuduotai.top/gtpxyzsjrq.html

[S52] C++：const 与 noexcept
来源：http://hz.yj202588.top/gtdvxumzpq.html

int size() const noexcept { return n_; }
来源：http://hz.chenjidiqi.icu/gtpkgepgfk.html

[S53] C++：移动语义
来源：http://hz.daxiang520.top/gtwviniclr.html

std::vector<int> w = std::move(v);
来源：http://hz.hysaishi.cn/gtbmmitwwe.html

[S54] C++：异常处理
来源：http://hz.nanxuanxn.top/gtpbqisxdz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yongpay.top/gtlziqqrrq.html

[S55] C++：结构化绑定
来源：http://hz.gogol.net.cn/gtjxyhiemt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhoulong.xyz/gtzvebvayr.html

[S56] C++：optional
来源：http://hz.zhiwuduotai.top/gthonvoztm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xylfe.cn/gtodncmwpo.html

[S57] C++：编译期常量
来源：http://hz.aibaodan.cn/gtuubalmdf.html

constexpr int N = 10;
来源：http://hz.bjfxy.top/gtlkbjdmlq.html

[S58] C++：命名空间
来源：http://hz.sufxvd.cn/gtpgnaevpy.html

namespace ns { int f() { return 1; } }
来源：http://hz.hywenlv.cn/gtovmedukw.html

[S59] C++：静态断言
来源：http://hz.ybcxt.top/gtdnahcfrq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.wangdashe.top/gtkkeyoiqc.html

[S60] C++：遍历并删除元素
来源：http://hz.zhixingplan.top/gtkuzirwre.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yvedp.cn/gtgtthiqrj.html

================================================================================
来源：http://hz.cheryme.top/gtyfmsukmy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj20258.top/gtfidnwszr.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtwzpjctrg.html

[T01] Kotlin：Hello World
来源：http://hz.svipenyu.cn/gthaqtdaqk.html

println("Hello")
来源：http://hz.nanxinkj.top/gtkxjkksny.html

[T02] Kotlin：变量
来源：http://hz.0kj1m.cn/gtswgtyeuw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.gogol.net.cn/gtqvzuqgtt.html

[T03] Kotlin：字符串模板
来源：http://hz.bjfxy.top/gtubnelzar.html

"值: $b"
来源：http://hz.cashguo.top/gtmozkgrfz.html

[T04] Kotlin：空安全
来源：http://hz.feifeiyinyue.top/gtceuttttz.html

val n: String? = null;  n?.length
来源：http://hz.316326.xyz/gtyhqzvugk.html

[T05] Kotlin：when 表达式
来源：http://hz.chenlongwang.top/gtmimtwvtn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhiwuduotai.top/gtgmbokwui.html

[T06] Kotlin：集合映射
来源：http://hz.chenjidiqi.icu/gtwfesfbat.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.tanke756.top/gtcylpkpdg.html

[T07] Kotlin：集合过滤
来源：http://hz.hnqzz.top/gthoonxdas.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zycfv.cn/gttnutbvfl.html

[T08] Kotlin：数据类
来源：http://hz.pengpengdd.cyou/gttohrtogm.html

data class User(val name: String, val age: Int)
来源：http://hz.ywan-chungtsiang.top/gthjgxhoji.html

[T09] Kotlin：扩展函数
来源：http://hz.zhixingplan.top/gttciqqjuw.html

fun String.exclaim() = this + "!"
来源：http://hz.xuetiantiany.cn/gtphavjkzl.html

[T10] Kotlin：默认参数
来源：http://hz.hfpthk.cn/gtecpoqoix.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.iojbl.cn/gtjajptsam.html

[T11] Kotlin：协程
来源：http://hz.ydzc1.top/gtvdftrmsm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.cashguo.top/gtxrtnqwms.html

[T12] Kotlin：解构声明
来源：http://hz.snrcjt.cn/gtuoaeshlj.html

val (a, b) = Pair(1, 2)
来源：http://hz.chenjidiqi.icu/gtqoospnnx.html

[T13] Kotlin：只读 Map
来源：http://hz.shangyingyoupin.top/gtpuezzfbe.html

val m = mapOf("a" to 1)
来源：http://hz.yangfankeji.com/gtvrpeuzzb.html

[T14] Kotlin：循环
来源：http://hz.zdqjudy.top/gtywtpjzcs.html

for (i in 1..10) println(i)
来源：http://hz.zycfv.cn/gtpfifvpne.html

[T15] Kotlin：接口
来源：http://hz.cdnleiting.top/gtjovscckt.html

interface Shape { fun area(): Double }
来源：http://hz.ybcxt.top/gtdirdpacq.html

[T16] Swift：Hello World
来源：http://hz.iojbl.cn/gtxnqvwsnc.html

print("Hello")
来源：http://hz.hammf.cn/gtivdsviqd.html

[T17] Swift：变量与常量
来源：http://hz.jqgufenzy.top/gthqrxbioc.html

var a = 1;  let b = 2
来源：http://hz.gaohongyu789.top/gthvlzxnlw.html

[T18] Swift：字符串插值
来源：http://hz.sysykeji.top/gtososfgcg.html

"值: \(b)"
来源：http://hz.feifeiyinyue.top/gtrzsggvym.html

[T19] Swift：可选绑定
来源：http://hz.feifeiyinyue.top/gtbsivuqvo.html

if let n = opt { print(n) }
来源：http://hz.pycfn.com/gtitcitlun.html

[T20] Swift：数组操作
来源：http://hz.tianlin.xyz/gtytsekmjl.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hywenlv.cn/gtklcbjbvv.html

[T21] Swift：遍历
来源：http://hz.snrcjt.cn/gtaelmphyt.html

for x in a { print(x) }
来源：http://hz.chenzaomai.com/gtmcpoisaz.html

[T22] Swift：字典
来源：http://hz.gogol.net.cn/gtmpbqfuyb.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ybcxt.top/gtwhbxidmj.html

[T23] Swift：函数
来源：http://hz.cqqwz.cn/gtsoflzpab.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.chenlongwang.top/gtmtwvbtmx.html

[T24] Swift：闭包
来源：http://hz.ybcxt.top/gtfhjsmbym.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.chenlongwang.top/gtmkxrnito.html

[T25] Swift：结构体
来源：http://hz.cqqwz.cn/gtzbrufgwu.html

struct P { var x: Int }
来源：http://hz.yj20258.top/gtmrjtpggb.html

[T26] Swift：类与重写
来源：http://hz.jiagoushi.top/gtsymiqrah.html

class A: Base { override func f() {} }
来源：http://hz.snrcjt.cn/gtaqcotyjn.html

[T27] Swift：错误处理
来源：http://hz.daxiang520.top/gtjwrgvukc.html

do { try f() } catch { print(error) }
来源：http://hz.xylfe.cn/gtyqmefozk.html

[T28] Swift：枚举
来源：http://hz.yanxiufei.cn/gtbzuaithf.html

enum Color { case red, green }
来源：http://hz.hysaishi.cn/gtajksfdpz.html

[T29] Swift：guard 提前返回
来源：http://hz.svipenyu.cn/gtwdzsfxud.html

guard let x = opt else { return }
来源：http://hz.smart0.xyz/gtgbdjwdej.html

[T30] Swift：协议
来源：http://hz.guowangkeji.top/gttwdslfoe.html

protocol Shape { func area() -> Double }
来源：http://hz.cqqwz.cn/gtncdhradf.html

[T31] Lua：Hello World
来源：http://hz.hnqzz.top/gtvubcsqhb.html

print("Hello")
来源：http://hz.fzhhl.top/gtluizojnh.html

[T32] Lua：局部变量
来源：http://hz.yj202588.top/gtnjigdjcs.html

local a = 1
来源：http://hz.sxryk.cn/gtltujygqx.html

[T33] Lua：表（数组）
来源：http://hz.dashuyun.cn/gtotcqmrcb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yonumen.top/gtkerkpfrm.html

[T34] Lua：遍历表
来源：http://hz.smart0.xyz/gtcbuuhosy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.316326.xyz/gttimhupir.html

[T35] Lua：字典表
来源：http://hz.yonumen.top/gtxbcgmjjh.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hnxiangtu.top/gtgjqcfkbo.html

[T36] Lua：函数
来源：http://hz.yongpay.top/gtzudsexki.html

function add(a, b) return a + b end
来源：http://hz.zycfv.cn/gtykzoicwk.html

[T37] Lua：字符串拼接
来源：http://hz.yj202588.top/gtmhovixcn.html

"a" .. "b"
来源：http://hz.kuanghao11.cn/gtpaeavnya.html

[T38] Lua：条件
来源：http://hz.jyoumei.cn/gtcroiglcq.html

if x > 0 then print("正") end
来源：http://hz.zycfv.cn/gtvvenhoui.html

[T39] Lua：模式匹配
来源：http://hz.redwolf501.top/gtlbdpyncd.html

string.find(s, "%d+")
来源：http://hz.jiagoushi.top/gtrzcrflma.html

[T40] Lua：元表
来源：http://hz.ppjwa.cn/gthmsuldvs.html

setmetatable({}, { __index = base })
来源：http://hz.wangshuangyany.cn/gtluongvhv.html

[T41] Perl：Hello World
来源：http://hz.zhongyouzk.top/gtzgcjnfxn.html

print "Hello\n";
来源：http://hz.hammf.cn/gtvnqbaflp.html

[T42] Perl：变量类型
来源：http://hz.wangdashe.top/gtlmnzxigm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.ywan-chungtsiang.top/gtpnlchrzm.html


<!-- 参考信息 -->